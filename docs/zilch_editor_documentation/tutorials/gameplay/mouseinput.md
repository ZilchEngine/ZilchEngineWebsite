This lesson covers using the mouse in the Zilch Engine.

 #  Learning Objectives

- Learning how to respond to mouse events
- Understanding how to convert from *screen space// to //world space*

 #  Level Setup

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ New Project](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#newproject)
 - Create a new project using the {nav icon=clone, name=Empty 2D Project} template

 #  Mouse Events

The easiest way to get mouse input in the Zilch Engine is via **mouse events**. Mouse events can be used to detect when the mouse is moved, when the cursor enters or exits an object, when the buttons are pressed or released, and so on. We'll begin by making an object that responds to mouse events by inflating like a balloon.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ CreateSphere](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsphere)
- In the `Properties Window`
 - Rename Sphere object to `Balloon`
 - [ Remove Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [ RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
 - [ Remove Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [ SphereCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spherecollider.md)



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/105388.png)


In order for the balloon to respond to mouse input, it needs the [ Reactive](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/reactive.md) component, which makes an object receive mouse events.

- In the `Properties Window`
 - [ Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [ Reactive](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/reactive.md)

Now we can add the code that will make the balloon inflate.

 ##  Update-Based Mouse Input

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `ScaleWithMouseEvents`
- Update the `ScaleWithMouseEvents` script to the following:

```lang=csharp, name="ScaleWithMouseEvents"
class ScaleWithMouseEvents : NadaComponent
{
  [Dependency] var Transform : Transform;
  [Dependency] var Reactive : Reactive;
  
  [Property]
  var ScaleRate : Real = 1.5;
  [Property]
  var MaxScale : Real3 = Real3(8);
  
  function Initialize(init : CogInitializer)
  {
    // The MouseUpdate event is dispatched to a Reactive
    // object every frame that the mouse cursor is over it
    Zilch.Connect(this.Owner, Events.MouseUpdate, this.OnMouseUpdate);
  }
  
  function OnMouseUpdate(event : ViewportMouseEvent)
  {
    // The ViewportMouseEvent lets us check whether the left mouse button is
    // currently held. If it is, we call a function that makes this object grow
    if (event.IsButtonDown(MouseButtons.Left))
      this.Grow();
  }
  
  function Grow()
  {
    // By starting from whatever the current scale is at the moment and taking
    // a small step toward the target max scale, the object will asymptotically
    // approach that maximum
    var dt = this.Space.TimeSpace.Dt;
    var currentScale = this.Transform.LocalScale;
    var newScale = Math.Lerp(currentScale, this.MaxScale, this.ScaleRate * dt);
    this.Transform.LocalScale = newScale;
  }
}
```

This component will let the user set a maximum scale to grow to, and then it will cause the balloon to inflate as long as the left mouse button is held while the cursor is over it, up to that max scale.

- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Balloon object
- In the `Properties Window`
 - [ Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `ScaleWithMouseEvents`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
 - `Click and hold` the left mouse button over the sphere to cause it to grow



![ScaleWithMouseEvents Demonstration](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/105397.gif)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

This method of implementing mouse controls by checking what the mouse is doing in an update function is known as **update-based** input.

Now let's add a bit more functionality to this component.

 ##  Reaction-Based Mouse Input

- Update the `ScaleWithMouseEvents` script to the following:

```lang=csharp, name="ScaleWithMouseEvents, updated"
class ScaleWithMouseEvents : NadaComponent
{
  [Dependency] var Transform : Transform;
  [Dependency] var Reactive : Reactive;
  
  [Property]
  var ScaleRate : Real = 1.5;
  [Property]
  var MaxScale : Real3 = Real3(8);
  [Property]
  var ShrinkDuration : Real = 1;
  
  var InitialScale : Real3;
  var ShrinkSequence : ActionSet;
  
  function Initialize(init : CogInitializer)
  {
    this.InitialScale = this.Transform.LocalScale;
    this.ShrinkSequence = Action.Sequence(this.Owner.Actions);
    
    // The MouseUpdate event is dispatched to a Reactive
    // object every frame that the mouse cursor is over it
    Zilch.Connect(this.Owner, Events.MouseUpdate, this.OnMouseUpdate);
    Zilch.Connect(this.Owner, Events.RightMouseDown, this.OnRightMouseDown);
  }
  
  function OnRightMouseDown(event : ViewportMouseEvent)
  {
    if (!this.ShrinkSequence.Active)
      this.Shrink();
  }
  
  function OnMouseUpdate(event : ViewportMouseEvent)
  {
    // The ViewportMouseEvent lets us check whether the left mouse button is
    // currently held. If it is, we call a function that makes this object grow
    if (event.IsButtonDown(MouseButtons.Left) && !this.ShrinkSequence.Active)
      this.Grow();
  }
  
  function Grow()
  {
    // By starting from whatever the current scale is at the moment and taking
    // a small step toward the target max scale, the object will asymptotically
    // approach that maximum
    var dt = this.Space.TimeSpace.Dt;
    var currentScale = this.Transform.LocalScale;
    var newScale = Math.Lerp(currentScale, this.MaxScale, this.ScaleRate * dt);
    this.Transform.LocalScale = newScale;
  }
  
  function Shrink()
  {
    // We can reduce the scale of this object back to its initial value with a
    // single click by using an Action
    this.ShrinkSequence = Action.Sequence(this.Owner.Actions);
      
      Action.Property(this.ShrinkSequence, @this.Transform.LocalScale,
        this.InitialScale, this.ShrinkDuration, Ease.BounceOut);
  }
}
```

Now the right mouse button can be used to deflate the balloon.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
 - `Click and hold` the left mouse button over the sphere to cause it to grow, and `right click` the sphere to cause it to shrink



![ScaleWithMouseEvents Second Demonstration](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/105444.gif)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

Now this component also connects to the [ RightMouseDown](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/event_reference.md#rightmousedown) event, which is dispatched to a Reactive object when the right mouse button is pressed while the cursor is over it. In its `OnRightMouseDown` callback function, it checks to make sure the balloon isn't already shrinking, and if it isn't, it calls a function that makes it shrink.

This method of implementing mouse controls by connecting to relevant mouse events and only running code when those events are dispatched is called **reaction-based** input.

 #  Screen Space and World Space

As we've seen already, mouse events are dispatched with the [ ViewportMouseEvent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/viewportmouseevent.md) class. Among other information, this includes the position of the mouse event, which we can see by printing it out.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `PrintPositionOnMouseDown`
- Update the `PrintPositionOnMouseDown` script to the following:

```lang=csharp, name="PrintPositionOnMouseDown"
class PrintPositionOnMouseDown : NadaComponent
{
  function Initialize(init : CogInitializer)
  {
    Zilch.Connect(this.Space, Events.MouseDown, this.OnMouseDown);
  }
  
  function OnMouseDown(event : ViewportMouseEvent)
  {
    var mousePosition = event.Position;
    Console.WriteLine(mousePosition);
  }
}
```

- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : LevelSettings object
- In the `Properties Window`
 - [ Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `PrintPositionOnMouseDown`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Console](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#console)
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
 - Click  around the screen a few times



![Screen Space Mouse Event Positions](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/106024.gif)


When you click the mouse, positions are printed to the console. Notice that these numbers are pretty big, they're all whole numbers, and no matter where you click, they're never negative. Furthermore, they're all 2D vectors. These are what are called **screen-space coordinates**: they refer to the pixel on your screen where the click occurred. In this form, they're a bit hard to use in a game. What we need is a way to convert them from screen space into **world space**, where the objects in our game exist. Fortunately, that's easy.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

The [ ViewportMouseEvent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/viewportmouseevent.md) contains a set of functions that can be used to convert the event's screen space position into world space: `ToWorldPlane`, `ToWorldViewPlane`, and `ToWorldZPlane`. Each of them has its purpose, but it's common in 2D games to make extensive use of that last one, `ToWorldZPlane`. This function projects a screen-space position onto a Z-aligned world plane at a given Z value. If you give it a value of, say, `0`, then it will return the world-space coordinates of the mouse event at a Z-depth of zero. In a typical 2D game, this is generally the most basic way to get the world position of the mouse.

- Replace the `OnMouseDown` function in the `PrintPositionOnMouseDown` class with the following:

```lang=csharp, name="PrintPositionOnMouseDown, updated"
function OnMouseDown(event : ViewportMouseEvent)
{
  var mousePosition = event.ToWorldZPlane(0);
  Console.WriteLine(mousePosition);
}
```

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
 - Click  around the screen a few times



![World Space Mouse Event Positions](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/106026.gif)


The positions that are now being printed to the console are now in world units, rather than screen pixel coordinates. This is generally much more useful for programming game logic.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

Now that we know how to find the world-space position of a mouse event, we can move things to the mouse's position, like, say, our balloon. First, though �

- [ Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : LevelSettings object
- In the `Properties Window`
 - [ Remove Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `PrintPositionOnMouseDown`

It's good practice to remove or comment out console print statements when you're done with them.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `MoveOnMiddleMouseDown`
- Update the `MoveOnMiddleMouseDown` script to the following:

```lang=csharp, name="MoveOnMiddleMouseDown"
class MoveOnMiddleMouseDown : NadaComponent
{
  [Dependency] var Transform : Transform;
  
  [Property]
  var MoveDuration : Real = 0.25;
  
  function Initialize(init : CogInitializer)
  {
    Zilch.Connect(this.Space, Events.MiddleMouseDown, this.OnMiddleMouseDown);
  }
  
  function OnMiddleMouseDown(event : ViewportMouseEvent)
  {
    var destination = event.ToWorldZPlane(0);
    Action.Property(this.Owner.Actions, @this.Transform.WorldTranslation,
      destination, this.MoveDuration, Ease.QuadInOut);
  }
}
```

This component will make whatever we attach it to animate its position to the world-space coordinates of the mouse whenever the middle mouse button is pressed.

- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Balloon object
- In the `Properties Window`
 - [ Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `MoveOnMiddleMouseDown`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
 - Use the middle mouse button to move the balloon, and the left and right mouse buttons to inflate and deflate it



![Balloon Moving to Mouse World Position](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/106030.gif)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

 #  Related Materials
 ##  Manual
- [commands](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md)
- [addremovecomponent](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md)
- [selectobject](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md)
- [resourceadding](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 ##  Reference
 ###  Commands
- [ NewProject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#newproject)
- [ CreateSphere](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsphere)
- [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
- [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)
- [ Console](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#console)
 ###  Classes
- [rigidbody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
- [spherecollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spherecollider.md)
- [reactive](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/reactive.md)
- [viewportmouseevent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/viewportmouseevent.md)
 ###  Events
- [ MouseUpdate](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/event_reference.md#mouseupdate)
- [ RightMouseDown](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/event_reference.md#rightmousedown)
- [ MiddleMouseDown](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/event_reference.md#middlemousedown)
 ##  Development Task
- {T1185}
 

 
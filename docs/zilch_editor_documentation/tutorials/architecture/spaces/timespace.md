Having already seen [spaces](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/tutorials/architecture/spaces.md) in a previous tutorial, we will now talk about a component that only appears on space objects: the [TimeSpace](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/timespace.md).


 #  Learning Objectives


- TimeScale
- Pausing


 #  Level Setup


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ New Project](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#newproject)
 - Create a new project using the {nav icon=clone, name=Empty 2D Project} template
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- In the `Properties Window`
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [BoxCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md)
 - Under [RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
  - Set `name=DynamicState,icon=list` to [Static](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#rigidbodydynamicstate)
 - Under [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Scale  to `[25,1,1]`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSphere](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsphere)
- In the `Properties Window`
 - Under [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Translation  to `[-10,5,0]`
 - Under [RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
  - Set Velocity  to `[10,0,0]`


 #  What is the TimeSpace?


The [TimeSpace](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/timespace.md) component allows for developer control over time in the space it is attached to. Time in that space can be slowed or even stopped. Let's see what the demo looks like right now to get a frame of reference.

  - [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![control](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/94788.gif)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

The ball falls, bounces, and rolls at a normal pace for the values it was initialized with.


 ##  TimeScale


A common dramatic effect is to slow down time during some in-game event. Slow motion effects are typically implemented via the [TimeScale](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/timespace.md#timescale-zilch-engine-do) property, which is a scalar for the rate at which time passes. There are also some times where running your project at a slower speed will allow you to debug issues more easily. Let's take a look at how to change TimeScale  using the UI.

(NOTE)**Space Selection**:
 The [Space](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md) can be selected via the `Select` menu, by clicking in the viewport and then pressing `Shift + S`, by pressing `Ctrl + Shift + S` with any window in focus, or by using the [ SelectSpace](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#selectspace) command.
 ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/94805.png)

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ SelectSpace](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#selectspace)
- In the `Properties Window`
 - Under [TimeSpace](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/timespace.md)
  - Set TimeScale  to `0.5`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![halfspeed](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/94807.gif)


*Demo running half speed with `0.5` TimeScale*


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

Now we can see that the time scale directly affects the rate of time without affecting the framerate.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ SelectSpace](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#selectspace)
- In the `Properties Window`
 - Under [TimeSpace](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/timespace.md)
  - Set TimeScale  to `1.0`


 ##  Adjusting TimeScale In Script


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `TimeControl`
- Update the `TimeControl` script to the following:

```lang=csharp, name="TimeControl"
class TimeControl : NadaComponent
{
  [Property]
  var IncreaseRateKey : Keys = Keys.Up;
  
  [Property]
  var DecreaseRateKey : Keys = Keys.Down;
  
  [Property]
  var TimeScaleRateOfChange : Real = 0.1;
  
  function Initialize(init : CogInitializer)
  {
    Zilch.Connect(this.Space, Events.LogicUpdate, this.OnLogicUpdate);
  }

  function OnLogicUpdate(event : UpdateEvent)
  {
    if(Zilch.Keyboard.KeyIsPressed(this.IncreaseRateKey))
      this.ScaleTime(this.TimeScaleRateOfChange);
      
    if(Zilch.Keyboard.KeyIsPressed(this.DecreaseRateKey))
      this.ScaleTime(-this.TimeScaleRateOfChange);
  }
  
  function ScaleTime(rateChange : Real)
  {
    var newTimeScale = this.Space.TimeSpace.TimeScale + rateChange;
    this.Space.TimeSpace.TimeScale = Math.Clamp(newTimeScale, 0.0, 2.0);
    Console.WriteLine("TimeScale: `this.Space.TimeSpace.TimeScale`");
  }
}
```

- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : LevelSettings object
- In the `Properties Window`
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `TimeControl`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [Console](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#console)
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
 - Adjust the time scale using the `up` and `down` keys



![controlled](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/94790.gif)


*TimeScale  being adjusted up and down*


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

Above we can see the demo progressing slower and then faster as the [TimeScale](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/timespace.md#timescale-zilch-engine-do) is adjusted using the keyboard.


 #  Pausing


- Add the following property to the `TimeControl` script:
```name=PauseKey Property, lang=csharp
  [Property]
  var PauseKey : Keys = Keys.Space;
```

- Add the following function to the `TimeControl` script:
```name=TogglePause, lang=csharp
  function TogglePause()
  {
    if(this.Space.TimeSpace.Paused)
    {
      Console.WriteLine("Game was paused, unpausing now");
      this.Space.TimeSpace.Paused = false;
    }
    else
    {
      Console.WriteLine("Game was not paused, pausing now");
      this.Space.TimeSpace.Paused = true;
    }
  }
```
- Add the following block to the end of the `OnLogicUpdate` function in the `TimeControl` script:
```name=OnLogicUpdate Extension,lang=csharp
    if(Zilch.Keyboard.KeyIsPressed(this.PauseKey))
      this.TogglePause();
```

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
 - Press `Space` to pause the game and then press `Space` again to attempt to unpause the game



![stopped](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/94809.gif)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

You probably noticed that the game will not unpause. This is because when the [TimeSpace](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/timespace.md) is paused, [Keyboard](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/keyboard.md), listening for the [KeyDown](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/event_reference.md#keydown) event, or to poll the keyboard input on [FrameUpdate](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/event_reference.md#frameupdate).

- Update the `Initialize` function in `TimeControl` to the following:
```name=Initialize, lang=csharp
  function Initialize(init : CogInitializer)
  {
    Zilch.Connect(Zilch.Keyboard, Events.KeyDown, this.OnKeyDown);
  }
```

- Replace the `OnLogicUpdate` function in `TimeControl` with the following:
```name=Initialize, lang=csharp
  function OnKeyDown(event : KeyboardEvent)
  {
    if(event.Key == this.IncreaseRateKey)
      this.ScaleTime(this.TimeScaleRateOfChange);
      
    if(event.Key == this.DecreaseRateKey)
      this.ScaleTime(-this.TimeScaleRateOfChange);
    
    if(event.Key == this.PauseKey)
      this.TogglePause();
  }
```

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
 - Press `Space` to pause the game and then press `Space` again to attempt to unpause the game



![pausing](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/94811.gif)


*Pausing with and unpausing in reaction to the [KeyDown](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/event_reference.md#keydown) event*


Now we can see the game being paused and unpaused successfully.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)


 #  Related Materials
 ##  Manual
- [LauncherNewProject](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/launchernewproject.md)
- [commands](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md)
- [selectobject](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md)
- [addremovecomponent](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md)
- [resourceadding](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)

 ##  Reference
 ###  Commands
- [ CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- [ CreateSphere](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsphere)
- [ SelectSpace](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#selectspace)
- [ Console](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#console)
- [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
- [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

 ###  Classes
- [transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
- [timespace](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/timespace.md)
- [rigidbody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
- [boxcollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md)
- [keyboard](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/keyboard.md)

 ###  Events
- [ LogicUpdate](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/event_reference.md#logicupdate)
- [ FrameUpdate](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/event_reference.md#frameupdate)
- [ KeyDown](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/event_reference.md#keydown)

 ##  Development Tasks
- {T1178} 

 
This tutorial covers the basics of what spaces are, how to create them, and how to use them with levels.


 #  Learning Objectives


- Creating new spaces
- Basic HUD
- ClearColor


 #  Level Setup


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ New Project](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#newproject)
 - Create a new project using the {nav icon=clone, name=Empty 2D Project} template
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSpriteText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createspritetext)
- In the `Property Window`
 - Under [SpriteText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spritetext.md)
  - Set Text  to `Game Level SpriteText`
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : GameCamera object
- In the `Properties Window`
 - Under [Camera](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/camera.md)
  - Set Size  to `5`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `HUDManager`


 #  What is a Space?


There have probably been a few times while learning Zilch that you typed `this.Space` but didn't really know what exactly a [Space](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md) was. A [Space](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md) is a special type of object which represents the *space* occupied by objects in a Level resource. Another way to think about it is as an object that represents the dimensions of whichever level is loaded into it, or as 3D area with infinite bounds that contains a level.


 ##  Space Basics


- Each game can have multiple spaces
- Objects in different spaces cannot interact graphically or physically
- Each [Space](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md) (usually) has its own renderer(s) that draws the loaded level to the viewport
- Each [ Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md) and each [ Cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md) contains a member variable that is a reference to the [Space](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md) it exists in


 #  Creating a Space


A very common reason for creating a second space is to implement a HUD that overlays the game. This approach takes advantage of the fact that objects in one space will not directly interact with objects in another. Let's make the level for our first HUD.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a Level resource using the {nav icon=clone, name=2D Level} template and name it `HUDLevel`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSpriteText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createspritetext)
- In the `Property Window`
 - Under [SpriteText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spritetext.md)
  - Set Text  to `HUD Level SpriteText`
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : GameCamera object
- In the `Properties Window`
 - Under [Camera](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/camera.md)
  - Set Size  to `5`
- Open the Level resource named `Level`
- [ Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : LevelSettings object
- In the `Properties Window`
 - [ Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `HUDManager`
- In `HUDManager`
 - Update the `HUDManager` script to the following:
```name=HUDManager, lang=csharp
class HUDManager : NadaComponent
{
  [Property]
  var HUDLevel : Level;
  
  [Property]
  var HUDSpaceArchetype : Archetype = Archetype.Space;
  
  var HUDSpace : Space;
  
  function Initialize(init : CogInitializer)
  {
    this.HUDSpace = this.GameSession.CreateSpace(this.HUDSpaceArchetype);
    this.HUDSpace.LoadLevel(this.HUDLevel);
  }
}
```

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ SaveProject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#saveproject)
- In the `Properties Window`
 - Under `HUDManager`
  - Set HUDLevel window to HUDLevel resource

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/94416.png)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

Notice how the text from the HUDLevel Level resource is visible, but not the text from the game Level resource. This is because by default spaces are rendered as opaque.  


 ##  Overlaying the HUD


- Open the Level resource named `HUDLevel`
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Renderer object
- In the `Properties Window`
 - Under `ForwardRenderer`
  - Set ClearColor  to `[R:0, G:0, B:0, A:0.00]`
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : GameCamera object
- In the `Properties Window`
 - Under [ CameraViewport](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cameraviewport.md)
  - Set RenderOrder  to `1`
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : SpriteText object
- In the `Properties Window`
 - Under [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Translation  to `[0,1,0]`
- Open the Level resource named `Level`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/94418.png)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

Notice that both text objects are now visible. This is because we reduced the alpha value of the HUD level clear color to `0`. The clear color is what is rendered behind everything in a level. We've also set the RenderOrder  of the HUD GameCamera object's [ CameraViewport](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cameraviewport.md) to `1`, while the main space's RenderOrder  remains at its default value of `0`. This is important for layering purposes: no two overlaid [ CameraViewports](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cameraviewport.md) should have the same RenderOrder .

Now that we know how to make a space transparent, it is fairly simple to extrapolate constructing a HUD within a dedicated level and rendering it on top of a game.


 #  Communicating Between Spaces


Having multiple spaces can increase a project's complexity. It is important to know how to allow components which exists in seperate spaces to communicate with each other. Information is often sent between spaces via events. Let's make a basic meter in our HUD.


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `Meter`
- Update the `Meter` script to the following:

```lang=csharp, name="Meter"
class Meter : NadaComponent
{
  [Dependency] var Transform : Transform;
  [Dependency] var Area : Area;
  
  [Property]
  var MaxValue : Real = 10;
  
  var CurrentValue : Real;
  
  var MeterScaleAction : Action;
  
  var OriginalSize : Real2;
  
  var ScaleRate : Real = 1.0;
  
  function Initialize(init : CogInitializer)
  {
    this.CurrentValue = this.MaxValue;
    this.OriginalSize = this.Area.Size;
    Zilch.Connect(this.Space, Events.MeterUpdate, this.OnMeterUpdate);
  }

  function OnMeterUpdate(event : MeterUpdate)
  {
    var val = this.CurrentValue + event.Value;
    this.CurrentValue = Math.Clamp(val, 0.0, this.MaxValue);
    this.ScaleMeter();
  }
  
  function ScaleMeter()
  {
    if(this.MeterScaleAction != null)
      this.MeterScaleAction.Cancel();
    
    //calculate and constrain the new meter size
    var perc = this.CurrentValue / this.MaxValue;
    var targetSize = perc * this.OriginalSize;
    targetSize.Y = this.OriginalSize.Y;
    
    //calculate the duration of the scale action
    var sizeDifference = Math.Abs(this.Area.Size.X - targetSize.X);
    var duration = sizeDifference / this.ScaleRate;
    
    this.MeterScaleAction = Action.Property(this.Owner.Actions, @this.Area.Size, targetSize, duration, Ease.Linear);
  }
}

class MeterUpdate : NadaEvent
{
  sends MeterUpdate : MeterUpdate;
  var Value : Real;
}
```

This `Meter` component will be be *communicated// with via events sent from the //GameSpace// to the //HUDSpace* by the following `Input` component.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `Input`
- Update the `Input` script to the following:
```name=Input, lang=csharp
class Input : NadaComponent
{
  [Dependency] var HUDManager : HUDManager;
  
  [Property]
  var IncreaseKey : Keys = Keys.Up;
  
  [Property]
  var DecreaseKey : Keys = Keys.Down;
  
  [Property]
  var InputValue : Real = 1.0;
  
  function Initialize(init : CogInitializer)
  {
    Zilch.Connect(Zilch.Keyboard, Events.KeyDown, this.OnKeyDown);
  }

  function OnKeyDown(event : KeyboardEvent)
  {
    if(event.Key == this.IncreaseKey)
    {
      Console.WriteLine("Increase");
      this.UpdateMeter(this.InputValue);
    }
    else if(event.Key == this.DecreaseKey)
    {
      Console.WriteLine("Decrease");
      this.UpdateMeter(-this.InputValue);
    }
  }
  
  function UpdateMeter(val : Real)
  {
    var meterUpdateEvent = MeterUpdate();
    meterUpdateEvent.Value = val;
    this.HUDManager.HUDSpace.DispatchEvent(Events.MeterUpdate, meterUpdateEvent);
  }
}
```

This simple input component will allow us to use the meter to simulate the game behavior of losing and gaining health without having to actually implement a game for this tutorial.

- Open the Level resource named `Level`
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : LevelSettings object
- In the `Properties Window`
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `Input`

- Open the Level resource named `HUDLevel`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- In the `Properties Window`
 - Under [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Translation  to `[-2.5, 0.0, 0.0]`
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [Area](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/area.md)
 - Under [Area](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/area.md)
  - Set Origin enum to [ BottomLeft](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#location)
  - Set Size  to `[5, 0.5]`
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `Meter`

- Open the Level resource named `Level`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [Console](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#console)
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
 - Press key the `Up` and `Down` keys to send events between spaces.



![MeterScale](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/94422.gif)


Each time `Up` or `Down` is pressed, the `MeterUpdate` event is dispatched on the `HUDSpace`. The `Meter` component is listening to its space (this `HUDSpace`) for that event. So when it receives the event, the `ScaleMeter` function is invoked.

(NOTE)Notice how the meter renders over the SpriteText object in the `GameLevel`. As mentioned earlier, spaces can not interact graphically or physically (forces, collision, clipping, etc.), and this is a prime example of that behavior. 

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

 # Related Materials
 ## Manual
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md)
- [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md)
- {icon university}[[zilch_engine_documentation/zilch_editor_documentation/zilchmanual/editor/addremovecomponent/|Add/Remove Component]]

 ## Tutorial

 ## Reference
 ### Classes
- [SpriteText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spritetext.md)
- [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
- [Area](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/area.md)
- [Camera](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/camera.md)
- [Space](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md)

 ### Enums
- [Location.BottomLeft](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#location)

 ### Commands
- [ New Project](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#newproject)
- [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
- [ Add](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#add)
- [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)
- [CreateSpriteText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createspritetext)
- [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)

 ## Tasks
- T1175 

 
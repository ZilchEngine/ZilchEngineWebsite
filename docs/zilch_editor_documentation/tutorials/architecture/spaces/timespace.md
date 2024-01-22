Having already seen [spaces](../spaces.md) in a previous tutorial, we will now talk about a component that only appears on space objects: the [TimeSpace](../../../../code_reference/class_reference/timespace.md).


 #  Learning Objectives


- TimeScale
- Pausing


 #  Level Setup


- [Command](../../../zilchmanual/editor/editorcommands/commands.md) : [New Project](../../../../code_reference/command_reference.md#newproject)
 - Create a new project using the {nav icon=clone, name=Empty 2D Project} template
- [Command](../../../zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](../../../../code_reference/command_reference.md#createsprite)
- In the `Properties Window`
 - [Add Component](../../../zilchmanual/editor/addremovecomponent.md) : [RigidBody](../../../../code_reference/class_reference/rigidbody.md)
 - [Add Component](../../../zilchmanual/editor/addremovecomponent.md) : [BoxCollider](../../../../code_reference/class_reference/boxcollider.md)
 - Under [RigidBody](../../../../code_reference/class_reference/rigidbody.md)
  - Set `name=DynamicState,icon=list` to [Static](../../../../code_reference/enum_reference.md#rigidbodydynamicstate)
 - Under [Transform](../../../../code_reference/class_reference/transform.md)
  - Set Scale  to `[25,1,1]`
- [Command](../../../zilchmanual/editor/editorcommands/commands.md) : [CreateSphere](../../../../code_reference/command_reference.md#createsphere)
- In the `Properties Window`
 - Under [Transform](../../../../code_reference/class_reference/transform.md)
  - Set Translation  to `[-10,5,0]`
 - Under [RigidBody](../../../../code_reference/class_reference/rigidbody.md)
  - Set Velocity  to `[10,0,0]`


 #  What is the TimeSpace?


The [TimeSpace](../../../../code_reference/class_reference/timespace.md) component allows for developer control over time in the space it is attached to. Time in that space can be slowed or even stopped. Let's see what the demo looks like right now to get a frame of reference.

  - [Command](../../../zilchmanual/editor/editorcommands/commands.md) : [PlayGame](../../../../code_reference/command_reference.md#playgame)



![control](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/94788.gif)


- [Command](../../../zilchmanual/editor/editorcommands/commands.md) : [StopGame](../../../../code_reference/command_reference.md#stopgame)

The ball falls, bounces, and rolls at a normal pace for the values it was initialized with.


 ##  TimeScale


A common dramatic effect is to slow down time during some in-game event. Slow motion effects are typically implemented via the [TimeScale](../../../../code_reference/class_reference/timespace.md#timescale-zilch-engine-do) property, which is a scalar for the rate at which time passes. There are also some times where running your project at a slower speed will allow you to debug issues more easily. Let's take a look at how to change TimeScale  using the UI.

(NOTE)**Space Selection**:
 The [Space](../../../../code_reference/class_reference/space.md) can be selected via the `Select` menu, by clicking in the viewport and then pressing `Shift + S`, by pressing `Ctrl + Shift + S` with any window in focus, or by using the [SelectSpace](../../../../code_reference/command_reference.md#selectspace) command.
 ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/94805.png)

- [Command](../../../zilchmanual/editor/editorcommands/commands.md) : [SelectSpace](../../../../code_reference/command_reference.md#selectspace)
- In the `Properties Window`
 - Under [TimeSpace](../../../../code_reference/class_reference/timespace.md)
  - Set TimeScale  to `0.5`
- [Command](../../../zilchmanual/editor/editorcommands/commands.md) : [PlayGame](../../../../code_reference/command_reference.md#playgame)



![halfspeed](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/94807.gif)


*Demo running half speed with `0.5` TimeScale*


- [Command](../../../zilchmanual/editor/editorcommands/commands.md) : [StopGame](../../../../code_reference/command_reference.md#stopgame)

Now we can see that the time scale directly affects the rate of time without affecting the framerate.

- [Command](../../../zilchmanual/editor/editorcommands/commands.md) : [SelectSpace](../../../../code_reference/command_reference.md#selectspace)
- In the `Properties Window`
 - Under [TimeSpace](../../../../code_reference/class_reference/timespace.md)
  - Set TimeScale  to `1.0`


 ##  Adjusting TimeScale In Script


- [Command](../../../zilchmanual/editor/editorcommands/commands.md) : [Add Resource](../../../zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `TimeControl`
- Update the `TimeControl` script to the following:

```TS:"TimeControl"
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

- [Select](../../../zilchmanual/editor/editorcommands/selectobject.md) : LevelSettings object
- In the `Properties Window`
 - [Add Component](../../../zilchmanual/editor/addremovecomponent.md) : `TimeControl`
- [Command](../../../zilchmanual/editor/editorcommands/commands.md) : [Console](../../../../code_reference/command_reference.md#console)
- [Command](../../../zilchmanual/editor/editorcommands/commands.md) : [PlayGame](../../../../code_reference/command_reference.md#playgame)
 - Adjust the time scale using the `up` and `down` keys



![controlled](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/94790.gif)


*TimeScale  being adjusted up and down*


- [Command](../../../zilchmanual/editor/editorcommands/commands.md) : [StopGame](../../../../code_reference/command_reference.md#stopgame)

Above we can see the demo progressing slower and then faster as the [TimeScale](../../../../code_reference/class_reference/timespace.md#timescale-zilch-engine-do) is adjusted using the keyboard.


 #  Pausing


- Add the following property to the `TimeControl` script:
```TS:PauseKey Property
  [Property]
  var PauseKey : Keys = Keys.Space;
```

- Add the following function to the `TimeControl` script:
```TS:TogglePause
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
```TS:OnLogicUpdate Extension
    if(Zilch.Keyboard.KeyIsPressed(this.PauseKey))
      this.TogglePause();
```

- [Command](../../../zilchmanual/editor/editorcommands/commands.md) : [PlayGame](../../../../code_reference/command_reference.md#playgame)
 - Press `Space` to pause the game and then press `Space` again to attempt to unpause the game



![stopped](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/94809.gif)


- [Command](../../../zilchmanual/editor/editorcommands/commands.md) : [StopGame](../../../../code_reference/command_reference.md#stopgame)

You probably noticed that the game will not unpause. This is because when the [TimeSpace](../../../../code_reference/class_reference/timespace.md) is paused, [Keyboard](../../../../code_reference/class_reference/keyboard.md), listening for the [KeyDown](../../../../code_reference/event_reference.md#keydown) event, or to poll the keyboard input on [FrameUpdate](../../../../code_reference/event_reference.md#frameupdate).

- Update the `Initialize` function in `TimeControl` to the following:
```TS:Initialize
  function Initialize(init : CogInitializer)
  {
    Zilch.Connect(Zilch.Keyboard, Events.KeyDown, this.OnKeyDown);
  }
```

- Replace the `OnLogicUpdate` function in `TimeControl` with the following:
```TS:Initialize
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

- [Command](../../../zilchmanual/editor/editorcommands/commands.md) : [PlayGame](../../../../code_reference/command_reference.md#playgame)
 - Press `Space` to pause the game and then press `Space` again to attempt to unpause the game



![pausing](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/94811.gif)


*Pausing with and unpausing in reaction to the [KeyDown](../../../../code_reference/event_reference.md#keydown) event*


Now we can see the game being paused and unpaused successfully.

- [Command](../../../zilchmanual/editor/editorcommands/commands.md) : [StopGame](../../../../code_reference/command_reference.md#stopgame)


 #  Related Materials
 ##  Manual
- [LauncherNewProject](../../../zilchmanual/editor/editorcommands/launchernewproject.md)
- [commands](../../../zilchmanual/editor/editorcommands/commands.md)
- [selectobject](../../../zilchmanual/editor/editorcommands/selectobject.md)
- [addremovecomponent](../../../zilchmanual/editor/addremovecomponent.md)
- [resourceadding](../../../zilchmanual/editor/editorcommands/resourceadding.md)

 ##  Reference
 ###  Commands
- [CreateSprite](../../../../code_reference/command_reference.md#createsprite)
- [CreateSphere](../../../../code_reference/command_reference.md#createsphere)
- [SelectSpace](../../../../code_reference/command_reference.md#selectspace)
- [Console](../../../../code_reference/command_reference.md#console)
- [PlayGame](../../../../code_reference/command_reference.md#playgame)
- [StopGame](../../../../code_reference/command_reference.md#stopgame)

 ###  Classes
- [transform](../../../../code_reference/class_reference/transform.md)
- [timespace](../../../../code_reference/class_reference/timespace.md)
- [rigidbody](../../../../code_reference/class_reference/rigidbody.md)
- [boxcollider](../../../../code_reference/class_reference/boxcollider.md)
- [keyboard](../../../../code_reference/class_reference/keyboard.md)

 ###  Events
- [LogicUpdate](../../../../code_reference/event_reference.md#logicupdate)
- [FrameUpdate](../../../../code_reference/event_reference.md#frameupdate)
- [KeyDown](../../../../code_reference/event_reference.md#keydown)

 ##  Development Tasks
- {T1178} 

 
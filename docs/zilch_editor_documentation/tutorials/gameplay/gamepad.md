IMPORTANT: This lesson requires a gamepad such as an Xbox controller.

 # Learning Objectives
- Gamepad input detection
- Detection of gamepad device connection and removal

Gamepads such as Xbox controllers are common input devices for games on both consoles and PC. While not all gamepads are the same, many gamepads follow a common input scheme that matches the interface of the Zilch Engine [Gamepad](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepad.md) class.

 # Level Setup
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ New Project](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#newproject)
 - Create a new project using the {nav icon=clone, name=Empty 2D Project} template
- Plug in a gamepad
- In the [ Market](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/using_the_market.md)
 - Download the SweptCharacter  ZilchPack
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- In the `Properties Window`
 - Rename the Sprite object to `Player`
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [BoxCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md)
 - Under [RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
  - Set DynamicState enum to `Kinematic`
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `SweptController`
 - Under `SweptController`
  - Set Gravity  to `0`
  - Set WorldUp  to `[0,0,1]`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `GamepadHandle`
- In the `Properties Window`
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `GamepadHandle`

NOTE: An interactive controller diagram with input feedback is included in many of the images on this page. The purpose of the diagram is to communicate input to the reader in sync with the behavior. The scripts and resources for the diagram will not be covered in this lesson.

 # Aquiring a Reference to a Gamepad
The first step in detecting input on a gamepad device is to detect the gamepad itself.

- Update `GamepadHandle` to the following:
```name=GamepadHandle Detecting the Gamepad, lang=csharp
class GamepadHandle : NadaComponent
{
  [Property]
  var GamepadId : Integer = 0;
  
  var Gamepad : Gamepad;
  
  function Initialize(init : CogInitializer)
  {
    this.Gamepad = Zilch.Gamepads.GetGamePad(this.GamepadId);
    Console.WriteLine("Gamepad: `this.Gamepad` Is Active: `this.Gamepad.IsActive`");
  }
}
```

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Console](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#console)
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)

```name=Console Output
---------------- Begin Game ----------------
Gamepad: Gamepad (060A7748) Is Active: true
Level 'Level' was loaded.
Loaded level 0.00s
----------------  End Game  ----------------
```

You should see this same console output but with a different ID for the [Gamepad](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepad.md) object. Detecting may seem simple, but there's more to it than this. We'll take another look at it near the end of the lesson.

 # Buttons
Now that we know how to grab a reference to a gamepad, we can start detecting input. The first type of input we will examine is button input.

 ## Button Events
Button events are very similar to keyboard events. `ButtonDown` and `ButtonUp` are both dispatched on the [Gamepad](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepad.md) object in reaction to the input state of a button changing. 

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `PauseManager`
- Update `PauseManager` to the following:
```name=PauseManager, lang=csharp
class PauseManager : NadaComponent
{
  [Dependency] var TimeSpace : TimeSpace;
  
  [Property]
  var PauseButton : Buttons = Buttons.Start;
  
  function Initialize(init : CogInitializer)
  {
    for(var i = 0; i < Zilch.Gamepads.MaxGamepadCount; ++i)
    {
      var gamepad = Zilch.Gamepads.GetGamePad(i);
      Zilch.Connect(gamepad, Events.ButtonDown, this.OnButtonDown);
    }
  }

  function OnButtonDown(event : GamepadEvent)
  {
    if(event.Button == this.PauseButton)
    {
      Console.WriteLine("Pause Button Pressed");
      this.Space.TimeSpace.Paused = !this.Space.TimeSpace.Paused;
    }
  }
}
```

Similar to how we retrieved the `gamepad` object in `GamepadHandle`, the `for` loop in the code block above retrieves all the gamepads. It then connects to the `ButtonDown` event on each gamepad. Just as we connect to the `Keyboard` for `KeyboardEvents`, we connect to the `gamepad` for `GamepadEvents`. This makes use of the fact that a **gamepad object will always exist whether the gamepad is actually connected or not**. This behavior allows us to never lose the connection, no matter what happens to the gamepad. In the response function we simply invert the value of `this.Space.TimeSpace.Paused` to toggle pausing the Space.


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [SelectSpace](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#selectspace)
- [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `PauseManager`

Since the player doesn't move yet, let's create an object that will allow us to test the functionality of our `PauseManager`.
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSphere](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsphere)
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : LevelSettings object
 - Under [GridDraw](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/griddraw.md)
  - Set DrawInGame checkBox to `True`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)

- Quickly press `Start` a few times to pause and unpause the game



![PausingOnStart](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/96091.gif)


*Game pausing and unpausing in reaction to `Start` being pressed*


In a real game, our pause manager might also create a pause menu, but for the purposes of our gamepad lesson, the example as is proves the point.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

 # Sticks
Buttons are fine for most input, but some input needs to be directional. While the directional pad buttons on a gamepad can be used to determine one of eight cardinal directions, a joystick allows for full range directional input.

Let's use the left stick to get our Player object moving.
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `SweptGamepadInput2D`

- Update `SweptGamepadInput2D` to the following:
```name=SweptGamepadInput2D, lang=csharp
class SweptGamepadInput2D : NadaComponent
{
  [Dependency] var SweptController : SweptController;
  
  [Property]
  var GamepadId : Integer = 0;
  
  var Gamepad : Gamepad;
  
  [Property]
  var DeadZoneRadius : Real = 0.1;
  
  function Initialize(init : CogInitializer)
  {
    this.Gamepad = Zilch.Gamepads.GetGamePad(this.GamepadId);
    Zilch.Connect(this.Space, Events.LogicUpdate, this.OnLogicUpdate);
  }

  function OnLogicUpdate(event : UpdateEvent)
  {
    var movement = Real2();
    
    var leftstick = this.Gamepad.LeftStick;
    if(Math.Length(leftstick) > this.DeadZoneRadius)
      movement = leftstick;
    
    this.SweptController.Update(Real3(movement, 0), event.Dt);
  }
}
```

In the above code block we get the [Real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md) value of [Gamepad.LeftStick](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepad.md#leftstick-zilch-engine-do) and pass it to the `Update` function of the `SweptController` component. We also check the length of the stick's input vector and make sure it is longer than the `DeadZoneRadius`. This is to ensure that there is a neutral state for stick input, even if the stick is slightly loose.

- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Player object
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `SweptGamepadInput2D`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
- Use the left stick to move the player



![LeftStickMovement](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/96110.gif)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

 # Triggers & Rumble
The final type of input on a gamepad are the triggers. [Left Trigger](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepad.md#lefttrigger-zilch-engine) and [RightTrigger](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepad.md#righttrigger-zilch-engine) each contain a value between `0.0` and `1.0` which represents the amount the trigger is depressed. We are going to use triggers as input for gamepad vibration, which is a common form of game feedback.

- Add the following to the `OnLogicUpdate` function in the `SweptGamepadInput2D` class:
```name=Vibration on Trigger Input
this.Gamepad.Vibrate(event.Dt, this.Gamepad.LeftTrigger, this.Gamepad.RightTrigger);
```

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
- Press the gamepad triggers to test the vibration code



![Rumble](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/96129.gif)


We can feel the gamepad vibrating in response to the triggers being depressed. You may have noticed that the [Vibrate](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepad.md#vibrate-void) function takes two parameters called `leftSpeed` and `rightSpeed`. What you may not have realized is that most gamepads have two vibration motors inside. The left motor typically has a heavier weight than the right motor. This difference in the rotating weights creates what is commonly known as the "rumble" effect. You can test this by pulling the triggers one at a time.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

 # Managing the Gamepad
Now that we have covered detecting various kinds of input, let's talk more about managing the gamepad itself, specifically considering what to do when gamepads are connected or disconnected while the game is running. Regardless of whether a gamepad is or was physically (or wirelessly) connected to the computer, the corresponding `Gamepad` object will always exist (as we mentioned earlier. This allows `Gamepad.IsActive` to be checked while the game is running regardless of the actual controller state.

Let's check if the gamepad is connected while the game is running.

- Update `GamepadHandle` to the following:
```name=GamepadHandle Detecting Gamepad at Runtime, lang=csharp
class GamepadHandle : NadaComponent
{
  [Property]
  var GamepadId : Integer = 0;
  
  var Gamepad : Gamepad;
  
  var Connected : Boolean = false;
  
  function Initialize(init : CogInitializer)
  {
    this.Gamepad = Zilch.Gamepads.GetGamePad(this.GamepadId);
    this.EvaluateGamepad();
    Zilch.Connect(this.Space, Events.FrameUpdate, this.OnFrameUpdate);
  }

  function OnFrameUpdate(event : UpdateEvent)
  {
    this.EvaluateGamepad();
  }
  
  function EvaluateGamepad()
  {
    Console.WriteLine("Connected: `this.Connected`, Active: `this.Gamepad.IsActive`");
    if(!this.Connected && this.Gamepad.IsActive)
    {
      this.Connected = true;
      Console.WriteLine("Gamepad connected");
    }
    else if(this.Connected && !this.Gamepad.IsActive)
    {
      this.Connected = false;
      Console.WriteLine("Gamepad disconnected");
    }
  }
}
```
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)

- Disconnect the gamepad from the computer
 - Give the computer a moment to detect the gamepad is unplugged
- Reconnect the gamepad to the computer
 - Give the computer a moment to detect the gamepad is plugged in
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)
- Scroll up in the ConsoleOutput 

```name=ConsoleOutput
---------------- Begin Game ----------------

Connected: true, Active: true
Connected: true, Active: true
Connected: true, Active: false
Gamepad disconnected
Connected: false, Active: false
...
Connected: false, Active: false
Connected: false, Active: true
Gamepad connected
Connected: true, Active: true
Connected: true, Active: true
...
----------------  End Game  ----------------
```

Your console output should roughly take the above form with more prints in place of the `...` depending on how quickly you ran the test. We can see that the `Gamepad.IsActive` becomes false allowing us to detect that the gamepad was disconnected, set `Connected` to `false`, and dispatch the corresponding events.

What use is this to us? So far, we simply have another Boolean, `this.Connected`, that tracks the state of `Gamepad.IsActive` from the previous frame. Before we update the value of `this.Connected` to match `Gamepad.IsActive`, if they are not already equal, then we know that the gamepad was connected or disconnected on that frame. In this way, we can detect the exact frame the gamepad disconnected or reconnected and let other parts of the game know.

- Update `GamepadHandle` to the following:
```name=GamepadHandle Sending Events, lang=csharp
class GamepadHandle : NadaComponent
{
  [Property]
  var GamepadId : Integer = 0;
  
  var Gamepad : Gamepad;
  
  var Connected : Boolean = false;
  
  function Initialize(init : CogInitializer)
  {
    this.Gamepad = Zilch.Gamepads.GetGamePad(this.GamepadId);
    this.EvaluateGamepad();
    Zilch.Connect(this.Space, Events.FrameUpdate, this.OnFrameUpdate);
  }

  function OnFrameUpdate(event : UpdateEvent)
  {
    this.EvaluateGamepad();
  }
  
  function EvaluateGamepad()
  {
    Console.WriteLine("Connected: `this.Connected`, Active: `this.Gamepad.IsActive`");
    if(!this.Connected && this.Gamepad.IsActive)
    {
      this.Connected = true;
      Console.WriteLine("Gamepad connected");
      var gamepadConnectionEvent = this.CreateGamepadConnectionEvent();
      this.Space.DispatchEvent(Events.GamepadConnected, gamepadConnectionEvent);
    }
    else if(this.Connected && !this.Gamepad.IsActive)
    {
      this.Connected = false;
      Console.WriteLine("Gamepad disconnected");
      var gamepadConnectionEvent = this.CreateGamepadConnectionEvent();
      this.Space.DispatchEvent(Events.GamepadDisconnected, gamepadConnectionEvent);
    }
  }
  
  function CreateGamepadConnectionEvent() : GamepadConnectionEvent
  {
    var gamepadEvent = GamepadConnectionEvent();
    gamepadEvent.Gamepad = this.Gamepad;
    gamepadEvent.Id = this.GamepadId;
    return gamepadEvent;
  }
  
  sends GamepadConnected : GamepadConnectionEvent;
  sends GamepadDisconnected : GamepadConnectionEvent;
}

class GamepadConnectionEvent : NadaEvent
{
  var Id : Integer;
  var Gamepad : Gamepad;
}
```

Now when a gamepad is disconnected or reconnected, `GamepadHandle` dispatches a `GamepadConnectionEvent` to the `Space` to let all objects who care know that the state of a gamepad has changed.

- Add the following to the `Initialize` function of the `PauseManager` class:
```name=PauseManager Initialize, lang=csharp
Zilch.Connect(this.Space, Events.GamepadConnected, this.OnGamepadConnected);
Zilch.Connect(this.Space, Events.GamepadDisconnected, this.OnGamepadDisconnected);
```
- Add the following to the `PauseManager` class:
```name=PauseManager Gamepad Event Callbacks, lang=csharp
function OnGamepadConnected(event : GamepadConnectionEvent)
{
  this.TimeSpace.Paused = false;
}

function OnGamepadDisconnected(event : GamepadConnectionEvent)
{
  this.TimeSpace.Paused = true;
}
```

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
 - Quickly disconnect and reconnect the gamepad



![PausingOnDC](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/96084.gif)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

Now we can see the game pausing and unpausing in reaction to the controller being disconnected and reconnected.



 # Related Materials
 ## Manual
- [Create a New 2D Project](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/launchernewproject.md)
- [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md)
- [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md)
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md)

 ## Reference
 ### Commands

- [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
- [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

- [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- [CreateSphere](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsphere)

 ### Classes
- [BoxCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md)
- [CameraViewport](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cameraviewport.md)
- [Gamepad](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepad.md)
- [GridDraw](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/griddraw.md)
- [RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
- [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md) 

 
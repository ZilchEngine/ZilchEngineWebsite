This lesson covers how to handle basic keyboard input in Zilch Engine.


 # Learning Objectives

- Checking for keyboard input

 # Level Setup
- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [New Project](../../../code_reference/command_reference.md#newproject)
 - Create a new project using the {nav icon=clone, name=Empty 2D Project} template
- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](../../zilchmanual/editor/editorcommands/createobject.md)
- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [Add Resource](../../zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `CharacterLogic`
- [Select](../../zilchmanual/editor/editorcommands/selectobject.md) : Sprite object
- In the `Properties Window`
 - Rename Sprite object to `Character`
 - [Add Component](../../zilchmanual/editor/addremovecomponent.md) : `CharacterLogic`

 # Keyboard Input

A critical part of making a game is to allow the user to interact with it. The simplest way to achieve that is to query the available hardware for input and have the simulation respond to it.

 - Update the `CharacterLogic` script to the following code block:

```TS:Keyboard Input
class CharacterLogic : NadaComponent
{
  function Initialize(init : CogInitializer)
  {
    Zilch.Connect(this.Space, Events.LogicUpdate, this.OnLogicUpdate);
  }

  function OnLogicUpdate(event : UpdateEvent)
  {
    if(Zilch.Keyboard.KeyIsPressed(Keys.Space))
    {
      this.Owner.Sprite.VertexColor = Colors.Red;
    }
  }
}
```
- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [PlayGame](../../../code_reference/command_reference.md#playgame)
 - Press key `Space`



![SimpleInput](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/89953.gif)


- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [StopGame](../../../code_reference/command_reference.md#stopgame)

Let's take a closer look inside our if statement:

| Zilch.Keyboard.KeyIsPressed(Keys.Space); |
|-----------------------------------------------|
| [Zilch](../../../code_reference/class_reference/zilch.md) | Accessing the Zilch engine class |
| [Keyboard](../../../code_reference/class_reference/keyboard.md) | Accessing Keyboard class |
| [KeyIsPressed](../../../code_reference/class_reference/keyboard.md#keyispressed-zilch-engine)(...); | Function that determines whether a given key has been pressed this frame |
| [Keys](../../../code_reference/enum_reference.md#keys) | Enumeration containing all keyboard keys |
| .Space |  The enumeration index corresponding to the `Space` key |

Here are all Keyboard functions:

| Keyboard Functions |
|-----------------------|
| [KeyIsDown](../../../code_reference/class_reference/keyboard.md#keyisdown-zilch-engine-do) | Checks whether a given key is currently down this frame |
| [KeyIsUp](../../../code_reference/class_reference/keyboard.md#keyisup-zilch-engine-docu) | Checks whether a given key is currently down this frame|
| [KeyIsPressed](../../../code_reference/class_reference/keyboard.md#keyispressed-zilch-engine) | Checks whether a given key was pressed this frame |
| [KeyIsReleased](../../../code_reference/class_reference/keyboard.md#keyisreleased-zilch-engin) | Checks whether a given key was released this frame |

(NOTE) **Enumerations** - 
An enumeration (or enum) is a data type that groups items assigning each a unique name under the enumerated list. Items can be referenced by accessing the type followed by a `.` and the name of the desired item (i.e. [Keys.Space](../../../code_reference/enum_reference.md#keys) or Colors.Red). You can read more on enumerations [here](../../zilchmanual/nada_in_zilch/enums.md).

 # Dynamic Character Controller

Let's use what we just learned to create a character controller for a simple platformer.

 ## Character Setup

- [Select](../../zilchmanual/editor/editorcommands/selectobject.md) : Character object
- In the `Properties Window`
 - [Add Component](../../zilchmanual/editor/addremovecomponent.md) : [RigidBody](../../../code_reference/class_reference/rigidbody.md)
 - [Add Component](../../zilchmanual/editor/addremovecomponent.md) : [BoxCollider](../../../code_reference/class_reference/boxcollider.md)
 - Under [RigidBody](../../../code_reference/class_reference/rigidbody.md)
  - Set RotationLocked checkBox to `true`

 ## Ground Setup

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](../../zilchmanual/editor/editorcommands/createobject.md)
- [Select](../../zilchmanual/editor/editorcommands/selectobject.md) : Sprite object
- In the `Properties Window`
 - Rename Sprite object to `Ground`
 - [Add Component](../../zilchmanual/editor/addremovecomponent.md) : [BoxCollider](../../../code_reference/class_reference/boxcollider.md)
 - Under [Transform](../../../code_reference/class_reference/transform.md)
  - Set Translation  to `0.0, -3.0, 0.0`
  - Set Scale  to `8.0, 0.0, 0.0`
 - Under [Sprite](../../../code_reference/class_reference/sprite.md) 
  - Set SpriteSource texture to `Square`
  - Set VertexColor  to Green `[R:0, G:255, B:0, A:1.00]`

 ## Movement Code

 - In the `CharacterLogic` script
  - Replace the previous `LogicUpdate` function with the following:

```TS:Movement Logic
function OnLogicUpdate(event : UpdateEvent)
{
  var speed : Real = 5.0;
  var xDir : Real = 0.0;
  
  if(Zilch.Keyboard.KeyIsDown(Keys.Right))
  {
    xDir += 1.0;
  }
  
  if(Zilch.Keyboard.KeyIsDown(Keys.Left))
  {
    xDir += -1.0;
  }
  
  this.Owner.RigidBody.Velocity = Real3(xDir * speed, this.Owner.RigidBody.Velocity.Y, 0.0);
}
```

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [PlayGame](../../../code_reference/command_reference.md#playgame)
 - Press key `Left` and `Right`



![CharacterMovement](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/89976.gif)


- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [StopGame](../../../code_reference/command_reference.md#stopgame)

 # Related Materials

 ## Manual
- [Sprites](../../zilchmanual/graphics/sprites.md)
- [RigidBody](../../zilchmanual/physics/rigidbody.md)
- [Colliders](../../zilchmanual/physics/colliders.md)
- [KeyboardInput](../../zilchmanual/gameplay/input/keyboardinput.md)
- [Enumerations](../../zilchmanual/nada_in_zilch/enums.md)
- [Create a New 2D Project](../../zilchmanual/editor/editorcommands/launchernewproject.md)
- [CreateSprite](../../zilchmanual/editor/editorcommands/createobject.md)
- [Add Resource](../../zilchmanual/editor/editorcommands/resourceadding.md)

 ## Reference
 ### Classes
- [Transform](../../../code_reference/class_reference/transform.md)
- [Sprite](../../../code_reference/class_reference/sprite.md)
- [RigidBody](../../../code_reference/class_reference/rigidbody.md)
- [Collider](../../../code_reference/class_reference/collider.md)
- [BoxCollider](../../../code_reference/class_reference/boxcollider.md)
- [keyboard](../../../code_reference/class_reference/keyboard.md)
- [Zilch](../../../code_reference/class_reference/zilch.md)

 ### Enums
- [Keys](../../../code_reference/enum_reference.md#keys)

 ### Commands

- [PlayGame](../../../code_reference/command_reference.md#playgame)
- [StopGame](../../../code_reference/command_reference.md#stopgame) 

 
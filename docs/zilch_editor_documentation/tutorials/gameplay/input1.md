This lesson covers how to handle basic keyboard input in Zilch Engine.


 # Learning Objectives

- Checking for keyboard input

 # Level Setup
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ New Project](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#newproject)
 - Create a new project using the {nav icon=clone, name=Empty 2D Project} template
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/createobject.md)
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `CharacterLogic`
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Sprite object
- In the `Properties Window`
 - Rename Sprite object to `Character`
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `CharacterLogic`

 # Keyboard Input

A critical part of making a game is to allow the user to interact with it. The simplest way to achieve that is to query the available hardware for input and have the simulation respond to it.

 - Update the `CharacterLogic` script to the following code block:

```lang=csharp, name=Keyboard Input
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
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
 - Press key `Space`



![SimpleInput](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/89953.gif)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

Let's take a closer look inside our if statement:

| Zilch.Keyboard.KeyIsPressed(Keys.Space); |
|-----------------------------------------------|
| [Zilch](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/zero.md) | Accessing the Zilch engine class |
| [Keyboard](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/keyboard.md) | Accessing Keyboard class |
| [KeyIsPressed](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/keyboard.md#keyispressed-zilch-engine)(...); | Function that determines whether a given key has been pressed this frame |
| [Keys](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#keys) | Enumeration containing all keyboard keys |
| .Space |  The enumeration index corresponding to the `Space` key |

Here are all Keyboard functions:

| Keyboard Functions |
|-----------------------|
| [KeyIsDown](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/keyboard.md#keyisdown-zilch-engine-do) | Checks whether a given key is currently down this frame |
| [KeyIsUp](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/keyboard.md#keyisup-zilch-engine-docu) | Checks whether a given key is currently down this frame|
| [KeyIsPressed](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/keyboard.md#keyispressed-zilch-engine) | Checks whether a given key was pressed this frame |
| [KeyIsReleased](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/keyboard.md#keyisreleased-zilch-engin) | Checks whether a given key was released this frame |

(NOTE) **Enumerations** - 
An enumeration (or enum) is a data type that groups items assigning each a unique name under the enumerated list. Items can be referenced by accessing the type followed by a `.` and the name of the desired item (i.e. [Keys.Space](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#keys) or Colors.Red). You can read more on enumerations [ here ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/nada_in_zero/enums.md).

 # Dynamic Character Controller

Let's use what we just learned to create a character controller for a simple platformer.

 ## Character Setup

- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Character object
- In the `Properties Window`
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [BoxCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md)
 - Under [RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
  - Set RotationLocked checkBox to `true`

 ## Ground Setup

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/createobject.md)
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Sprite object
- In the `Properties Window`
 - Rename Sprite object to `Ground`
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [BoxCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md)
 - Under [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Translation  to `0.0, -3.0, 0.0`
  - Set Scale  to `8.0, 0.0, 0.0`
 - Under [Sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md) 
  - Set SpriteSource texture to `Square`
  - Set VertexColor  to Green `[R:0, G:255, B:0, A:1.00]`

 ## Movement Code

 - In the `CharacterLogic` script
  - Replace the previous `LogicUpdate` function with the following:

```lang=csharp, name=Movement Logic
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

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
 - Press key `Left` and `Right`



![CharacterMovement](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/89976.gif)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

 # Related Materials

 ## Manual
- [Sprites](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/graphics/sprites.md)
- [RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/rigidbody.md)
- [Colliders](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/colliders.md)
- [KeyboardInput](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/gameplay/input/keyboardinput.md)
- [ Enumerations ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/nada_in_zero/enums.md)
- [Create a New 2D Project](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/launchernewproject.md)
- [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/createobject.md)
- [Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)

 ## Reference
 ### Classes
- [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
- [Sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md)
- [RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
- [Collider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md)
- [BoxCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md)
- [keyboard](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/keyboard.md)
- [Zilch](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/zilch.md)

 ### Enums
- [Keys](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#keys)

 ### Commands

- [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
- [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame) 

 
This lesson covers the basics of [ Components ](../../zilchmanual/architecture/components/components.md) and demonstrates basic usage of the [ Collider ](../../zilchmanual/physics/colliders.md), [ RigidBody ](../../zilchmanual/physics/rigidbody.md), [ Sprite ](../../zilchmanual/graphics/sprites/sprite.md), and [ SpriteText ](../../zilchmanual/graphics/sprites/spritetext.md) components.


 #  Learning Objectives


- Component basics
- Common built-in components


 #  Component Overview


Each component will typically have its own set of properties that can be modified to customize that component's behavior. In this tutorial we're going to show you some of the most commonly used components.


 #  Level Setup


- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [ New Project](../../../code_reference/command_reference.md#newproject)
 - Create a new project using the {nav icon=clone, name=Empty 2D Project} template


 ##  Create a Transform Object


- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [ CreateTransform](../../../code_reference/command_reference.md#createtransform)



![micreatetransform](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/113.png)


*Creating a Transform object via the `Create Menu`*


Notice that the Trasnform object object can be found in the `Objects Window`:


![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46956.png)


*The Transform object listed in the `Objects Window`*


This provides a very basic object that has a defined position, scale and rotation. Let's go ahead and make our object more interesting by adding a [Sprite](../../../code_reference/class_reference/sprite.md) component.


 #  Adding a Component


- In the `Properties Window`
 - Click  the `Add Component` button
 - Type key : `Sprite`
 - Click  on Sprite button to add a [Sprite](../../../code_reference/class_reference/sprite.md) component.



![AddSprite](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46957.gif)


*Adding the [Sprite](../../../code_reference/class_reference/sprite.md) component to the Transform object*


You can also add components to a selected object by using the hotkey `Ctrl + M`.

NOTE:
  Some components may require another component to be present on an object before they can be added: this is called a **dependency**. Many of the components in Zilch (Including Sprite, for example) depend on the [Transform](../../../code_reference/class_reference/transform.md) component. If one or more dependencies aren't satisfied, Zilch will notify you when you attempt to add that component.
  ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46145.png)


 #  Sprite Component


The [Sprite](../../../code_reference/class_reference/sprite.md) component provides a 2D visual representation of an object. Let's take a look at some of its most commonly used properties:



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46960.png)


*The `Properties Window` showing the Sprite component*


| Common Sprite Properties |
|---|
| Visible checkBox | Whether the object can be seen |
| VertexColor  | The base color of the Sprite |
| SpriteSource enum | The image file that this Sprite displays |


 #  Making a Copy of an Object


- [ Select](../../zilchmanual/editor/editorcommands/selectobject.md) : Transform object
 - Press key `Ctrl + C` to copy it 
 - Press key `Ctrl + V` to paste a new copy

Notice how there are two objects in the `Objects Window`, but we only see one in the `Level Window`. That's because they are overlapping; we can fix this by moving one of the objects.


 # Altering Component Properties



- In the `Properties Window`
 - Rename Transform object to `RedBall`
 - Under [Transform](../../../code_reference/class_reference/transform.md)
  - Set Translation  to `[0, 5, 0]`
    ![Move](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46961.gif)
 - Under [Sprite](../../../code_reference/class_reference/sprite.md)
  - Set SpriteSource enum to `CircleBordered`
    ![SpriteSourceChange](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46962.gif)
  - Set VertexColor  to `[R:255, G:0, B:0, A:1.00]`
    ![ColorChange](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46963.gif)

NOTE:
  Color is defined by four values; Red, Green, Blue, and Alpha, in that order: RGBA. The first three refer to the amount of each respective color, while Alpha denotes the opacity of the color. Color values in the property grid range from 0 to 255, while alpha ranges from 0.00 (fully transparent) to 1.00 (fully opaque).

| Color References |
|---|
| Red     | `[R:255, G:0  , B:0  , A:1.00]` | ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46257.png) |
| Green   | `[R:0  , G:255, B:0  , A:1.00]` | ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46258.png) |
| Blue    | `[R:0  , G:0  , B:255, A:1.00]` | ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46265.png) |
| Yellow  | `[R:255, G:255, B:0  , A:1.00]` | ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46262.png) |
| Magenta | `[R:255, G:0  , B:255, A:1.00]` | ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46294.png) |
| Cyan    | `[R:0  , G:255, B:255, A:1.00]` | ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46276.png) |
| Orange  | `[R:255, G:128, B:0  , A:1.00]` | ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46266.png) |
| Pink    | `[R:255, G:0  , B:128, A:1.00]` | ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46264.png) |
| Purple  | `[R:128, G:0  , B:255, A:1.00]` | ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46275.png) |
| Teal    | `[R:0  , G:255, B:128, A:1.00]` | ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46293.png) |
| White   | `[R:255, G:255, B:255, A:1.00]` | ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46260.png) |
| Black   | `[R:0  , G:0  , B:0  , A:1.00]` | ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46261.png) |

- [ Select](../../zilchmanual/editor/editorcommands/selectobject.md) : the other Transform object object
- Rename it to `Ground`
- In the `Properties Window`
 - Under [Transform](../../../code_reference/class_reference/transform.md)
  - Set Scale  to `[5, 0, 0]`
 - Under [Sprite](../../../code_reference/class_reference/sprite.md)
  - Set VertexColor  to `[R:0, G:255, B:0, A:1.00]`

Your level should look like this:


![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46281.png)



 #  RigidBody Component


The [RigidBody](../../../code_reference/class_reference/rigidbody.md) component gives an object physics properties, like mass and velocity. Let's take a look at it:



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46964.png)


*The `Properties Window` showing the RigidBody component*


| Common RigidBody Properties |
|---|
| Velocity  | The current velocity being applied to the object. Changing this property in the editor sets the object's initial velocity |
| AngularVelocity  | Angular velocity is an object's current spin. Changing this property in the editor sets the object's initial spin (only around the Z axis for 2D objects) |
| RotationLocked checkBox | Prevents the physics system from rotating the object. (The object can still be rotated by modifying its Transform's Rotation  property.) Commonly used for player characters |

- [ Select](../../zilchmanual/editor/editorcommands/selectobject.md) : RedBall object
- In the `Properties Window`
 - [ Add Component](../../zilchmanual/editor/addremovecomponent.md) : [ RigidBody](../../../code_reference/class_reference/rigidbody.md)
- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [ Save Project](../../../code_reference/command_reference.md#saveproject)
- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](../../../code_reference/command_reference.md#playgame)

The RedBall object  is now affected by gravity.



![FallingBall](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46284.gif)


*The RedBall object object falling due to gravity*


Notice that it didn't collide with the Ground object object, though. To have the RedBall object  hit the ground, we'll need to add [ colliders](../../zilchmanual/physics/colliders.md) to our objects.

- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [ StopGame](../../../code_reference/command_reference.md#stopgame)


 #  Collider Components


Colliders are used to detect when two objects occupy the same physical space, and, if so desired, prevent that. Zilch Engine offers several different types of colliders, including [ BoxCollider](../../../code_reference/class_reference/boxcollider.md), [ SphereCollider](../../../code_reference/class_reference/spherecollider.md), [ CylinderCollider](../../../code_reference/class_reference/cylindercollider.md), and [ CapsuleCollider](../../../code_reference/class_reference/capsulecollider.md); in this section, we'll demonstrate a couple of these.



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46965.png)


*The `Properties Window` showing the BoxCollider component*


| Common Collider Properties |
|---|
| Offset  | How far the collider should be offset from the object's position |
| Ghost checkBox | Allows for collision detection without resolution |
| Size  | How big the collider should be, relative to the object's scale (only available on BoxCollider) |
| Radius  | How big the radius of the collider should be, relative to the object's scale (only available on SphereCollider) |

- [ Select](../../zilchmanual/editor/editorcommands/selectobject.md) : RedBall object
- In the `Properties Window`
 - [ Add Component](../../zilchmanual/editor/addremovecomponent.md) : [ SphereCollider](../../../code_reference/class_reference/spherecollider.md)

Let's also add a collider to our Ground object object.

- [ Select](../../zilchmanual/editor/editorcommands/selectobject.md) : Ground object
- In the `Properties Window`
 - [ Add Component](../../zilchmanual/editor/addremovecomponent.md) : [ BoxCollider](../../../code_reference/class_reference/boxcollider.md)

- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [ Save Project](../../../code_reference/command_reference.md#saveproject)
- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](../../../code_reference/command_reference.md#playgame)



![FallingBallHit](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46288.gif)


*The RedBall object object landing on the Ground object object*


Now our RedBall object is colliding with the Ground object as intended.

- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [ StopGame](../../../code_reference/command_reference.md#stopgame)


 #  SpriteText Component


Similar to [Sprite](../../../code_reference/class_reference/sprite.md), the [SpriteText](../../../code_reference/class_reference/spritetext.md)  component allows us to draw 2D text onto the screen. Let's take a look at its properties:



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46966.png)


*The `Properties Window` showing the SpriteText component*


| Common SpriteText Properties |
|---|
| Visible checkBox | Whether the text can be seen |
| VertexColor  | The color of the text |
| Font enum | Which Font resource resource to use |
| FontSize  | How big the text should be |
| Text  | The actual text to be displayed |

To finish up, the project let's add a Title object.

- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [CreateSpriteText](../../../code_reference/command_reference.md#createspritetext)
- Rename SpriteText object to `Title`
- In the `Properties Window`
 - Under [Transform](../../../code_reference/class_reference/transform.md)
  - Set Translation  to `[0, 7, 0]`
 - [ Add Component](../../zilchmanual/editor/addremovecomponent.md) : [ SpriteText](../../../code_reference/class_reference/spritetext.md)
 - Under [SpriteText](../../../code_reference/class_reference/spritetext.md)
  - Set FontSize  to `100`
  - Set Text  to `Hello World!`, or your preferred title

Let's take a look at our final result:

- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](../../../code_reference/command_reference.md#playgame)



![FallingBallFinal](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46291.gif)


*The RedBall object falls and lands on the Ground object while the Title object says hello*


- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [ StopGame](../../../code_reference/command_reference.md#stopgame)

 #  Related Materials
 ##  Manual
- [components](../../zilchmanual/architecture/components/components.md)
- [colliders](../../zilchmanual/physics/colliders.md)
- [rigidbody](../../zilchmanual/physics/rigidbody.md)
- [sprites](../../zilchmanual/graphics/sprites.md)
- [spritetext](../../zilchmanual/graphics/sprites/spritetext.md)
- [editorcommands](../../zilchmanual/editor/editorcommands.md)
- [selectobject](../../zilchmanual/editor/editorcommands/selectobject.md)
- [addremovecomponent](../../zilchmanual/editor/addremovecomponent.md)
- [gameobjectsconcept](../../zilchmanual/architecture/cogs/gameobjectsconcept.md)

 ##  Code Reference
 ###  Commands
- [ NewProject](../../../code_reference/command_reference.md#newproject)
- [ CreateTransform](../../../code_reference/command_reference.md#createtransform)
- [ SaveProject](../../../code_reference/command_reference.md#saveproject)
- [ PlayGame](../../../code_reference/command_reference.md#playgame)
- [ StopGame](../../../code_reference/command_reference.md#stopgame)
- [ CreateSpriteText](../../../code_reference/command_reference.md#createspritetext)

 ###  Classes
- [Sprite](../../../code_reference/class_reference/sprite.md)
- [transform](../../../code_reference/class_reference/transform.md)
- [rigidbody](../../../code_reference/class_reference/rigidbody.md)
- [collider](../../../code_reference/class_reference/collider.md)
- [boxcollider](../../../code_reference/class_reference/boxcollider.md)
- [spherecollider](../../../code_reference/class_reference/spherecollider.md)
- [cylindercollider](../../../code_reference/class_reference/cylindercollider.md)
- [capsulecollider](../../../code_reference/class_reference/capsulecollider.md)
- [SpriteText](../../../code_reference/class_reference/spritetext.md) 

 
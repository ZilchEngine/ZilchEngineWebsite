This lesson covers the basics of [ Components ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/architecture/components/components.md) and demonstrates basic usage of the [ Collider ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/colliders.md), [ RigidBody ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/rigidbody.md), [ Sprite ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/graphics/sprites/sprite.md), and [ SpriteText ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/graphics/sprites/spritetext.md) components.


 #  Learning Objectives


- Component basics
- Common built-in components


 #  Component Overview


Each component will typically have its own set of properties that can be modified to customize that component's behavior. In this tutorial we're going to show you some of the most commonly used components.


 #  Level Setup


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ New Project](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#newproject)
 - Create a new project using the {nav icon=clone, name=Empty 2D Project} template


 ##  Create a Transform Object


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ CreateTransform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createtransform)



![micreatetransform](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/113.png)


*Creating a Transform object via the `Create Menu`*


Notice that the Trasnform object object can be found in the `Objects Window`:


![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46956.png)


*The Transform object listed in the `Objects Window`*


This provides a very basic object that has a defined position, scale and rotation. Let's go ahead and make our object more interesting by adding a [Sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md) component.


 #  Adding a Component


- In the `Properties Window`
 - Click  the `Add Component` button
 - Type key : `Sprite`
 - Click  on Sprite button to add a [Sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md) component.



![AddSprite](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46957.gif)


*Adding the [Sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md) component to the Transform object*


You can also add components to a selected object by using the hotkey `Ctrl + M`.

NOTE:
  Some components may require another component to be present on an object before they can be added: this is called a **dependency**. Many of the components in Zilch (Including Sprite, for example) depend on the [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md) component. If one or more dependencies aren't satisfied, Zilch will notify you when you attempt to add that component.
  ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46145.png)


 #  Sprite Component


The [Sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md) component provides a 2D visual representation of an object. Let's take a look at some of its most commonly used properties:



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46960.png)


*The `Properties Window` showing the Sprite component*


| Common Sprite Properties |
|---|
| Visible checkBox | Whether the object can be seen |
| VertexColor  | The base color of the Sprite |
| SpriteSource enum | The image file that this Sprite displays |


 #  Making a Copy of an Object


- [ Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Transform object
 - Press key `Ctrl + C` to copy it 
 - Press key `Ctrl + V` to paste a new copy

Notice how there are two objects in the `Objects Window`, but we only see one in the `Level Window`. That's because they are overlapping; we can fix this by moving one of the objects.


 # Altering Component Properties



- In the `Properties Window`
 - Rename Transform object to `RedBall`
 - Under [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Translation  to `[0, 5, 0]`
    ![Move](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46961.gif)
 - Under [Sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md)
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

- [ Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : the other Transform object object
- Rename it to `Ground`
- In the `Properties Window`
 - Under [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Scale  to `[5, 0, 0]`
 - Under [Sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md)
  - Set VertexColor  to `[R:0, G:255, B:0, A:1.00]`

Your level should look like this:


![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46281.png)



 #  RigidBody Component


The [RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md) component gives an object physics properties, like mass and velocity. Let's take a look at it:



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46964.png)


*The `Properties Window` showing the RigidBody component*


| Common RigidBody Properties |
|---|
| Velocity  | The current velocity being applied to the object. Changing this property in the editor sets the object's initial velocity |
| AngularVelocity  | Angular velocity is an object's current spin. Changing this property in the editor sets the object's initial spin (only around the Z axis for 2D objects) |
| RotationLocked checkBox | Prevents the physics system from rotating the object. (The object can still be rotated by modifying its Transform's Rotation  property.) Commonly used for player characters |

- [ Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : RedBall object
- In the `Properties Window`
 - [ Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [ RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Save Project](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#saveproject)
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)

The RedBall object  is now affected by gravity.



![FallingBall](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46284.gif)


*The RedBall object object falling due to gravity*


Notice that it didn't collide with the Ground object object, though. To have the RedBall object  hit the ground, we'll need to add [ colliders](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/colliders.md) to our objects.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)


 #  Collider Components


Colliders are used to detect when two objects occupy the same physical space, and, if so desired, prevent that. Zilch Engine offers several different types of colliders, including [ BoxCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md), [ SphereCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spherecollider.md), [ CylinderCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cylindercollider.md), and [ CapsuleCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/capsulecollider.md); in this section, we'll demonstrate a couple of these.



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46965.png)


*The `Properties Window` showing the BoxCollider component*


| Common Collider Properties |
|---|
| Offset  | How far the collider should be offset from the object's position |
| Ghost checkBox | Allows for collision detection without resolution |
| Size  | How big the collider should be, relative to the object's scale (only available on BoxCollider) |
| Radius  | How big the radius of the collider should be, relative to the object's scale (only available on SphereCollider) |

- [ Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : RedBall object
- In the `Properties Window`
 - [ Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [ SphereCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spherecollider.md)

Let's also add a collider to our Ground object object.

- [ Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Ground object
- In the `Properties Window`
 - [ Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [ BoxCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md)

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Save Project](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#saveproject)
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![FallingBallHit](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46288.gif)


*The RedBall object object landing on the Ground object object*


Now our RedBall object is colliding with the Ground object as intended.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)


 #  SpriteText Component


Similar to [Sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md), the [SpriteText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spritetext.md)  component allows us to draw 2D text onto the screen. Let's take a look at its properties:



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

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSpriteText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createspritetext)
- Rename SpriteText object to `Title`
- In the `Properties Window`
 - Under [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Translation  to `[0, 7, 0]`
 - [ Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [ SpriteText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spritetext.md)
 - Under [SpriteText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spritetext.md)
  - Set FontSize  to `100`
  - Set Text  to `Hello World!`, or your preferred title

Let's take a look at our final result:

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![FallingBallFinal](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46291.gif)


*The RedBall object falls and lands on the Ground object while the Title object says hello*


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

 #  Related Materials
 ##  Manual
- [components](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/architecture/components/components.md)
- [colliders](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/colliders.md)
- [rigidbody](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/rigidbody.md)
- [sprites](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/graphics/sprites.md)
- [spritetext](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/graphics/sprites/spritetext.md)
- [editorcommands](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands.md)
- [selectobject](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md)
- [addremovecomponent](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md)
- [gameobjectsconcept](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/architecture/cogs/gameobjectsconcept.md)

 ##  Code Reference
 ###  Commands
- [ NewProject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#newproject)
- [ CreateTransform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createtransform)
- [ SaveProject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#saveproject)
- [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
- [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)
- [ CreateSpriteText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createspritetext)

 ###  Classes
- [Sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md)
- [transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
- [rigidbody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
- [collider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md)
- [boxcollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md)
- [spherecollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spherecollider.md)
- [cylindercollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cylindercollider.md)
- [capsulecollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/capsulecollider.md)
- [SpriteText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spritetext.md) 

 
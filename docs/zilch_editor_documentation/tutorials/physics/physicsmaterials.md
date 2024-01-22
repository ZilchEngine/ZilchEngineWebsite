This lecture covers the basic usage of [PhysicsMaterials](../../zilchmanual/physics/physicsmaterial.md) and the [MassOverride](../../../code_reference/class_reference/massoverride.md) component.

 # Learning Objectives

- Creating and applying [PhysicsMaterials](../../zilchmanual/physics/physicsmaterial.md)
- Basic physics concepts (Mass, Volume, Density, Restitution and Friction)
- Using the [MassOverride](../../../code_reference/class_reference/massoverride.md) component

 # Level Setup

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [New Project](../../../code_reference/command_reference.md#newproject)
 - Create a new project using the {nav icon=clone, name=Empty 2D Project} template
- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](../../../code_reference/command_reference.md#createsprite)
- [Select](../../zilchmanual/editor/editorcommands/selectobject.md) : Sprite object
- In the `Properties Window`
 - Rename Sprite object to `RedSquare`
 - Under [Transform](../../../code_reference/class_reference/transform.md)
  - Set Translation  to `[-3, 0, 0]`
 - Under [Sprite](../../../code_reference/class_reference/sprite.md)
  - Set VertexColor  to `Red: [R:255, G:0, B:0, A:1.00]`
 - [Add Component](../../zilchmanual/editor/addremovecomponent.md) : [RigidBody](../../../code_reference/class_reference/rigidbody.md)
 - Under [RigidBody](../../../code_reference/class_reference/rigidbody.md)
  - Set Velocity  to `[4, 0, 0]`
 - [Add Component](../../zilchmanual/editor/addremovecomponent.md) : [BoxCollider](../../../code_reference/class_reference/boxcollider.md)
- Duplicate the RedSquare object object
- In the `Properties Window`
 - Rename it to `BlueSquare`
 - Under [Transform](../../../code_reference/class_reference/transform.md)
  - Set Translation  to `[3, 0, 0]`
 - Under [Sprite](../../../code_reference/class_reference/sprite.md)
  - Set VertexColor  to `Blue: [R:0, G:0, B:255, A:1.00]`
 - Under [RigidBody](../../../code_reference/class_reference/rigidbody.md)
  - Set Velocity  to `[-4, 0, 0]`
- [Select](../../zilchmanual/editor/editorcommands/selectobject.md) : LevelSettings object
- In the `Properties Window`
 - Under [GravityEffect](../../../code_reference/class_reference/gravityeffect.md)
  - Set Active checkBox to `false`
 - Under [DragEffect](../../../code_reference/class_reference/drageffect.md)
  - Set Active checkBox to `false`
- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [PlayGame](../../../code_reference/command_reference.md#playgame)



![CollidingSquares](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46602.gif)


- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [StopGame](../../../code_reference/command_reference.md#stopgame)

 #  Mass

In Zilch Engine, any object with a [RigidBody](../../../code_reference/class_reference/rigidbody.md) is automatically assigned mass. An object's mass represents its weight and is determined by its **Volume** and **Density** (`M = D * V`). **Volume** is calculated from a combination of the [Collider](../../../code_reference/class_reference/collider.md) type along with its size defining properties and the object's scale, while its **Density** is defined by the object's [PhysicsMaterial](../../zilchmanual/physics/physicsmaterial.md). By altering these properties we can manipulate how objects interact physically with each other.

NOTE: An object with [RigidBody](../../../code_reference/class_reference/rigidbody.md) but with no [Collider](../../../code_reference/class_reference/collider.md) will be assigned a mass of 1 while an object with a [Collider](../../../code_reference/class_reference/collider.md) but no [RigidBody](../../../code_reference/class_reference/rigidbody.md) can be thought of as having infinite mass.

In our constructed scenario so far we see two objects colliding with each other in a space with no gravity or drag. A quick look on each object's [RigidBody](../../../code_reference/class_reference/rigidbody.md) component shows the current Mass . Since both objects have the same physics properties (mass, restitution, velocity magnitude, etc) we conclude that the collision is symmetric and both objects apply an equal force to each other when they collide. 

 # Volume

Let's explore what happens when we give them different Volumes:

- [Select](../../zilchmanual/editor/editorcommands/selectobject.md) : RedSquare object
- In the `Properties Window`
 - Under [Transform](../../../code_reference/class_reference/transform.md)
  - Set Scale  to `[2, 2, 2]`
- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [PlayGame](../../../code_reference/command_reference.md#playgame)



![CollidingSquaresMass1](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46537.gif)


Since we've made the object bigger, its mass has also increased which we can verify by checking the [RigidBody](../../../code_reference/class_reference/rigidbody.md) on RedSquare object. We can observe that the more massive object imparts a larger force onto the smaller object than the smaller does to it.

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [StopGame](../../../code_reference/command_reference.md#stopgame)

In the next section, we'll explore tweaking an object mass by altering its density.

 # Density

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [Add Resource](../../zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a [PhysicsMaterial](../../zilchmanual/physics/physicsmaterial.md) named `Dense`



![DensePhysMat](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46545.gif)


- In the `Library Window`
 - Under PhysicsMaterial 
  - `Double-Click` Dense resource
- In the `Properties Window`
 - Set Density  to `8`



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/113355.png)


- [Select](../../zilchmanual/editor/editorcommands/selectobject.md) : RedSquare object
- In the `Properties Window`
 - Under [Transform](../../../code_reference/class_reference/transform.md)
  - Set Scale  back to `[1, 1, 1]`
 - Under [BoxCollider](../../../code_reference/class_reference/boxcollider.md)
  - Set Material resource to `Dense`



![DenseCollision](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46561.gif)


Similar to the previous case, the more massive object imparts a greater force despite both objects having the same volume. Lastly, let's look into another way of setting an object's mass.

 # MassOverride

The [MassOverride](../../../code_reference/class_reference/massoverride.md) component allows you to set an object's mass regardless of its **Volume** or **Density**. It has a dependency on [RigidBody](../../../code_reference/class_reference/rigidbody.md).



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46565.png)


| MassOverride Properties |
|------------|
| Active checkBox   | Whether this component is currently overriding the RigidBody's mass |
| Mass    | The value RigidBody's mass is being overrided by) |
| RecomputeMass   | Recalculates and sets MassOverride's mass property to the default value |

- [Select](../../zilchmanual/editor/editorcommands/selectobject.md) : RedSquare object
- In the `Properties Window`
 - [Add Component](../../zilchmanual/editor/addremovecomponent.md) : [MassOverride](../../../code_reference/class_reference/massoverride.md)
- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [PlayGame](../../../code_reference/command_reference.md#playgame)



![CollidingSquares](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46602.gif)


In adding the [MassOverride](../../../code_reference/class_reference/massoverride.md) component, we just reset the RedSquare object's mass to 1 despite it still having the Dense resource [PhysicsMaterial](../../zilchmanual/physics/physicsmaterial.md)

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [StopGame](../../../code_reference/command_reference.md#stopgame)

 # Restitution

Another useful feature of [PhysicsMaterial](../../zilchmanual/physics/physicsmaterial.md) is **Restitution**: a value that represents the object's bounciness. It is represented by a value from 0 to 1 and denotes how much of its energy is preserved after the collision (0 being no energy preserved and 1 being 100% of energy preserved). You may also set Restitution to a value greater than 1 (by right-clicking the field) to cause the object to bounce away with greater energy.

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [Add Resource](../../zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a [PhysicsMaterial](../../zilchmanual/physics/physicsmaterial.md) named `Bouncy`
- In the `Library Window`
 - Under PhysicsMaterial resource
  - `Double-Click` Bouncy resource
- In the `Property Window`
 - Set Restitution  to `1`
 - Set RestitutionImportance  to `1`

- [Add Resource](../../zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a [PhysicsMaterial](../../zilchmanual/physics/physicsmaterial.md) named `NotBouncy`
- In the `Library Window`
 - Under PhysicsMaterial resource
  - `Double-Click` the NotBouncy resource resource
- In the `Property Window`
 - Set Restitution  to `0`
 - Set RestitutionImportance  to `1`

- [Select](../../zilchmanual/editor/editorcommands/selectobject.md) : BlueSquare resource
- In the `Properties Window`
 - [Remove Component](../../zilchmanual/editor/addremovecomponent.md) : [RigidBody](../../../code_reference/class_reference/rigidbody.md)
 - Under [BoxCollider](../../../code_reference/class_reference/boxcollider.md)
  - Experiment by setting PhysicsMaterial enum to `Bouncy` and `NotBouncy`

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [PlayGame](../../../code_reference/command_reference.md#playgame)



![Bouncy](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46611.gif) ![NotBouncy](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46616.gif)


- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [StopGame](../../../code_reference/command_reference.md#stopgame)

 # Friction

**Friction** is a coefficient that represents how much energy is lost when objects slide against one another. Each [PhysicsMaterial](../../zilchmanual/physics/physicsmaterial.md) provides a friction value and their combination will determine the friction force used for the collision between the two objects. The higher the friction value, the more energy will be lost per frame except when either object has a friction value of 0, in which case no energy will be lost.

NOTE: Similar to the case with restitution, PhysicsMaterials have a FrictionImportance  property, which determines which object's Friction  value to use in a collision.

- [Select](../../zilchmanual/editor/editorcommands/selectobject.md) : LevelSettings object
- In the `Properties Window`
 - Under [GravityEffect](../../../code_reference/class_reference/gravityeffect.md)
  - Set Active to `true`

- [Add Resource](../../zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a [PhysicsMaterial](../../zilchmanual/physics/physicsmaterial.md) named `HighFriction`
- In the `Library Window`
 - Under PhysicsMaterial resource
  - `Double-Click` HighFriction resource
- In the `Property Window`
 - Set Friction  to `2`
 - Set FrictionImportance  to `1`

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](../../../code_reference/command_reference.md#createsprite)
- In the `Properties Window`
 - Rename Sprite object to `GreenSquare`
 - Under [Sprite](../../../code_reference/class_reference/sprite.md)
  - Set Sprite  to `Green: [R:0, G:255, B:0, A:1.00]`
 - Under [Transform](../../../code_reference/class_reference/transform.md) 
  - Set Translation  to `[0, -1, 0]`
  - Set Scale  to `[10, 0, 0]`
 - [Add Component](../../zilchmanual/editor/addremovecomponent.md) : [BoxCollider](../../../code_reference/class_reference/boxcollider.md) component
 - Under [BoxCollider](../../../code_reference/class_reference/boxcollider.md)
  - Set Material resource to `HighFriction`

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [PlayGame](../../../code_reference/command_reference.md#playgame)



![Friction](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46630.gif)


- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [StopGame](../../../code_reference/command_reference.md#stopgame)

 # Related Materials
 ## Manual
- [PhysicsMaterials](../../zilchmanual/physics/physicsmaterial.md)

 ## Reference
 ### Classes
- [Transform](../../../code_reference/class_reference/transform.md)
- [MassOverride](../../../code_reference/class_reference/massoverride.md)
- [Sprite](../../../code_reference/class_reference/sprite.md)
- [RigidBody](../../../code_reference/class_reference/rigidbody.md)
- [Collider](../../../code_reference/class_reference/collider.md)
- [BoxCollider](../../../code_reference/class_reference/boxcollider.md)
- [GravityEffect](../../../code_reference/class_reference/gravityeffect.md)
- [DragEffect](../../../code_reference/class_reference/drageffect.md)

 ### Commands
- [Create a New 2D Project](../../zilchmanual/editor/editorcommands/launchernewproject.md)
- [PlayGame](../../../code_reference/command_reference.md#playgame)
- [StopGame](../../../code_reference/command_reference.md#stopgame)
- [Add Component](../../zilchmanual/editor/addremovecomponent.md)
- [CreateSprite](../../../code_reference/command_reference.md#createsprite)

 ## Development Tasks
- T2562
- T141 

 
This lesson focuses on teaching the basics of physics effects and components.

 # Learning Objectives

- [GravityEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gravityeffect.md) and [DragEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/drageffect.md) components
- Apply / Ignore physics effects on objects
- Basic uses of `name=LevelSettings, icon=cog`

 # Level Setup
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ New Project](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#newproject)
 - Create a new project using the {nav icon=clone, name=Empty 2D Project} template
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![FallingSquare](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46396.gif)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

 # GravityEffect

When running the game, we can see the square object falling. As we mentioned in previous tutorials, the [RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md) component allows an object to be subjected by physics forces. However, it is **not** the one responsible for the object falling.

Let's take a look at the LevelSettings object in our level:

- In the `Objects window`
 - [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : LevelSettings object



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46967.png)


- In the `Properties window`
 - Under [GravityEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gravityeffect.md)



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46968.png)


| Common GravityEffect Properties |
|------------|
| Active checkBox    | Whether this component applies force or not |
| Strength    | The magnitude of the force applied |
| Direction   | The direction which force is applied (normalized) |
|LocalSpaceDirection checkBox | Whether the specified direction is local (true) or global (false) |

- In the `Properties window`
 - Under [GravityEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gravityeffect.md)
  - Set Active checkBox to `false`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46414.png)


Notice that the Sprite object isn't being affected by gravity anymore. That's because components that produce physics effects, when attached to the LevelSettings object object, will apply that effect to all objects within the Space.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

Let's try and move the Sprite object in other ways:

- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Sprite object object
- In the `Properties Window`
 - Under [RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
  - Set Velocity  to `[3.0, 0.0, 0.0]`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![SlowingSquare](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46429.gif)


The Sprite object appears to be moving in the desired direction and still isn't affected by gravity but it slowed down and stopped. But according to Newton's first law of motion; an object retains its movement at a constant velocity unless acted upon by an external force. So what external force caused our object to stop?

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

 # DragEffect 

Let's take a look again at the LevelSettings object:

- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : LevelSettings object
- In the `Properties Window`
 - Under [DragEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/drageffect.md)
   ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46969.png)
   - Set Active checkBox to `false`

| Common DragEffect Properties |
|------------|
| Active checkBox  | Whether this component applies force or not |
| LinearDamping    | The amount of damping applied to the object's velocity |
| AngularDamping    | The amount of damping applied to the object's angular velocity |

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![EverMovingSquare](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46484.gif)


The [DragEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/drageffect.md)  exists to simulate air resistance and other forces that would prevent your object from moving indefinitely.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

 # Adding Physics Effects to Objects

These effects can also be applied to individual objects, let's take a look:

- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Sprite object
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [GravityEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gravityeffect.md)
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [DragEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/drageffect.md)
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)




![FallingSquare](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46396.gif)


Now we get the same result we had initially, but we could tweak individual gravity and drag effects per object.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

WARNING: GravityEffect (and some other PhysicsEffects) have the LocalSpaceDirection checkBox property set to true by default. This means that, as the object rotates, the "down direction" will be constantly changing. Set LocalSpaceDirection checkBox to false to avoid this behavior.


![TumblingSquare](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46531.gif)


 # IgnoreSpaceEffects

Lastly, let's say you wanted all objects in your level to be affected by gravity except for a few. You could turn off the [GravityEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gravityeffect.md) on LevelSettings object and add a [GravityEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gravityeffect.md) component to every object that needs it but that would be a lot of work.

Alternatively, you could leave the [GravityEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gravityeffect.md) on LevelSettings object on and just add the [IgnoreSpaceEffects](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ignorespaceeffects.md) component to the objects that you don't want gravity on:



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46970.png)


NOTE: The [IgnoreSpaceEffects](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ignorespaceeffects.md) component will only stop physics effects attached to LevelSettings object or Space to affect the object; if the object has a [GravityEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gravityeffect.md) component or any other physics effects components on itself, they will not be ignored!

 #  Region

The region component can be used to apply any physics effects (Gravity, Drag, etc) to  a specific zone. It works by using a Collider (which it has a dependency on) as a trigger volume to determine whether objects are inside it and then applies the specified force effects.

- [Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- In the `Property Window`
 - Rename Sprite object to `RegionEffect`
 - Under [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)  
  - Set Scale  to `[5, 5, 5]`
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [BoxCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md)
 - Under [BoxCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md)
  - Set Ghost checkBox to `true`
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [Region](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/region.md)


NOTE: Experiment by adding the [ForceEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/forceeffect.md) , [BuoyancyEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/buoyancyeffect.md) and [WindEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/windeffect.md)

 # Related Materials

 ## Manual
- [Physics Effects & Regions](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/physicseffectsandregions.md)
- [ Colliders ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/colliders.md)
- [ RigidBody ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/rigidbody.md)

 ## Code Reference
 ### Classes
- [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
- [RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
- [BoxCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md)
- [Region](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/region.md)
- [GravityEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gravityeffect.md)
- [DragEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/drageffect.md)
- [ForceEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/forceeffect.md)
- [BuoyancyEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/buoyancyeffect.md)
- [WindEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/windeffect.md)

 ### Commands
- [Create a New 2D Project](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/launchernewproject.md)
- [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
- [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
- [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)
- [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite) 

 
This lesson focuses on covering the basics of how Archetypes work in Zilch Engine.


 # Learning Objectives

- Creating Archetypes
- Instantiating objects from Archetypes
- Uploading and modifying Archetypes
- Reverting objects and properties to match an Archetype
- Turning hierarchies into archetypes

 # Level Setup
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ New Project](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#newproject)
 - Create a new project using the {nav icon=clone, name=Empty 2D Project} template
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Sprite object
- In the `Properties Window`
 - Rename Sprite object to `RedCircle`
 - Under [ Sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md)
  - Set VertexColor  to `Red: [R:255, G:0, B:0, A:1.00]`
  - Set  SpriteSource texture to `Circle`



![ArchetypeSetup](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46908.gif)


 # Creating Archetypes

An **Archetype** in Zilch Engine (similar to blueprints, prefabs or templates in other engines) is a collection of objects in a hierarchy. Archetypes are used to quickly instantiate (create a copy of) and modify copies of objects. Let's take a closer look:

- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : RedCircle object
- In the `Properties Window`
 - In the Archetype  field
  - Type `RedCircleArchetype` then press ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46915.png) or `Enter`



![ArchetypeCreate](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46917.gif)


Now we have made an archetype out of our RedCircle object object, which we can verify by looking at the `Object Window` and the `Library Window`.



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46921.png) ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46923.png)


 # Instantiating from Archetypes

As previously mentioned, one of the major benefits of Archetypes resource is being able to quickly make copies of it.

- In the `Library Window`
 - Under Archetype 
  - `Click + Drag` the `RedCircleArchetype` into the `Level Window`



![ArchetypeInstantiate](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46925.gif)


- In the `Library Window`
 - Under Archetype 
  - `Click + Drag` the `RedCircleArchetype` to the `Level Window`
- In the `Properties Window`
 - Under [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Translation  to: `[-2, 0, 0]`

- In the `Library Window`
 - Under Archetype 
  - `Click + Drag` the `RedCircleArchetype` to the `Level Window`
- In the `Properties Window`
 - Under [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Translation  to: `[2, 0, 0]`



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46927.png)


 # Modifying Archetypes

The other useful property of Archetypes is being able to edit their definition and have the changes propagate to all instances.

- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : RedCircle object
- In the `Properties Window`
 - Under [ Sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md)
  - Set VertexColor  to `Blue: [R:0, G:0, B:255, A:1.00]`

Notice that the modified property turns orange; this means that this property has been modified from the archetype this object is associated with.



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46929.png)


We can then upload our changes to the **Archetype** to have them propagate to other objects that were instantiated from it.

- In the `Properties Window`
 - Press the ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46915.png) button



![ArchetypeUpload](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46931.gif)


Once we upload our changes, the Archetype's definition changes and all properties of instances that were not modified will update to match the new definition.

 # Reverting to Archetypes

Another benefit of Archetypes is being able to revert an instance with modified properties back to match the archetype. This can be done for all modified properties or for individual properties.

- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : RedCircle object (the left most)
- In the `Properties Window`
 - Under [ Sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md)
  - Set VertexColor  to `Green: [R:0, G:255, B:0, A:1.00]`



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46936.png)


As we have seen before, the VertexColor property turns orange to indicate that it has been modified from its Archetype. Let's say you didn't like this change and want to revert it.

- In the `Properties Window`
 - Press the ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46938.png) button



![ArchetypeRevert1](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46940.gif)


You can also revert that property individually (in case you want to retain other changes) by right-clicking the individual property and selecting the revert option.



![ArchetypeRevert2](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46942.gif)


 # Archeytpes and Hierarchies

In addition to single objects you can also turn object hierarchies into archetypes. Let's see how:

- In the `Level Window`
 - Press  `Ctrl + A`
 - Press  `Delete`

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Sprite object
- In the `Properties Window`
 - Rename Sprite object to `ParentSquare`
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [BoxCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md)
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
 - Under [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Translation  to `[0, 0, 0]`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Sprite object
- In the `Properties Window`
 - Rename Sprite object to `ChildSquare`
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [BoxCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md)
 - Under [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
    - Set Translation  to: `[1, -1, 0]`
- In the `Object Window`
 - Parent the ChildSquare object object to the ParentSquare object
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : ParentSquare object
- In the `Properties Window`
 - Set Archetype  to `Squares`



![SquaresArchetype](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/88648.gif)


You can now create multiple copies of that new hierarchy by instantiating it.



![SquaresArchetypeInstances](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/88650.gif)


Once parented, both objects behave physically as if they were a single one. Let's test that by adding the following:

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateCube](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createcube)
- In the `Properties Window`
 - [Remove Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
 - Under [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
    - Set Translation  to: `[-2, -4, 0]`
    - Set Scale  to: `[4, 1, 1]`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![SquaresCollision](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/88652.gif)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

 # Related Materials

 ## Manual
- [Create a New 2D Project](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/launchernewproject.md)
- [ COGs](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/architecture/cogs/gameobjectsconcept.md)
- [ Archetypes](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/architecture/archetypes.md)

 ## Reference
 ### Classes
- [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
- [Sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md)
- [Cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)
- [RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
- [BoxCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md)

 ### Commands
- [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
- [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)
- [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- [CreateCube](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createcube) 

 
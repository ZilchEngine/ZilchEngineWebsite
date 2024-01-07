CollisionGroups allow users to categorize colliders into different groups. CollisionTables define the relationships between those groups and the behavior of those colliders when they collide with one another.


 #  Learning Objectives


- CollisionGroups
- CollisionTables
- CollisionGroup relationships


 #  Level Setup


Before jumping into how CollisionGroups are used, we need to set up a simulation to use them in.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ New Project](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#newproject)
 - Create a new project using the {nav icon=clone, name=Empty 2D Project} template
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- In the `Properties Window`
 - Rename Sprite object to `Platform`
 - Under [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Scale  to `[10,1,1]`
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [BoxCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md)
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSphere](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsphere)
- In the `Properties Window`
 - Rename Sphere object to `DefaultSphere`
 - Under [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Translation  to `[-3,5,0]`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [Duplicate](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#dupliate)
- In the `Properties Window`
 - Rename the duplicate DefaultSphere object to `SkipResolutionSphere`
 - Under [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Translation  to `[0,5,0]`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [Duplicate](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#dupliate)
- In the `Properties Window`
 - Rename the duplicate SkipResolutionSphere object to `SkipDetectionSphere`
 - Under [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Translation  to `[3,5,0]`


 #  Collision Groups


A [CollisionGroup](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisiongroup.md) is a resource assigned to one or more colliders, usually before the game is run.



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/94461.png)


*CollisionGroup enum property on the [SphereCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spherecollider.md) component*


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a CollisionGroup resource using the Default template template and name it `SkipResolution`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a CollisionGroup resource using the Default template template and name it `SkipDetection`
- [ Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : SkipResolutionSphere object
- In the `Properties Window`
 - Under [ SphereCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spherecollider.md)
  - Set CollisionGroup enum to `SkipResolution`
- [ Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : SkipDetectionSphere object
- In the `Properties Window`
 - Under [ SphereCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spherecollider.md)
  - Set CollisionGroup enum to `SkipDetection`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![notable](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/94463.gif)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

You will notice that the behavior of the balls has not changed as of yet. This is because in order for CollisionGroups to be used, they must be included in the space's [CollisionTable](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisiontable.md).


 #  CollisionTables


A [CollisionTable](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisiontable.md) defines the relationship between CollisionGroup pairs.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
  - Create a CollisionTable resource using the Default template template and name it `GameTable`

When a [CollisionTable](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisiontable.md) is created, the `CollisionTableEditor Window` opens.



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/94465.png)


*The `CollisionTableEditor Window`*


This is the default configuration for a CollisionTable. It takes all the existing CollisionGroups and generates a permutation table of all the pairs.

- In the `CollisionTableEditor Window`
 - Set `DefaultGroup` / `SkipResolution` to `SkipResolution`
 - Set `DefaultGroup` / `SkipDetection` to `SkipDetection`



![setting_Tables](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/94835.gif)


- Close the `CollisionTableEditor Window`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![notable](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/94463.gif)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

You are probably wondering why the groups still aren't working. There is still one more step to perform for the groups to take effect: we have to tell the Space to use the CollisionTable we have created instead of the default CollisionTable.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ SelectSpace](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#selectspace)
- In the `Properties Window`
 - Under [PhysicsSpace](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md)
  - Set CollisionTable enum to `GameTable`



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/94469.png)


*Setting the CollisionTable enum property for the Space*


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![noprint](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/94471.gif)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

Now we can see the two spheres, which are set up to skip resolution and detection respectively, fall through the platform as expected. We still need to prove to ourselves, however, that the SkipResolutionSphere object is still at least detecting the collision.


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `PrintCollision`
- Update the `PrintCollision` script to the following:

```lang=csharp, name="PrintCollision"
class PrintCollision : NadaComponent
{
  function Initialize(init : CogInitializer)
  {
    Zilch.Connect(this.Owner, Events.CollisionStarted, this.OnCollisionStarted);
  }

  function OnCollisionStarted(event : CollisionEvent)
  {
    Console.WriteLine("CollisionStarted: `this.Owner`, Other: `event.OtherObject`");
  }
}
```


- [ Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : SkipResolutionSphere object
- In the `Properties Window`
 - [ Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `PrintCollision`
- [ Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : SkipDetectionSphere object
- In the `Properties Window`
 - [ Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `PrintCollision`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Console](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#console)
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![printcollision](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/94783.gif)


*CollisionGroups properly configured, and printing collision detection*


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

As can be seen by the printed message in the above image, the SkipResolutionSphere object is indeed detecting collision, whereas the SkipDetectionSphere object is not.

Collision groups and tables allow for a lot of flexibility in the usage of collision for game logic. They can also allow for significant performance improvement in games that heavily use physics.


 #  Related Materials
 ##  Manual
- [LauncherNewProject](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/launchernewproject.md)
- [commands](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md)
- [resourceadding](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
- [addremovecomponent](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md)
- [selectobject](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md)

 ##  Reference
 ###  Commands
- [ CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- [ CreateSphere](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsphere)
- [ Duplicate](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#duplicate)
- [ SelectSpace](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#selectspace)

 ###  Classes
- [spherecollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spherecollider.md)
- [transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
- [physicsspace](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md)
- [collisiongroup](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisiongroup.md)
- [collisiontable](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisiontable.md)

 ###  Events
- [ CollisionStarted](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/event_reference.md#collisionstarted)

 ###  Enums
- [ CollisionFilterCollisionFlags](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#collisionfiltercollision)

 ##  Development Task 
- {T1176} 

 
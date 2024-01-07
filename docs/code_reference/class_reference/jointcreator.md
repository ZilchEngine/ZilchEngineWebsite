 `Physics`

(NOTE) A helper class to create joints of various configurations. Each joint is configured from two points. Any other specific joint properties are calculated from these two points.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddJointLimit](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointcreator.md#addjointlimit-zilch-engin)|[ AttachToCommonParent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointcreator.md#attachtocommonparent-zer)| | |
|[ AddJointMotor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointcreator.md#addjointmotor-zilch-engin)|[ AttachToWorld](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointcreator.md#attachtoworld-zilch-engin)| | |
|[ AddJointSpring](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointcreator.md#addjointspring-zilch-engi)|[ AutoSnaps](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointcreator.md#autosnaps-zilch-engine-do)| | |
|[ Create](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointcreator.md#create-zilch-engine-docum)|[ OverrideLength](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointcreator.md#overridelength-zilch-engi)| | |
|[ CreateLocalPoints](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointcreator.md#createlocalpoints-zilch-e)|[ UseCenter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointcreator.md#usecenter-zilch-engine-do)| | |
|[ CreateWorldPoints](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointcreator.md#createworldpoints-zilch-e)| | | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointcreator.md#jointcreator-void)| | | |


 #  Properties


---  
 #  AttachToCommonParent : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Should the cog of the joint be added as a child of the common parent of the two given cogs? Useful for putting the joint in the same hierarchy so that archetypes can be created.
> ``` lang=cpp, name=Nada
> var AttachToCommonParent : Boolean


---  
 #  AttachToWorld : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Used to create a connection to a dummy object. Instead of connecting to object B, the connection will be between object A and "the world".
> ``` lang=cpp, name=Nada
> var AttachToWorld : Boolean


---  
 #  AutoSnaps : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Should the joint auto-snap when the force limit is reached?
> ``` lang=cpp, name=Nada
> var AutoSnaps : Boolean


---  
 #  OverrideLength : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Should the length of the joint be overridden or computed from the two points? Mainly used for StickJoint.
> ``` lang=cpp, name=Nada
> var OverrideLength : Boolean


---  
 #  UseCenter : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Should the center of each object be used instead of the given points?
> ``` lang=cpp, name=Nada
> var UseCenter : Boolean


---  
 #  Methods


---  
 #  AddJointLimit : [jointlimit](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointlimit.md)

> Add a JointLimit to the given joint cog.
> |Name|Type|Description|
> |---|---|---|
> |joint|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Nada
> function AddJointLimit(joint : Cog) : JointLimit
> ``` 


---  
 #  AddJointMotor : [jointmotor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointmotor.md)

> Add a JointMotor to the given joint cog.
> |Name|Type|Description|
> |---|---|---|
> |joint|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Nada
> function AddJointMotor(joint : Cog) : JointMotor
> ``` 


---  
 #  AddJointSpring : [jointspring](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointspring.md)

> Add a JointSpring to the given joint cog.
> |Name|Type|Description|
> |---|---|---|
> |joint|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Nada
> function AddJointSpring(joint : Cog) : JointSpring
> ``` 


---  
 #  Create : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Create a joint (by archetype) attached to the two given cogs.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |objectB|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |jointArchetype|[archetype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/archetype.md)| |
> ``` lang=cpp, name=Nada
> function Create(objectA : Cog, objectB : Cog, jointArchetype : Archetype) : Cog
> ``` 


---  
 #  Create : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Create a joint (by component name) attached to the two given cogs.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |objectB|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |jointName|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function Create(objectA : Cog, objectB : Cog, jointName : String) : Cog
> ``` 


---  
 #  CreateLocalPoints : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Create a joint (by archetype) attached to the two given cogs.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |objectB|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |jointArchetype|[archetype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/archetype.md)| |
> |localPointA|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |localPointB|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function CreateLocalPoints(objectA : Cog, objectB : Cog, jointArchetype : Archetype, localPointA : Real3, localPointB : Real3) : Cog
> ``` 


---  
 #  CreateLocalPoints : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Create a joint (by component name) attached to the two given cogs.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |objectB|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |jointName|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |localPointA|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |localPointB|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function CreateLocalPoints(objectA : Cog, objectB : Cog, jointName : String, localPointA : Real3, localPointB : Real3) : Cog
> ``` 


---  
 #  CreateWorldPoints : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Create a joint (by archetype) attached to the two given cogs. Both world points on the joint are set to the same world point value.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |objectB|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |jointArchetype|[archetype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/archetype.md)| |
> |bothWorldPoints|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function CreateWorldPoints(objectA : Cog, objectB : Cog, jointArchetype : Archetype, bothWorldPoints : Real3) : Cog
> ``` 


---  
 #  CreateWorldPoints : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Create a joint (by archetype) attached to the two given cogs.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |objectB|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |jointArchetype|[archetype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/archetype.md)| |
> |worldPointA|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |worldPointB|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function CreateWorldPoints(objectA : Cog, objectB : Cog, jointArchetype : Archetype, worldPointA : Real3, worldPointB : Real3) : Cog
> ``` 


---  
 #  CreateWorldPoints : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Create a joint (by component name) attached to the two given cogs. Both world points on the joint are set to the same world point value.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |objectB|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |jointName|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |bothWorldPoints|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function CreateWorldPoints(objectA : Cog, objectB : Cog, jointName : String, bothWorldPoints : Real3) : Cog
> ``` 


---  
 #  CreateWorldPoints : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Create a joint (by component name) attached to the two given cogs.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |objectB|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |jointName|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |worldPointA|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |worldPointB|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function CreateWorldPoints(objectA : Cog, objectB : Cog, jointName : String, worldPointA : Real3, worldPointB : Real3) : Cog
> ``` 


---  
 #  JointCreator : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function JointCreator()
> ``` 


---  
 

 
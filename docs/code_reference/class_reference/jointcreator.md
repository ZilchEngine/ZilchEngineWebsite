 `Physics`

(NOTE) A helper class to create joints of various configurations. Each joint is configured from two points. Any other specific joint properties are calculated from these two points.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddJointLimit](jointcreator.md#addjointlimit-zilch-engin)|[ AttachToCommonParent](jointcreator.md#attachtocommonparent-zer)| | |
|[ AddJointMotor](jointcreator.md#addjointmotor-zilch-engin)|[ AttachToWorld](jointcreator.md#attachtoworld-zilch-engin)| | |
|[ AddJointSpring](jointcreator.md#addjointspring-zilch-engi)|[ AutoSnaps](jointcreator.md#autosnaps-zilch-engine-do)| | |
|[ Create](jointcreator.md#create-zilch-engine-docum)|[ OverrideLength](jointcreator.md#overridelength-zilch-engi)| | |
|[ CreateLocalPoints](jointcreator.md#createlocalpoints-zilch-e)|[ UseCenter](jointcreator.md#usecenter-zilch-engine-do)| | |
|[ CreateWorldPoints](jointcreator.md#createworldpoints-zilch-e)| | | |
|[ Constructor](jointcreator.md#jointcreator-void)| | | |


 #  Properties


---  
 #  AttachToCommonParent : [boolean](../nada_base_types/boolean.md)

> Should the cog of the joint be added as a child of the common parent of the two given cogs? Useful for putting the joint in the same hierarchy so that archetypes can be created.
> ``` lang=cpp, name=Nada
> var AttachToCommonParent : Boolean


---  
 #  AttachToWorld : [boolean](../nada_base_types/boolean.md)

> Used to create a connection to a dummy object. Instead of connecting to object B, the connection will be between object A and "the world".
> ``` lang=cpp, name=Nada
> var AttachToWorld : Boolean


---  
 #  AutoSnaps : [boolean](../nada_base_types/boolean.md)

> Should the joint auto-snap when the force limit is reached?
> ``` lang=cpp, name=Nada
> var AutoSnaps : Boolean


---  
 #  OverrideLength : [boolean](../nada_base_types/boolean.md)

> Should the length of the joint be overridden or computed from the two points? Mainly used for StickJoint.
> ``` lang=cpp, name=Nada
> var OverrideLength : Boolean


---  
 #  UseCenter : [boolean](../nada_base_types/boolean.md)

> Should the center of each object be used instead of the given points?
> ``` lang=cpp, name=Nada
> var UseCenter : Boolean


---  
 #  Methods


---  
 #  AddJointLimit : [jointlimit](jointlimit.md)

> Add a JointLimit to the given joint cog.
> |Name|Type|Description|
> |---|---|---|
> |joint|[cog](cog.md)| |
> ``` lang=cpp, name=Nada
> function AddJointLimit(joint : Cog) : JointLimit
> ``` 


---  
 #  AddJointMotor : [jointmotor](jointmotor.md)

> Add a JointMotor to the given joint cog.
> |Name|Type|Description|
> |---|---|---|
> |joint|[cog](cog.md)| |
> ``` lang=cpp, name=Nada
> function AddJointMotor(joint : Cog) : JointMotor
> ``` 


---  
 #  AddJointSpring : [jointspring](jointspring.md)

> Add a JointSpring to the given joint cog.
> |Name|Type|Description|
> |---|---|---|
> |joint|[cog](cog.md)| |
> ``` lang=cpp, name=Nada
> function AddJointSpring(joint : Cog) : JointSpring
> ``` 


---  
 #  Create : [cog](cog.md)

> Create a joint (by archetype) attached to the two given cogs.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](cog.md)| |
> |objectB|[cog](cog.md)| |
> |jointArchetype|[archetype](archetype.md)| |
> ``` lang=cpp, name=Nada
> function Create(objectA : Cog, objectB : Cog, jointArchetype : Archetype) : Cog
> ``` 


---  
 #  Create : [cog](cog.md)

> Create a joint (by component name) attached to the two given cogs.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](cog.md)| |
> |objectB|[cog](cog.md)| |
> |jointName|[string](../nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function Create(objectA : Cog, objectB : Cog, jointName : String) : Cog
> ``` 


---  
 #  CreateLocalPoints : [cog](cog.md)

> Create a joint (by archetype) attached to the two given cogs.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](cog.md)| |
> |objectB|[cog](cog.md)| |
> |jointArchetype|[archetype](archetype.md)| |
> |localPointA|[real3](../nada_base_types/real3.md)| |
> |localPointB|[real3](../nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function CreateLocalPoints(objectA : Cog, objectB : Cog, jointArchetype : Archetype, localPointA : Real3, localPointB : Real3) : Cog
> ``` 


---  
 #  CreateLocalPoints : [cog](cog.md)

> Create a joint (by component name) attached to the two given cogs.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](cog.md)| |
> |objectB|[cog](cog.md)| |
> |jointName|[string](../nada_base_types/string.md)| |
> |localPointA|[real3](../nada_base_types/real3.md)| |
> |localPointB|[real3](../nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function CreateLocalPoints(objectA : Cog, objectB : Cog, jointName : String, localPointA : Real3, localPointB : Real3) : Cog
> ``` 


---  
 #  CreateWorldPoints : [cog](cog.md)

> Create a joint (by archetype) attached to the two given cogs. Both world points on the joint are set to the same world point value.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](cog.md)| |
> |objectB|[cog](cog.md)| |
> |jointArchetype|[archetype](archetype.md)| |
> |bothWorldPoints|[real3](../nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function CreateWorldPoints(objectA : Cog, objectB : Cog, jointArchetype : Archetype, bothWorldPoints : Real3) : Cog
> ``` 


---  
 #  CreateWorldPoints : [cog](cog.md)

> Create a joint (by archetype) attached to the two given cogs.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](cog.md)| |
> |objectB|[cog](cog.md)| |
> |jointArchetype|[archetype](archetype.md)| |
> |worldPointA|[real3](../nada_base_types/real3.md)| |
> |worldPointB|[real3](../nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function CreateWorldPoints(objectA : Cog, objectB : Cog, jointArchetype : Archetype, worldPointA : Real3, worldPointB : Real3) : Cog
> ``` 


---  
 #  CreateWorldPoints : [cog](cog.md)

> Create a joint (by component name) attached to the two given cogs. Both world points on the joint are set to the same world point value.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](cog.md)| |
> |objectB|[cog](cog.md)| |
> |jointName|[string](../nada_base_types/string.md)| |
> |bothWorldPoints|[real3](../nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function CreateWorldPoints(objectA : Cog, objectB : Cog, jointName : String, bothWorldPoints : Real3) : Cog
> ``` 


---  
 #  CreateWorldPoints : [cog](cog.md)

> Create a joint (by component name) attached to the two given cogs.
> |Name|Type|Description|
> |---|---|---|
> |objectA|[cog](cog.md)| |
> |objectB|[cog](cog.md)| |
> |jointName|[string](../nada_base_types/string.md)| |
> |worldPointA|[real3](../nada_base_types/real3.md)| |
> |worldPointB|[real3](../nada_base_types/real3.md)| |
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
 

 
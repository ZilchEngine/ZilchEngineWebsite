 `Resource` `Physics`



(NOTE) Defines filter pairs between CollisionGroups. These filters are used to control if collision detection and resolution happens between Colliders. Additionally, CollisionFilterBlocks can be defined on filters to send out extra events.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[CreateRuntime](collisiontable.md#createruntime-zilch-engin)| |[dataresource](dataresource.md)| |
|[FindFilter](collisiontable.md#findfilter-zilch-engine-d)| | | |
|[RuntimeClone](collisiontable.md#runtimeclone-zilch-engine)| | | |


 #  Properties


---  
 #  Methods


---  
 #  CreateRuntime : [collisiontable](collisiontable.md)

 `static`

> Creates a CollisionTable for run-time modifications.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function CreateRuntime() : CollisionTable
> ``` 


---  
 #  FindFilter : [collisionfilter](collisionfilter.md)

> Finds the filter between the pair of collision groups.
> |Name|Type|Description|
> |---|---|---|
> |groupA|[collisiongroup](collisiongroup.md)| |
> |groupB|[collisiongroup](collisiongroup.md)| |
> ```TS:Nada
> function FindFilter(groupA : CollisionGroup, groupB : CollisionGroup) : CollisionFilter
> ``` 


---  
 #  RuntimeClone : [collisiontable](collisiontable.md)

> Creates a clone of this CollisionTable for run-time modifications.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function RuntimeClone() : CollisionTable
> ``` 


---  
 

 
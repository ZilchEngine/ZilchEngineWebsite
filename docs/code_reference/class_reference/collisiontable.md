 `Resource` `Physics`



(NOTE) Defines filter pairs between CollisionGroups. These filters are used to control if collision detection and resolution happens between Colliders. Additionally, CollisionFilterBlocks can be defined on filters to send out extra events.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ CreateRuntime](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisiontable.md#createruntime-zilch-engin)| |[dataresource](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/dataresource.md)| |
|[ FindFilter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisiontable.md#findfilter-zilch-engine-d)| | | |
|[ RuntimeClone](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisiontable.md#runtimeclone-zilch-engine)| | | |


 #  Properties


---  
 #  Methods


---  
 #  CreateRuntime : [collisiontable](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisiontable.md)

 `static`

> Creates a CollisionTable for run-time modifications.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function CreateRuntime() : CollisionTable
> ``` 


---  
 #  FindFilter : [collisionfilter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisionfilter.md)

> Finds the filter between the pair of collision groups.
> |Name|Type|Description|
> |---|---|---|
> |groupA|[collisiongroup](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisiongroup.md)| |
> |groupB|[collisiongroup](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisiongroup.md)| |
> ``` lang=cpp, name=Nada
> function FindFilter(groupA : CollisionGroup, groupB : CollisionGroup) : CollisionFilter
> ``` 


---  
 #  RuntimeClone : [collisiontable](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisiontable.md)

> Creates a clone of this CollisionTable for run-time modifications.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function RuntimeClone() : CollisionTable
> ``` 


---  
 

 
 `Physics`

(NOTE) A filter for storing the relationship between a pair of groups. Stores flags for the kind of filter this is, as well as what events to send out and to whom.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](collisionfilter.md#collisionfilter-void)|[ CollisionFlag](collisionfilter.md#collisionflag-zilch-engin)|[safeid32eventobject](safeid32eventobject.md)| |
| |[ CollisionGroupA](collisionfilter.md#collisiongroupa-zilch-eng)| | |
| |[ CollisionGroupB](collisionfilter.md#collisiongroupb-zilch-eng)| | |


 #  Properties


---  
 #  CollisionFlag : [CollisionFilterCollisionFlags](../enum_reference.md#collisionfiltercollisionflags)

> The collision state between the two types. Controls whether the types skip detection, skip resolution, or resolve as normal.
> ```TS:Nada
> var CollisionFlag : CollisionFilterCollisionFlags


---  
 #  CollisionGroupA : [collisiongroup](collisiongroup.md)

 `read-only`

> 
> ```TS:Nada
> var CollisionGroupA : CollisionGroup


---  
 #  CollisionGroupB : [collisiongroup](collisiongroup.md)

 `read-only`

> 
> ```TS:Nada
> var CollisionGroupB : CollisionGroup


---  
 #  Methods


---  
 #  CollisionFilter : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function CollisionFilter()
> ``` 


---  
 

 
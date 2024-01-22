 `Component` `Physics`



(NOTE) Legacy. A position joint that is designed to manipulate one object. The only difference between this and the position joint is that the manipulator always draws itself, draws differently, and configures the max impulse differently.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](manipulatorjoint.md#manipulatorjoint-void)|[LocalPoint](manipulatorjoint.md#localpoint-zilch-engine-d)|[joint](joint.md)| |
| |[TargetPoint](manipulatorjoint.md#targetpoint-zilch-engine)| | |
| |[WorldPoint](manipulatorjoint.md#worldpoint-zilch-engine-d)| | |


 #  Properties


---  
 #  LocalPoint : [real3](../nada_base_types/real3.md)

> The local space point on the object that the joint is connected to.
> ```TS:Nada
> var LocalPoint : Real3


---  
 #  TargetPoint : [real3](../nada_base_types/real3.md)

> The point in world space that the object's point is being moved towards.
> ```TS:Nada
> var TargetPoint : Real3


---  
 #  WorldPoint : [real3](../nada_base_types/real3.md)

> The world space point on the object that the joint is connected to.
> ```TS:Nada
> var WorldPoint : Real3


---  
 #  Methods


---  
 #  ManipulatorJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ManipulatorJoint()
> ``` 


---  
 

 
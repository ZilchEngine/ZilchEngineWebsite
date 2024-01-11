 `Component` `Physics`



(NOTE) A prismatic joint sometimes called a slider) is used to create something similar to a piston. This joint fixes all degrees of rotation and leaves one linear axis free. Therefore, the bodies will rotate with each other and move with each other, except for one axis where they can move freely. Add on definitions: Limit: A limit will provide a min/max translational distance for the two objects on the slider axis. Motor: A motor will push/pull the objects on the slider axis. Spring: A spring will make the slider axis springy at its limits.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](prismaticjoint.md#prismaticjoint-void)|[ LocalAxisA](prismaticjoint.md#localaxisa-zilch-engine-d)|[joint](joint.md)| |
|[ SetWorldPoints](prismaticjoint.md#setworldpoints-void)|[ LocalAxisB](prismaticjoint.md#localaxisb-zilch-engine-d)| | |
| |[ LocalBasisA](prismaticjoint.md#localbasisa-zilch-engine)| | |
| |[ LocalBasisB](prismaticjoint.md#localbasisb-zilch-engine)| | |
| |[ LocalPointA](prismaticjoint.md#localpointa-zilch-engine)| | |
| |[ LocalPointB](prismaticjoint.md#localpointb-zilch-engine)| | |
| |[ WorldAxis](prismaticjoint.md#worldaxis-zilch-engine-do)| | |
| |[ WorldPointA](prismaticjoint.md#worldpointa-zilch-engine)| | |
| |[ WorldPointB](prismaticjoint.md#worldpointb-zilch-engine)| | |


 #  Properties


---  
 #  LocalAxisA : [real3](../nada_base_types/real3.md)

> The locally defined axis on object A . 
> ```TS:Nada
> var LocalAxisA : Real3


---  
 #  LocalAxisB : [real3](../nada_base_types/real3.md)

> The locally defined axis on object B . 
> ```TS:Nada
> var LocalAxisB : Real3


---  
 #  LocalBasisA : [quaternion](../nada_base_types/quaternion.md)

> The local space reference frame of object A . This frame is transformed to world space and then aligned with object B s frame . 
> ```TS:Nada
> var LocalBasisA : Quaternion


---  
 #  LocalBasisB : [quaternion](../nada_base_types/quaternion.md)

> The local space reference frame of object B . This frame is transformed to world space and then aligned with object A s frame . 
> ```TS:Nada
> var LocalBasisB : Quaternion


---  
 #  LocalPointA : [real3](../nada_base_types/real3.md)

> The local point of the anchor on object A . 
> ```TS:Nada
> var LocalPointA : Real3


---  
 #  LocalPointB : [real3](../nada_base_types/real3.md)

> The local point of the anchor on object B . 
> ```TS:Nada
> var LocalPointB : Real3


---  
 #  WorldAxis : [real3](../nada_base_types/real3.md)

> The axis in world space that is being rotated about . 
> ```TS:Nada
> var WorldAxis : Real3


---  
 #  WorldPointA : [real3](../nada_base_types/real3.md)

> The position of the anchor on object A given a position in world space 
> ```TS:Nada
> var WorldPointA : Real3


---  
 #  WorldPointB : [real3](../nada_base_types/real3.md)

> The position of the anchor on object B given a position in world space 
> ```TS:Nada
> var WorldPointB : Real3


---  
 #  Methods


---  
 #  PrismaticJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function PrismaticJoint()
> ``` 


---  
 #  SetWorldPoints : Void

> Sets the position of the anchor on object A and B given a position in world space 
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function SetWorldPoints(point : Real3)
> ``` 


---  
 

 
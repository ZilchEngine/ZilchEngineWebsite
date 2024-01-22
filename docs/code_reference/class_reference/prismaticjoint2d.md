 `Component` `Physics`



(NOTE) A prismatic joint is used to create something similar to a piston. This is the 2d version of PrismaticJoint. This joint is used in 2d mode for increased performance and stability. The slider axis is projected onto the z axis (the z component is ignored) so that the objects can be arbitrarily far apart. The x and y rotations are also ignored since the objects are only allowed to rotate about the z axis. Add on definitions: Limit: A limit will provide a min/max translational distance for the two objects on the slider axis. Motor: A motor will push/pull the objects on the slider axis. Spring: A spring will make the slider axis springy at its limits.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](prismaticjoint2d.md#prismaticjoint2d-void)|[LocalAxisA](prismaticjoint2d.md#localaxisa-zilch-engine-d)|[joint](joint.md)| |
|[SetWorldPoints](prismaticjoint2d.md#setworldpoints-void)|[LocalAxisB](prismaticjoint2d.md#localaxisb-zilch-engine-d)| | |
| |[LocalBasisA](prismaticjoint2d.md#localbasisa-zilch-engine)| | |
| |[LocalBasisB](prismaticjoint2d.md#localbasisb-zilch-engine)| | |
| |[LocalPointA](prismaticjoint2d.md#localpointa-zilch-engine)| | |
| |[LocalPointB](prismaticjoint2d.md#localpointb-zilch-engine)| | |
| |[WorldAxis](prismaticjoint2d.md#worldaxis-zilch-engine-do)| | |
| |[WorldPointA](prismaticjoint2d.md#worldpointa-zilch-engine)| | |
| |[WorldPointB](prismaticjoint2d.md#worldpointb-zilch-engine)| | |


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
 #  PrismaticJoint2d : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function PrismaticJoint2d()
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
 

 
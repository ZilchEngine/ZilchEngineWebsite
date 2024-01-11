 `Component` `Physics`



(NOTE) A joint that models a wheel with shocks. A wheel aligns the two local axes together and allows free rotation about this axis. The specified shock axis is turned into a soft constraint to model the shocks. Note: ObjectA should be the root object as the shock axis rotates with this object. If ObjectA is the wheel, then the shock axis will rotate with the wheel, causing the shocks to not stay aligned. Add on definitions: Limit: A limit will provide a min/max angle on the motor axis. Motor: A motor will turn the objects about the motor axis. Spring: A spring will make the shock axis springy. A spring is attached by default to a wheel.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ SetWorldPoints](wheeljoint.md#setworldpoints-void)|[ LocalAxisA](wheeljoint.md#localaxisa-zilch-engine-d)|[joint](joint.md)| |
|[ Constructor](wheeljoint.md#wheeljoint-void)|[ LocalAxisB](wheeljoint.md#localaxisb-zilch-engine-d)| | |
| |[ LocalBasisA](wheeljoint.md#localbasisa-zilch-engine)| | |
| |[ LocalBasisB](wheeljoint.md#localbasisb-zilch-engine)| | |
| |[ LocalPointA](wheeljoint.md#localpointa-zilch-engine)| | |
| |[ LocalPointB](wheeljoint.md#localpointb-zilch-engine)| | |
| |[ ShockAxis](wheeljoint.md#shockaxis-zilch-engine-do)| | |
| |[ WorldAxis](wheeljoint.md#worldaxis-zilch-engine-do)| | |
| |[ WorldPointA](wheeljoint.md#worldpointa-zilch-engine)| | |
| |[ WorldPointB](wheeljoint.md#worldpointb-zilch-engine)| | |
| |[ WorldShockAxis](wheeljoint.md#worldshockaxis-zilch-engi)| | |


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
 #  ShockAxis : [real3](../nada_base_types/real3.md)

> The shock axis in the local space of body A.
> ```TS:Nada
> var ShockAxis : Real3


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
 #  WorldShockAxis : [real3](../nada_base_types/real3.md)

> The shock axis after it has been translated into world space.
> ```TS:Nada
> var WorldShockAxis : Real3


---  
 #  Methods


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
 #  WheelJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function WheelJoint()
> ``` 


---  
 

 
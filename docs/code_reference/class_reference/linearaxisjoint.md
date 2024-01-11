 `Component` `Physics`



(NOTE) Legacy. A linear axis joint is used to keep an object locked on a plane that is defined by a normal. This was made to help make a dynamic character controller. Instead of locking translation along a plane, the constraint can be turned off with a motor attached to it which will drive movement in the direction of the plane normal. This can then be thought of as a "move in direction" constraint.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](linearaxisjoint.md#linearaxisjoint-void)|[ WorldAxis](linearaxisjoint.md#worldaxis-zilch-engine-do)|[joint](joint.md)| |


 #  Properties


---  
 #  WorldAxis : [real3](../nada_base_types/real3.md)

> The axis in world space that is constrained.
> ```TS:Nada
> var WorldAxis : Real3


---  
 #  Methods


---  
 #  LinearAxisJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function LinearAxisJoint()
> ``` 


---  
 

 
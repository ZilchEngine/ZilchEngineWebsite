 `Component` `Physics`



(NOTE) Legacy. A physics gun joint is an experimental joint for picking up objects. This acts as a weld between an object and the world. Primarily an experiment for picking up objects as a player. Should be custom implemented in script with CustomJoint instead.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](phygunjoint.md#phygunjoint-void)|[ LocalPoint](phygunjoint.md#localpoint-zilch-engine-d)|[joint](joint.md)| |
| |[ TargetPoint](phygunjoint.md#targetpoint-zilch-engine)| | |
| |[ TargetRotation](phygunjoint.md#targetrotation-zilch-engi)| | |
| |[ WorldPoint](phygunjoint.md#worldpoint-zilch-engine-d)| | |
| |[ WorldRotation](phygunjoint.md#worldrotation-zilch-engin)| | |


 #  Properties


---  
 #  LocalPoint : [real3](../nada_base_types/real3.md)

> The local point on the object that should match the target point.
> ``` lang=cpp, name=Nada
> var LocalPoint : Real3


---  
 #  TargetPoint : [real3](../nada_base_types/real3.md)

> The point in world space that the object's point should match.
> ``` lang=cpp, name=Nada
> var TargetPoint : Real3


---  
 #  TargetRotation : [quaternion](../nada_base_types/quaternion.md)

> The world space rotation that the basis of the object should match. Used to set the desired rotation of the object in world space.
> ``` lang=cpp, name=Nada
> var TargetRotation : Quaternion


---  
 #  WorldPoint : [real3](../nada_base_types/real3.md)

> The world point on the object that should match the target point.
> ``` lang=cpp, name=Nada
> var WorldPoint : Real3


---  
 #  WorldRotation : [quaternion](../nada_base_types/quaternion.md)

> Used to set the world rotation basis of the object that should be matched to the target rotation.
> ``` lang=cpp, name=Nada
> var WorldRotation : Quaternion


---  
 #  Methods


---  
 #  PhyGunJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function PhyGunJoint()
> ``` 


---  
 

 
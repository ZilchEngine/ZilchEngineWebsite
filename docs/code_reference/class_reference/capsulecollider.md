 `Component` `Physics`



(NOTE) Defines the collision volume for a capsule defined by a height and radius. A capsule can be thought of as a cylinder with spherical end caps.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](capsulecollider.md#capsulecollider-void)|[Direction](capsulecollider.md#direction-zilch-engine-do)|[collider](collider.md)| |
| |[Height](capsulecollider.md#height-zilch-engine-docum)| | |
| |[Radius](capsulecollider.md#radius-zilch-engine-docum)| | |
| |[ScalingMode](capsulecollider.md#scalingmode-zilch-engine)| | |
| |[WorldCylinderHeight](capsulecollider.md#worldcylinderheight-zero)| | |
| |[WorldRadius](capsulecollider.md#worldradius-zilch-engine)| | |


 #  Properties


---  
 #  Direction : [AxisDirection](../enum_reference.md#axisdirection)

> The direction that the height is defined along. Allows the user to change whether the capsule's height is along the local-space x, y, or z axis.
> ```TS:Nada
> var Direction : AxisDirection


---  
 #  Height : [real](../nada_base_types/real.md)

> The local space distance from the center of one sphere to another.
> ```TS:Nada
> var Height : Real


---  
 #  Radius : [real](../nada_base_types/real.md)

> The local space radius of the spheres at the capsule edges.
> ```TS:Nada
> var Radius : Real


---  
 #  ScalingMode : [CapsuleScalingMode](../enum_reference.md#capsulescalingmode)

> How should non-uniform scale affect the capsules size. Should a scale of 2 on the height axis double the total capsule size or should it double the capsule height?
> ```TS:Nada
> var ScalingMode : CapsuleScalingMode


---  
 #  WorldCylinderHeight : [real](../nada_base_types/real.md)

 `read-only`

> The full height of the capsule's cylinder after the scale is applied (world distance from one sphere to another).
> ```TS:Nada
> var WorldCylinderHeight : Real


---  
 #  WorldRadius : [real](../nada_base_types/real.md)

 `read-only`

> The radius of the sphere caps after scale is applied.
> ```TS:Nada
> var WorldRadius : Real


---  
 #  Methods


---  
 #  CapsuleCollider : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function CapsuleCollider()
> ``` 


---  
 

 
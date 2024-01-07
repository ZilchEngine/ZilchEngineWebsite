 `Component` `Physics`



(NOTE) Defines the collision volume for a capsule defined by a height and radius. A capsule can be thought of as a cylinder with spherical end caps.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/capsulecollider.md#capsulecollider-void)|[ Direction](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/capsulecollider.md#direction-zilch-engine-do)|[collider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md)| |
| |[ Height](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/capsulecollider.md#height-zilch-engine-docum)| | |
| |[ Radius](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/capsulecollider.md#radius-zilch-engine-docum)| | |
| |[ ScalingMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/capsulecollider.md#scalingmode-zilch-engine)| | |
| |[ WorldCylinderHeight](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/capsulecollider.md#worldcylinderheight-zero)| | |
| |[ WorldRadius](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/capsulecollider.md#worldradius-zilch-engine)| | |


 #  Properties


---  
 #  Direction : [AxisDirection](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#axisdirection)

> The direction that the height is defined along. Allows the user to change whether the capsule's height is along the local-space x, y, or z axis.
> ``` lang=cpp, name=Nada
> var Direction : AxisDirection


---  
 #  Height : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The local space distance from the center of one sphere to another.
> ``` lang=cpp, name=Nada
> var Height : Real


---  
 #  Radius : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The local space radius of the spheres at the capsule edges.
> ``` lang=cpp, name=Nada
> var Radius : Real


---  
 #  ScalingMode : [CapsuleScalingMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#capsulescalingmode)

> How should non-uniform scale affect the capsules size. Should a scale of 2 on the height axis double the total capsule size or should it double the capsule height?
> ``` lang=cpp, name=Nada
> var ScalingMode : CapsuleScalingMode


---  
 #  WorldCylinderHeight : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

 `read-only`

> The full height of the capsule's cylinder after the scale is applied (world distance from one sphere to another).
> ``` lang=cpp, name=Nada
> var WorldCylinderHeight : Real


---  
 #  WorldRadius : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

 `read-only`

> The radius of the sphere caps after scale is applied.
> ``` lang=cpp, name=Nada
> var WorldRadius : Real


---  
 #  Methods


---  
 #  CapsuleCollider : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function CapsuleCollider()
> ``` 


---  
 

 
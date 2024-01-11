 `Component` `Physics`



(NOTE) Defines the collision volume for a cylinder defined by a height and radius.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](cylindercollider.md#cylindercollider-void)|[ Direction](cylindercollider.md#direction-zilch-engine-do)|[collider](collider.md)| |
| |[ Height](cylindercollider.md#height-zilch-engine-docum)| | |
| |[ Radius](cylindercollider.md#radius-zilch-engine-docum)| | |
| |[ WorldHeight](cylindercollider.md#worldheight-zilch-engine)| | |
| |[ WorldRadius](cylindercollider.md#worldradius-zilch-engine)| | |


 #  Properties


---  
 #  Direction : [AxisDirection](../enum_reference.md#axisdirection)

> The direction that the height is defined along. Allows the user to change whether the cylinder's height is along the x, y, or z axis.
> ``` lang=cpp, name=Nada
> var Direction : AxisDirection


---  
 #  Height : [real](../nada_base_types/real.md)

> The local space distance from the top of the cylinder to the bottom.
> ``` lang=cpp, name=Nada
> var Height : Real


---  
 #  Radius : [real](../nada_base_types/real.md)

> The local space radius of the cylinder.
> ``` lang=cpp, name=Nada
> var Radius : Real


---  
 #  WorldHeight : [real](../nada_base_types/real.md)

 `read-only`

> The full height of the cylinder after scale is applied.
> ``` lang=cpp, name=Nada
> var WorldHeight : Real


---  
 #  WorldRadius : [real](../nada_base_types/real.md)

 `read-only`

> The radius of the cylinder after scale is applied.
> ``` lang=cpp, name=Nada
> var WorldRadius : Real


---  
 #  Methods


---  
 #  CylinderCollider : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function CylinderCollider()
> ``` 


---  
 

 
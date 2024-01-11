 `Component` `Physics`



(NOTE) Defines the collision volume for an ellipsoid (3 dimensional ellipse) defined by three radius values.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](ellipsoidcollider.md#ellipsoidcollider-void)|[ Radii](ellipsoidcollider.md#radii-zilch-engine-docume)|[collider](collider.md)| |
| |[ WorldRadii](ellipsoidcollider.md#worldradii-zilch-engine-d)| | |


 #  Properties


---  
 #  Radii : [real3](../nada_base_types/real3.md)

> The x, y, and z radius of the ellipsoid.
> ``` lang=cpp, name=Nada
> var Radii : Real3


---  
 #  WorldRadii : [real3](../nada_base_types/real3.md)

 `read-only`

> The radii of the ellipsoid after transform is applied (scale and rotation).
> ``` lang=cpp, name=Nada
> var WorldRadii : Real3


---  
 #  Methods


---  
 #  EllipsoidCollider : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function EllipsoidCollider()
> ``` 


---  
 

 
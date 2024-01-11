 `Component` `Physics`



(NOTE) Defines the collision volume for a sphere defined by a radius.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](spherecollider.md#spherecollider-void)|[ Radius](spherecollider.md#radius-zilch-engine-docum)|[collider](collider.md)| |
| |[ WorldRadius](spherecollider.md#worldradius-zilch-engine)| | |


 #  Properties


---  
 #  Radius : [real](../nada_base_types/real.md)

> The radius of the sphere in local space (before transform is applied).
> ``` lang=cpp, name=Nada
> var Radius : Real


---  
 #  WorldRadius : [real](../nada_base_types/real.md)

 `read-only`

> The radius of the sphere after transform is applied (scale).
> ``` lang=cpp, name=Nada
> var WorldRadius : Real


---  
 #  Methods


---  
 #  SphereCollider : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function SphereCollider()
> ``` 


---  
 

 
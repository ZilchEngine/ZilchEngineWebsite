 `Component` `Physics`



(NOTE) Defines the collision volume for a sphere defined by a radius.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spherecollider.md#spherecollider-void)|[ Radius](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spherecollider.md#radius-zilch-engine-docum)|[collider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md)| |
| |[ WorldRadius](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spherecollider.md#worldradius-zilch-engine)| | |


 #  Properties


---  
 #  Radius : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The radius of the sphere in local space (before transform is applied).
> ``` lang=cpp, name=Nada
> var Radius : Real


---  
 #  WorldRadius : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

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
 

 
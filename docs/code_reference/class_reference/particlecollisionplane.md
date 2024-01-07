 `Component` `Graphics`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particlecollisionplane.md#particlecollisionplane-v)|[ Friction](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particlecollisionplane.md#friction-zilch-engine-doc)|[particleanimator](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particleanimator.md)| |
| |[ PlaneNormal](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particlecollisionplane.md#planenormal-zilch-engine)| | |
| |[ PlanePosition](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particlecollisionplane.md#planeposition-zilch-engin)| | |
| |[ PlaneSpace](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particlecollisionplane.md#planespace-zilch-engine-d)| | |
| |[ Restitution](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particlecollisionplane.md#restitution-zilch-engine)| | |


 #  Properties


---  
 #  Friction : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> How slippery or rough the particle is. When friction is 0, the object will be slippery. When friction is 1, it will completely stop in the direction tangential to the collision normal. Values should be in the range [0, 1].
> ``` lang=cpp, name=Nada
> var Friction : Real


---  
 #  PlaneNormal : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> 
> ``` lang=cpp, name=Nada
> var PlaneNormal : Real3


---  
 #  PlanePosition : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> 
> ``` lang=cpp, name=Nada
> var PlanePosition : Real3


---  
 #  PlaneSpace : [SystemSpace](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#systemspace)

> 
> ``` lang=cpp, name=Nada
> var PlaneSpace : SystemSpace


---  
 #  Restitution : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> How much the particle will bounce during a collision. Values should be in the range of [0, 1], where 0 is an in-elastic collision and 1 is a fully elastic collision (bouncy). If the value is greater than 1, the particle will gain energy and move faster after the bounce.
> ``` lang=cpp, name=Nada
> var Restitution : Real


---  
 #  Methods


---  
 #  ParticleCollisionPlane : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ParticleCollisionPlane()
> ``` 


---  
 

 
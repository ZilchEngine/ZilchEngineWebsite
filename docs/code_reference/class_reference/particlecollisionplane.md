 `Component` `Graphics`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](particlecollisionplane.md#particlecollisionplane-v)|[Friction](particlecollisionplane.md#friction-zilch-engine-doc)|[particleanimator](particleanimator.md)| |
| |[PlaneNormal](particlecollisionplane.md#planenormal-zilch-engine)| | |
| |[PlanePosition](particlecollisionplane.md#planeposition-zilch-engin)| | |
| |[PlaneSpace](particlecollisionplane.md#planespace-zilch-engine-d)| | |
| |[Restitution](particlecollisionplane.md#restitution-zilch-engine)| | |


 #  Properties


---  
 #  Friction : [real](../nada_base_types/real.md)

> How slippery or rough the particle is. When friction is 0, the object will be slippery. When friction is 1, it will completely stop in the direction tangential to the collision normal. Values should be in the range [0, 1].
> ```TS:Nada
> var Friction : Real


---  
 #  PlaneNormal : [real3](../nada_base_types/real3.md)

> 
> ```TS:Nada
> var PlaneNormal : Real3


---  
 #  PlanePosition : [real3](../nada_base_types/real3.md)

> 
> ```TS:Nada
> var PlanePosition : Real3


---  
 #  PlaneSpace : [SystemSpace](../enum_reference.md#systemspace)

> 
> ```TS:Nada
> var PlaneSpace : SystemSpace


---  
 #  Restitution : [real](../nada_base_types/real.md)

> How much the particle will bounce during a collision. Values should be in the range of [0, 1], where 0 is an in-elastic collision and 1 is a fully elastic collision (bouncy). If the value is greater than 1, the particle will gain energy and move faster after the bounce.
> ```TS:Nada
> var Restitution : Real


---  
 #  Methods


---  
 #  ParticleCollisionPlane : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ParticleCollisionPlane()
> ``` 


---  
 

 
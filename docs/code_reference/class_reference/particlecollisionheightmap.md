 `Component` `Graphics`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](particlecollisionheightmap.md#particlecollisionheightm)|[Friction](particlecollisionheightmap.md#friction-zilch-engine-doc)|[particleanimator](particleanimator.md)| |
| |[HeightMap](particlecollisionheightmap.md#heightmap-zilch-engine-do)| | |
| |[Restitution](particlecollisionheightmap.md#restitution-zilch-engine)| | |


 #  Properties


---  
 #  Friction : [real](../nada_base_types/real.md)

> How slippery or rough the particle is. When friction is 0, the object will be slippery. When friction is 1, it will completely stop in the direction tangential to the collision normal.
> ```TS:Nada
> var Friction : Real


---  
 #  HeightMap : [cogpath](cogpath.md)

> 
> ```TS:Nada
> var HeightMap : CogPath


---  
 #  Restitution : [real](../nada_base_types/real.md)

> How much the particle will bounce during a collision. Values should be in the range of [0, 1], where 0 is an in-elastic collision and 1 is a fully elastic collision (bouncy). If the value is greater than 1, the particle will gain energy and move faster after the bounce.
> ```TS:Nada
> var Restitution : Real


---  
 #  Methods


---  
 #  ParticleCollisionHeightmap : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ParticleCollisionHeightmap()
> ``` 


---  
 

 
 `Component` `Graphics`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particlecollisionheightmap.md#particlecollisionheightm)|[ Friction](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particlecollisionheightmap.md#friction-zilch-engine-doc)|[particleanimator](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particleanimator.md)| |
| |[ HeightMap](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particlecollisionheightmap.md#heightmap-zilch-engine-do)| | |
| |[ Restitution](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particlecollisionheightmap.md#restitution-zilch-engine)| | |


 #  Properties


---  
 #  Friction : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> How slippery or rough the particle is. When friction is 0, the object will be slippery. When friction is 1, it will completely stop in the direction tangential to the collision normal.
> ``` lang=cpp, name=Nada
> var Friction : Real


---  
 #  HeightMap : [cogpath](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cogpath.md)

> 
> ``` lang=cpp, name=Nada
> var HeightMap : CogPath


---  
 #  Restitution : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> How much the particle will bounce during a collision. Values should be in the range of [0, 1], where 0 is an in-elastic collision and 1 is a fully elastic collision (bouncy). If the value is greater than 1, the particle will gain energy and move faster after the bounce.
> ``` lang=cpp, name=Nada
> var Restitution : Real


---  
 #  Methods


---  
 #  ParticleCollisionHeightmap : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ParticleCollisionHeightmap()
> ``` 


---  
 

 
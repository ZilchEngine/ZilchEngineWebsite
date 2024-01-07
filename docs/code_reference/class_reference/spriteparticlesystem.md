 `Component` `Graphics`



(NOTE) A particle system that uses sprites to represent each particle.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spriteparticlesystem.md#spriteparticlesystem-voi)|[ BeamBaseScale](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spriteparticlesystem.md#beambasescale-zilch-engin)|[particlesystem](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particlesystem.md)| |
| |[ BeamVelocityScale](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spriteparticlesystem.md#beamvelocityscale-zilch-e)| | |
| |[ GeometryMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spriteparticlesystem.md#geometrymode-zilch-engine)| | |
| |[ ParticleAnimation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spriteparticlesystem.md#particleanimation-zilch-e)| | |
| |[ ParticleSort](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spriteparticlesystem.md#particlesort-zilch-engine)| | |
| |[ SpriteSource](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spriteparticlesystem.md#spritesource-zilch-engine)| | |
| |[ VertexColor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spriteparticlesystem.md#vertexcolor-zilch-engine)| | |


 #  Properties


---  
 #  BeamBaseScale : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> How much to scale particles along their direction of movement.
> ``` lang=cpp, name=Nada
> var BeamBaseScale : Real


---  
 #  BeamVelocityScale : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> How much additional scale to add to particles by how fast they are moving.
> ``` lang=cpp, name=Nada
> var BeamVelocityScale : Real


---  
 #  GeometryMode : [SpriteParticleGeometryMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#spriteparticlegeometrymode)

> How the geometry of the particles are generated.
> ``` lang=cpp, name=Nada
> var GeometryMode : SpriteParticleGeometryMode


---  
 #  ParticleAnimation : [SpriteParticleAnimationMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#spriteparticleanimationmode)

> How the sprite's animation should be used.
> ``` lang=cpp, name=Nada
> var ParticleAnimation : SpriteParticleAnimationMode


---  
 #  ParticleSort : [SpriteParticleSortMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#spriteparticlesortmode)

> How particles should be sorted with each other, determines draw order between particles.
> ``` lang=cpp, name=Nada
> var ParticleSort : SpriteParticleSortMode


---  
 #  SpriteSource : [spritesource](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spritesource.md)

> The sprite definition to use for each particle.
> ``` lang=cpp, name=Nada
> var SpriteSource : SpriteSource


---  
 #  VertexColor : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

> Color attribute of the generated vertices accessible in the vertex shader, value is multiplied with the particle color.
> ``` lang=cpp, name=Nada
> var VertexColor : Real4


---  
 #  Methods


---  
 #  SpriteParticleSystem : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function SpriteParticleSystem()
> ``` 


---  
 

 
 `Component` `Graphics`



(NOTE) A particle system that uses sprites to represent each particle.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](spriteparticlesystem.md#spriteparticlesystem-voi)|[ BeamBaseScale](spriteparticlesystem.md#beambasescale-zilch-engin)|[particlesystem](particlesystem.md)| |
| |[ BeamVelocityScale](spriteparticlesystem.md#beamvelocityscale-zilch-e)| | |
| |[ GeometryMode](spriteparticlesystem.md#geometrymode-zilch-engine)| | |
| |[ ParticleAnimation](spriteparticlesystem.md#particleanimation-zilch-e)| | |
| |[ ParticleSort](spriteparticlesystem.md#particlesort-zilch-engine)| | |
| |[ SpriteSource](spriteparticlesystem.md#spritesource-zilch-engine)| | |
| |[ VertexColor](spriteparticlesystem.md#vertexcolor-zilch-engine)| | |


 #  Properties


---  
 #  BeamBaseScale : [real](../nada_base_types/real.md)

> How much to scale particles along their direction of movement.
> ``` lang=cpp, name=Nada
> var BeamBaseScale : Real


---  
 #  BeamVelocityScale : [real](../nada_base_types/real.md)

> How much additional scale to add to particles by how fast they are moving.
> ``` lang=cpp, name=Nada
> var BeamVelocityScale : Real


---  
 #  GeometryMode : [SpriteParticleGeometryMode](../enum_reference.md#spriteparticlegeometrymode)

> How the geometry of the particles are generated.
> ``` lang=cpp, name=Nada
> var GeometryMode : SpriteParticleGeometryMode


---  
 #  ParticleAnimation : [SpriteParticleAnimationMode](../enum_reference.md#spriteparticleanimationmode)

> How the sprite's animation should be used.
> ``` lang=cpp, name=Nada
> var ParticleAnimation : SpriteParticleAnimationMode


---  
 #  ParticleSort : [SpriteParticleSortMode](../enum_reference.md#spriteparticlesortmode)

> How particles should be sorted with each other, determines draw order between particles.
> ``` lang=cpp, name=Nada
> var ParticleSort : SpriteParticleSortMode


---  
 #  SpriteSource : [spritesource](spritesource.md)

> The sprite definition to use for each particle.
> ``` lang=cpp, name=Nada
> var SpriteSource : SpriteSource


---  
 #  VertexColor : [real4](../nada_base_types/real4.md)

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
 

 
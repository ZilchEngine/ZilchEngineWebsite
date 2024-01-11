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
> ```TS:Nada
> var BeamBaseScale : Real


---  
 #  BeamVelocityScale : [real](../nada_base_types/real.md)

> How much additional scale to add to particles by how fast they are moving.
> ```TS:Nada
> var BeamVelocityScale : Real


---  
 #  GeometryMode : [SpriteParticleGeometryMode](../enum_reference.md#spriteparticlegeometrymode)

> How the geometry of the particles are generated.
> ```TS:Nada
> var GeometryMode : SpriteParticleGeometryMode


---  
 #  ParticleAnimation : [SpriteParticleAnimationMode](../enum_reference.md#spriteparticleanimationmode)

> How the sprite's animation should be used.
> ```TS:Nada
> var ParticleAnimation : SpriteParticleAnimationMode


---  
 #  ParticleSort : [SpriteParticleSortMode](../enum_reference.md#spriteparticlesortmode)

> How particles should be sorted with each other, determines draw order between particles.
> ```TS:Nada
> var ParticleSort : SpriteParticleSortMode


---  
 #  SpriteSource : [spritesource](spritesource.md)

> The sprite definition to use for each particle.
> ```TS:Nada
> var SpriteSource : SpriteSource


---  
 #  VertexColor : [real4](../nada_base_types/real4.md)

> Color attribute of the generated vertices accessible in the vertex shader, value is multiplied with the particle color.
> ```TS:Nada
> var VertexColor : Real4


---  
 #  Methods


---  
 #  SpriteParticleSystem : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function SpriteParticleSystem()
> ``` 


---  
 

 
 `Component` `Graphics`



(NOTE) An interface for generating and managing particles of a generic definition using emitters and animators.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AllParticles](particlesystem.md#allparticles-zilch-engine)|[ BoundingBoxSize](particlesystem.md#boundingboxsize-zilch-eng)|[graphical](graphical.md)|[spriteparticlesystem](spriteparticlesystem.md)|
|[ Clear](particlesystem.md#clear-void)|[ ChildSystem](particlesystem.md#childsystem-zilch-engine)| | |
| |[ PreviewInEditor](particlesystem.md#previewineditor-zilch-eng)| | |
| |[ SystemSpace](particlesystem.md#systemspace-zilch-engine)| | |
| |[ WarmUpTime](particlesystem.md#warmuptime-zilch-engine-d)| | |


 #  Properties


---  
 #  BoundingBoxSize : [real](../nada_base_types/real.md)

> Size of all sides of the bounding box used for frustum culling.
> ```TS:Nada
> var BoundingBoxSize : Real


---  
 #  ChildSystem : [boolean](../nada_base_types/boolean.md)

> If set, particle emission will happen for each particle in a parent system.
> ```TS:Nada
> var ChildSystem : Boolean


---  
 #  PreviewInEditor : [boolean](../nada_base_types/boolean.md)

> If the particle system should run on frame update in the editor instead of logic update.
> ```TS:Nada
> var PreviewInEditor : Boolean


---  
 #  SystemSpace : [SystemSpace](../enum_reference.md#systemspace)

> If particles are emitted into world space or if transform data remains relative to the transform of the system object.
> ```TS:Nada
> var SystemSpace : SystemSpace


---  
 #  WarmUpTime : [real](../nada_base_types/real.md)

> The amount of time to simulate the particle system on startup. This will be done on AllObjectsCreated, and will use the engines dt. This is good for when you want the particle effect to be in full bloom when you first see it. However, it can hurt performance at high values on startup.
> ```TS:Nada
> var WarmUpTime : Real


---  
 #  Methods


---  
 #  AllParticles : [particlelistrange](particlelistrange.md)

> A list of all particles currently active in the system.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function AllParticles() : ParticleListRange
> ``` 


---  
 #  Clear : Void

> Clear all current particles.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Clear()
> ``` 


---  
 

 
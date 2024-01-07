 `Component` `Graphics`



(NOTE) An interface for generating and managing particles of a generic definition using emitters and animators.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AllParticles](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particlesystem.md#allparticles-zilch-engine)|[ BoundingBoxSize](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particlesystem.md#boundingboxsize-zilch-eng)|[graphical](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/graphical.md)|[spriteparticlesystem](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spriteparticlesystem.md)|
|[ Clear](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particlesystem.md#clear-void)|[ ChildSystem](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particlesystem.md#childsystem-zilch-engine)| | |
| |[ PreviewInEditor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particlesystem.md#previewineditor-zilch-eng)| | |
| |[ SystemSpace](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particlesystem.md#systemspace-zilch-engine)| | |
| |[ WarmUpTime](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particlesystem.md#warmuptime-zilch-engine-d)| | |


 #  Properties


---  
 #  BoundingBoxSize : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Size of all sides of the bounding box used for frustum culling.
> ``` lang=cpp, name=Nada
> var BoundingBoxSize : Real


---  
 #  ChildSystem : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> If set, particle emission will happen for each particle in a parent system.
> ``` lang=cpp, name=Nada
> var ChildSystem : Boolean


---  
 #  PreviewInEditor : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> If the particle system should run on frame update in the editor instead of logic update.
> ``` lang=cpp, name=Nada
> var PreviewInEditor : Boolean


---  
 #  SystemSpace : [SystemSpace](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#systemspace)

> If particles are emitted into world space or if transform data remains relative to the transform of the system object.
> ``` lang=cpp, name=Nada
> var SystemSpace : SystemSpace


---  
 #  WarmUpTime : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The amount of time to simulate the particle system on startup. This will be done on AllObjectsCreated, and will use the engines dt. This is good for when you want the particle effect to be in full bloom when you first see it. However, it can hurt performance at high values on startup.
> ``` lang=cpp, name=Nada
> var WarmUpTime : Real


---  
 #  Methods


---  
 #  AllParticles : [particlelistrange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particlelistrange.md)

> A list of all particles currently active in the system.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function AllParticles() : ParticleListRange
> ``` 


---  
 #  Clear : Void

> Clear all current particles.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Clear()
> ``` 


---  
 

 
 `Component` `Gameplay`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/splineparticleanimator.md#splineparticleanimator-v)|[ AutoCalculateLifetime](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/splineparticleanimator.md#autocalculatelifetime-ze)|[particleanimator](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particleanimator.md)| |
| |[ Helix](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/splineparticleanimator.md#helix-zilch-engine-docume)| | |
| |[ HelixOffset](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/splineparticleanimator.md#helixoffset-zilch-engine)| | |
| |[ HelixRadius](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/splineparticleanimator.md#helixradius-zilch-engine)| | |
| |[ HelixWaveLength](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/splineparticleanimator.md#helixwavelength-zilch-eng)| | |
| |[ Mode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/splineparticleanimator.md#mode-zilch-engine-documen)| | |
| |[ Speed](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/splineparticleanimator.md#speed-zilch-engine-docume)| | |
| |[ SpringDampingRatio](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/splineparticleanimator.md#springdampingratio-zero)| | |
| |[ SpringFrequencyHz](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/splineparticleanimator.md#springfrequencyhz-zilch-e)| | |


 #  Properties


---  
 #  AutoCalculateLifetime : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> If checked, the lifetime on the SplineParticleEmitter will be updated to the time it would take to travel the entire path at the current speed.
> ``` lang=cpp, name=Nada
> var AutoCalculateLifetime : Boolean


---  
 #  Helix : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var Helix : Boolean


---  
 #  HelixOffset : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Offset in radians for where the helix starts.
> ``` lang=cpp, name=Nada
> var HelixOffset : Real


---  
 #  HelixRadius : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The radius of the helix.
> ``` lang=cpp, name=Nada
> var HelixRadius : Real


---  
 #  HelixWaveLength : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> How fast the helix rotates in radians / second.
> ``` lang=cpp, name=Nada
> var HelixWaveLength : Real


---  
 #  Mode : [SplineAnimatorMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#splineanimatormode)

> The current animate mode.
> ``` lang=cpp, name=Nada
> var Mode : SplineAnimatorMode


---  
 #  Speed : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The speed at which the particles move in meters / second.
> ``` lang=cpp, name=Nada
> var Speed : Real


---  
 #  SpringDampingRatio : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> 
> ``` lang=cpp, name=Nada
> var SpringDampingRatio : Real


---  
 #  SpringFrequencyHz : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Spring properties.
> ``` lang=cpp, name=Nada
> var SpringFrequencyHz : Real


---  
 #  Methods


---  
 #  SplineParticleAnimator : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function SplineParticleAnimator()
> ``` 


---  
 

 
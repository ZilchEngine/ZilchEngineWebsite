 `Component` `Graphics`



(NOTE) Particle Emitter Shared.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ResetCount](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particleemittershared.md#resetcount-void)|[ Active](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particleemittershared.md#active-zilch-engine-docum)|[particleemitter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particleemitter.md)|[boxparticleemitter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxparticleemitter.md)|
| |[ EmitCount](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particleemittershared.md#emitcount-zilch-engine-do)| |[meshparticleemitter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/meshparticleemitter.md)|
| |[ EmitDelay](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particleemittershared.md#emitdelay-zilch-engine-do)| |[sphericalparticleemitter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sphericalparticleemitter.md)|
| |[ EmitRate](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particleemittershared.md#emitrate-zilch-engine-doc)| |[splineparticleemitter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/splineparticleemitter.md)|
| |[ EmitRateSoftStartTime](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particleemittershared.md#emitratesoftstarttime-ze)| | |
| |[ EmitterSize](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particleemittershared.md#emittersize-zilch-engine)| | |
| |[ EmitterVelocityPercent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particleemittershared.md#emittervelocitypercent-z)| | |
| |[ EmitVariance](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particleemittershared.md#emitvariance-zilch-engine)| | |
| |[ FastMovingEmitter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particleemittershared.md#fastmovingemitter-zilch-e)| | |
| |[ Fill](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particleemittershared.md#fill-zilch-engine-documen)| | |
| |[ Lifetime](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particleemittershared.md#lifetime-zilch-engine-doc)| | |
| |[ LifetimeVariance](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particleemittershared.md#lifetimevariance-zilch-en)| | |
| |[ RandomSpin](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particleemittershared.md#randomspin-zilch-engine-d)| | |
| |[ RandomVelocity](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particleemittershared.md#randomvelocity-zilch-engi)| | |
| |[ Size](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particleemittershared.md#size-zilch-engine-documen)| | |
| |[ SizeVariance](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particleemittershared.md#sizevariance-zilch-engine)| | |
| |[ Spin](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particleemittershared.md#spin-zilch-engine-documen)| | |
| |[ SpinVariance](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particleemittershared.md#spinvariance-zilch-engine)| | |
| |[ StartVelocity](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particleemittershared.md#startvelocity-zilch-engin)| | |
| |[ TangentVelocity](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particleemittershared.md#tangentvelocity-zilch-eng)| | |


 #  Properties


---  
 #  Active : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Is this emitter currently emitting particles?
> ``` lang=cpp, name=Nada
> var Active : Boolean


---  
 #  EmitCount : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> Number of particles to emit per reset.
> ``` lang=cpp, name=Nada
> var EmitCount : Integer


---  
 #  EmitDelay : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Time in seconds to delay the emission of particles from time of creation.
> ``` lang=cpp, name=Nada
> var EmitDelay : Real


---  
 #  EmitRate : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Rate that particles spawn per second.
> ``` lang=cpp, name=Nada
> var EmitRate : Real


---  
 #  EmitRateSoftStartTime : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Slowly ramps up to EmitRate over this time.
> ``` lang=cpp, name=Nada
> var EmitRateSoftStartTime : Real


---  
 #  EmitterSize : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Size of the emitter.
> ``` lang=cpp, name=Nada
> var EmitterSize : Real3


---  
 #  EmitterVelocityPercent : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> How much of the objects velocity is added to the particles.
> ``` lang=cpp, name=Nada
> var EmitterVelocityPercent : Real


---  
 #  EmitVariance : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> How much the emit can vary per sample.
> ``` lang=cpp, name=Nada
> var EmitVariance : Real


---  
 #  FastMovingEmitter : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Whether or not we attempt to emit along the vector between the previous position to the current position, which looks better for fast moving particle systems Note: Particle systems that teleport will emit along the teleport line.
> ``` lang=cpp, name=Nada
> var FastMovingEmitter : Boolean


---  
 #  Fill : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> How much area of the emitter to used 0 to 1.
> ``` lang=cpp, name=Nada
> var Fill : Real


---  
 #  Lifetime : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> How a particle's starting lifetime is.
> ``` lang=cpp, name=Nada
> var Lifetime : Real


---  
 #  LifetimeVariance : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> How much lifetime can vary per particle.
> ``` lang=cpp, name=Nada
> var LifetimeVariance : Real


---  
 #  RandomSpin : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Each particle should start with random spin.
> ``` lang=cpp, name=Nada
> var RandomSpin : Boolean


---  
 #  RandomVelocity : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Random Velocity per particle.
> ``` lang=cpp, name=Nada
> var RandomVelocity : Real3


---  
 #  Size : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Size of each particle spawned.
> ``` lang=cpp, name=Nada
> var Size : Real


---  
 #  SizeVariance : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> How much the size can vary from the base size per particle.
> ``` lang=cpp, name=Nada
> var SizeVariance : Real


---  
 #  Spin : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Speed in rads per second of the particle.
> ``` lang=cpp, name=Nada
> var Spin : Real


---  
 #  SpinVariance : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> How much spin speed can vary per particle.
> ``` lang=cpp, name=Nada
> var SpinVariance : Real


---  
 #  StartVelocity : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Velocity of each particle at start.
> ``` lang=cpp, name=Nada
> var StartVelocity : Real3


---  
 #  TangentVelocity : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Velocity of each particle in x horizontal tangent y vertical tangent and z outward tangent.
> ``` lang=cpp, name=Nada
> var TangentVelocity : Real3


---  
 #  Methods


---  
 #  ResetCount : Void

> Reset the number of particles to emit back to EmitCount.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ResetCount()
> ``` 


---  
 

 
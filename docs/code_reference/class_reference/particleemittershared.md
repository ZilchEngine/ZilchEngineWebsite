 `Component` `Graphics`



(NOTE) Particle Emitter Shared.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ResetCount](particleemittershared.md#resetcount-void)|[Active](particleemittershared.md#active-zilch-engine-docum)|[particleemitter](particleemitter.md)|[boxparticleemitter](boxparticleemitter.md)|
| |[EmitCount](particleemittershared.md#emitcount-zilch-engine-do)| |[meshparticleemitter](meshparticleemitter.md)|
| |[EmitDelay](particleemittershared.md#emitdelay-zilch-engine-do)| |[sphericalparticleemitter](sphericalparticleemitter.md)|
| |[EmitRate](particleemittershared.md#emitrate-zilch-engine-doc)| |[splineparticleemitter](splineparticleemitter.md)|
| |[EmitRateSoftStartTime](particleemittershared.md#emitratesoftstarttime-ze)| | |
| |[EmitterSize](particleemittershared.md#emittersize-zilch-engine)| | |
| |[EmitterVelocityPercent](particleemittershared.md#emittervelocitypercent-z)| | |
| |[EmitVariance](particleemittershared.md#emitvariance-zilch-engine)| | |
| |[FastMovingEmitter](particleemittershared.md#fastmovingemitter-zilch-e)| | |
| |[Fill](particleemittershared.md#fill-zilch-engine-documen)| | |
| |[Lifetime](particleemittershared.md#lifetime-zilch-engine-doc)| | |
| |[LifetimeVariance](particleemittershared.md#lifetimevariance-zilch-en)| | |
| |[RandomSpin](particleemittershared.md#randomspin-zilch-engine-d)| | |
| |[RandomVelocity](particleemittershared.md#randomvelocity-zilch-engi)| | |
| |[Size](particleemittershared.md#size-zilch-engine-documen)| | |
| |[SizeVariance](particleemittershared.md#sizevariance-zilch-engine)| | |
| |[Spin](particleemittershared.md#spin-zilch-engine-documen)| | |
| |[SpinVariance](particleemittershared.md#spinvariance-zilch-engine)| | |
| |[StartVelocity](particleemittershared.md#startvelocity-zilch-engin)| | |
| |[TangentVelocity](particleemittershared.md#tangentvelocity-zilch-eng)| | |


 #  Properties


---  
 #  Active : [boolean](../nada_base_types/boolean.md)

> Is this emitter currently emitting particles?
> ```TS:Nada
> var Active : Boolean


---  
 #  EmitCount : [integer](../nada_base_types/integer.md)

> Number of particles to emit per reset.
> ```TS:Nada
> var EmitCount : Integer


---  
 #  EmitDelay : [real](../nada_base_types/real.md)

> Time in seconds to delay the emission of particles from time of creation.
> ```TS:Nada
> var EmitDelay : Real


---  
 #  EmitRate : [real](../nada_base_types/real.md)

> Rate that particles spawn per second.
> ```TS:Nada
> var EmitRate : Real


---  
 #  EmitRateSoftStartTime : [real](../nada_base_types/real.md)

> Slowly ramps up to EmitRate over this time.
> ```TS:Nada
> var EmitRateSoftStartTime : Real


---  
 #  EmitterSize : [real3](../nada_base_types/real3.md)

> Size of the emitter.
> ```TS:Nada
> var EmitterSize : Real3


---  
 #  EmitterVelocityPercent : [real](../nada_base_types/real.md)

> How much of the objects velocity is added to the particles.
> ```TS:Nada
> var EmitterVelocityPercent : Real


---  
 #  EmitVariance : [real](../nada_base_types/real.md)

> How much the emit can vary per sample.
> ```TS:Nada
> var EmitVariance : Real


---  
 #  FastMovingEmitter : [boolean](../nada_base_types/boolean.md)

> Whether or not we attempt to emit along the vector between the previous position to the current position, which looks better for fast moving particle systems Note: Particle systems that teleport will emit along the teleport line.
> ```TS:Nada
> var FastMovingEmitter : Boolean


---  
 #  Fill : [real](../nada_base_types/real.md)

> How much area of the emitter to used 0 to 1.
> ```TS:Nada
> var Fill : Real


---  
 #  Lifetime : [real](../nada_base_types/real.md)

> How a particle's starting lifetime is.
> ```TS:Nada
> var Lifetime : Real


---  
 #  LifetimeVariance : [real](../nada_base_types/real.md)

> How much lifetime can vary per particle.
> ```TS:Nada
> var LifetimeVariance : Real


---  
 #  RandomSpin : [boolean](../nada_base_types/boolean.md)

> Each particle should start with random spin.
> ```TS:Nada
> var RandomSpin : Boolean


---  
 #  RandomVelocity : [real3](../nada_base_types/real3.md)

> Random Velocity per particle.
> ```TS:Nada
> var RandomVelocity : Real3


---  
 #  Size : [real](../nada_base_types/real.md)

> Size of each particle spawned.
> ```TS:Nada
> var Size : Real


---  
 #  SizeVariance : [real](../nada_base_types/real.md)

> How much the size can vary from the base size per particle.
> ```TS:Nada
> var SizeVariance : Real


---  
 #  Spin : [real](../nada_base_types/real.md)

> Speed in rads per second of the particle.
> ```TS:Nada
> var Spin : Real


---  
 #  SpinVariance : [real](../nada_base_types/real.md)

> How much spin speed can vary per particle.
> ```TS:Nada
> var SpinVariance : Real


---  
 #  StartVelocity : [real3](../nada_base_types/real3.md)

> Velocity of each particle at start.
> ```TS:Nada
> var StartVelocity : Real3


---  
 #  TangentVelocity : [real3](../nada_base_types/real3.md)

> Velocity of each particle in x horizontal tangent y vertical tangent and z outward tangent.
> ```TS:Nada
> var TangentVelocity : Real3


---  
 #  Methods


---  
 #  ResetCount : Void

> Reset the number of particles to emit back to EmitCount.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ResetCount()
> ``` 


---  
 

 
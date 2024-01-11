 `Component` `Graphics`



(NOTE) Basic Particle Animation Effects.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](linearparticleanimator.md#linearparticleanimator-v)|[ Dampening](linearparticleanimator.md#dampening-zilch-engine-do)|[particleanimator](particleanimator.md)| |
| |[ Force](linearparticleanimator.md#force-zilch-engine-docume)| | |
| |[ Growth](linearparticleanimator.md#growth-zilch-engine-docum)| | |
| |[ RandomForce](linearparticleanimator.md#randomforce-zilch-engine)| | |
| |[ Torque](linearparticleanimator.md#torque-zilch-engine-docum)| | |
| |[ Twist](linearparticleanimator.md#twist-zilch-engine-docume)| | |


 #  Properties


---  
 #  Dampening : [real](../nada_base_types/real.md)

> Velocity dampening.
> ```TS:Nada
> var Dampening : Real


---  
 #  Force : [real3](../nada_base_types/real3.md)

> Constance force applied to particles.
> ```TS:Nada
> var Force : Real3


---  
 #  Growth : [real](../nada_base_types/real.md)

> Rate of particle size growth.
> ```TS:Nada
> var Growth : Real


---  
 #  RandomForce : [real3](../nada_base_types/real3.md)

> Random force applied to particles.
> ```TS:Nada
> var RandomForce : Real3


---  
 #  Torque : [real](../nada_base_types/real.md)

> Force that applies spin.
> ```TS:Nada
> var Torque : Real


---  
 #  Twist : [real3](../nada_base_types/real3.md)

> Twist applies a twisting/tornado force to the particles.
> ```TS:Nada
> var Twist : Real3


---  
 #  Methods


---  
 #  LinearParticleAnimator : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function LinearParticleAnimator()
> ``` 


---  
 

 
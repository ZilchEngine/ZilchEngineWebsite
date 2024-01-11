 `Component` `Physics`



(NOTE) Applies a force about an axis at the object's center. This will apply two forces to a body: One pulls the object towards the center of the vortex and the other applies a tangential force. Useful to model a vortex. This only expects to be used as a Region effect.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](vortexeffect.md#vortexeffect-void)|[ EndCondition](vortexeffect.md#endcondition-zilch-engine)|[physicseffect](physicseffect.md)| |
| |[ InterpolationType](vortexeffect.md#interpolationtype-zilch-e)| | |
| |[ InwardStrengthAtMaxDistance](vortexeffect.md#inwardstrengthatmaxdista)| | |
| |[ InwardStrengthAtMinDistance](vortexeffect.md#inwardstrengthatmindista)| | |
| |[ LocalAxis](vortexeffect.md#localaxis-zilch-engine-do)| | |
| |[ MaxDistance](vortexeffect.md#maxdistance-zilch-engine)| | |
| |[ MinDistance](vortexeffect.md#mindistance-zilch-engine)| | |
| |[ TwistStrengthAtMaxDistance](vortexeffect.md#twiststrengthatmaxdistan)| | |
| |[ TwistStrengthAtMinDistance](vortexeffect.md#twiststrengthatmindistan)| | |
| |[ VortexAxis](vortexeffect.md#vortexaxis-zilch-engine-d)| | |
| |[ WorldVortexAxis](vortexeffect.md#worldvortexaxis-zilch-eng)| | |


 #  Properties


---  
 #  EndCondition : [PhysicsEffectEndCondition](../enum_reference.md#physicseffectendcondition)

> How the interpolation should be handled at MaxDistance. ClampToMax will clamp to the max strength values. NoEffect will ignore the effect. ContinueFalloff will continue the interpolation (this may go negative).
> ``` lang=cpp, name=Nada
> var EndCondition : PhysicsEffectEndCondition


---  
 #  InterpolationType : [PhysicsEffectInterpolationType](../enum_reference.md#physicseffectinterpolationtype)

> The type of interpolation used (e.g. Linear, Quadratic) for the forces.
> ``` lang=cpp, name=Nada
> var InterpolationType : PhysicsEffectInterpolationType


---  
 #  InwardStrengthAtMaxDistance : [real](../nada_base_types/real.md)

> The inward strength of the vortex at the max distance.
> ``` lang=cpp, name=Nada
> var InwardStrengthAtMaxDistance : Real


---  
 #  InwardStrengthAtMinDistance : [real](../nada_base_types/real.md)

> The inward strength of the vortex at the min distance.
> ``` lang=cpp, name=Nada
> var InwardStrengthAtMinDistance : Real


---  
 #  LocalAxis : [boolean](../nada_base_types/boolean.md)

> Determines if the vortex axis is in world or local space.
> ``` lang=cpp, name=Nada
> var LocalAxis : Boolean


---  
 #  MaxDistance : [real](../nada_base_types/real.md)

> The max distance that attenuation will happen at. If an object is between min and max distance, the value will be attenuated. If the object is further away, the effect strength will be determined by EndCondition.
> ``` lang=cpp, name=Nada
> var MaxDistance : Real


---  
 #  MinDistance : [real](../nada_base_types/real.md)

> The first distance at which attenuation will start. If an object is under the min distance, the min strength values will be used. If an object is in between min and max, then it will attenuate.
> ``` lang=cpp, name=Nada
> var MinDistance : Real


---  
 #  TwistStrengthAtMaxDistance : [real](../nada_base_types/real.md)

> The perpendicular strength (twist) of the vortex at max distance.
> ``` lang=cpp, name=Nada
> var TwistStrengthAtMaxDistance : Real


---  
 #  TwistStrengthAtMinDistance : [real](../nada_base_types/real.md)

> The perpendicular strength (twist) of the vortex at min distance.
> ``` lang=cpp, name=Nada
> var TwistStrengthAtMinDistance : Real


---  
 #  VortexAxis : [real3](../nada_base_types/real3.md)

> The axis the vortex spins about.
> ``` lang=cpp, name=Nada
> var VortexAxis : Real3


---  
 #  WorldVortexAxis : [real3](../nada_base_types/real3.md)

 `read-only`

> The axis the vortex spins about in world space.
> ``` lang=cpp, name=Nada
> var WorldVortexAxis : Real3


---  
 #  Methods


---  
 #  VortexEffect : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function VortexEffect()
> ``` 


---  
 

 
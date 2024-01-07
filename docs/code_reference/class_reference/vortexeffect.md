 `Component` `Physics`



(NOTE) Applies a force about an axis at the object's center. This will apply two forces to a body: One pulls the object towards the center of the vortex and the other applies a tangential force. Useful to model a vortex. This only expects to be used as a Region effect.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/vortexeffect.md#vortexeffect-void)|[ EndCondition](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/vortexeffect.md#endcondition-zilch-engine)|[physicseffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicseffect.md)| |
| |[ InterpolationType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/vortexeffect.md#interpolationtype-zilch-e)| | |
| |[ InwardStrengthAtMaxDistance](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/vortexeffect.md#inwardstrengthatmaxdista)| | |
| |[ InwardStrengthAtMinDistance](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/vortexeffect.md#inwardstrengthatmindista)| | |
| |[ LocalAxis](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/vortexeffect.md#localaxis-zilch-engine-do)| | |
| |[ MaxDistance](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/vortexeffect.md#maxdistance-zilch-engine)| | |
| |[ MinDistance](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/vortexeffect.md#mindistance-zilch-engine)| | |
| |[ TwistStrengthAtMaxDistance](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/vortexeffect.md#twiststrengthatmaxdistan)| | |
| |[ TwistStrengthAtMinDistance](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/vortexeffect.md#twiststrengthatmindistan)| | |
| |[ VortexAxis](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/vortexeffect.md#vortexaxis-zilch-engine-d)| | |
| |[ WorldVortexAxis](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/vortexeffect.md#worldvortexaxis-zilch-eng)| | |


 #  Properties


---  
 #  EndCondition : [PhysicsEffectEndCondition](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#physicseffectendcondition)

> How the interpolation should be handled at MaxDistance. ClampToMax will clamp to the max strength values. NoEffect will ignore the effect. ContinueFalloff will continue the interpolation (this may go negative).
> ``` lang=cpp, name=Nada
> var EndCondition : PhysicsEffectEndCondition


---  
 #  InterpolationType : [PhysicsEffectInterpolationType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#physicseffectinterpolationtype)

> The type of interpolation used (e.g. Linear, Quadratic) for the forces.
> ``` lang=cpp, name=Nada
> var InterpolationType : PhysicsEffectInterpolationType


---  
 #  InwardStrengthAtMaxDistance : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The inward strength of the vortex at the max distance.
> ``` lang=cpp, name=Nada
> var InwardStrengthAtMaxDistance : Real


---  
 #  InwardStrengthAtMinDistance : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The inward strength of the vortex at the min distance.
> ``` lang=cpp, name=Nada
> var InwardStrengthAtMinDistance : Real


---  
 #  LocalAxis : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Determines if the vortex axis is in world or local space.
> ``` lang=cpp, name=Nada
> var LocalAxis : Boolean


---  
 #  MaxDistance : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The max distance that attenuation will happen at. If an object is between min and max distance, the value will be attenuated. If the object is further away, the effect strength will be determined by EndCondition.
> ``` lang=cpp, name=Nada
> var MaxDistance : Real


---  
 #  MinDistance : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The first distance at which attenuation will start. If an object is under the min distance, the min strength values will be used. If an object is in between min and max, then it will attenuate.
> ``` lang=cpp, name=Nada
> var MinDistance : Real


---  
 #  TwistStrengthAtMaxDistance : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The perpendicular strength (twist) of the vortex at max distance.
> ``` lang=cpp, name=Nada
> var TwistStrengthAtMaxDistance : Real


---  
 #  TwistStrengthAtMinDistance : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The perpendicular strength (twist) of the vortex at min distance.
> ``` lang=cpp, name=Nada
> var TwistStrengthAtMinDistance : Real


---  
 #  VortexAxis : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The axis the vortex spins about.
> ``` lang=cpp, name=Nada
> var VortexAxis : Real3


---  
 #  WorldVortexAxis : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

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
 

 
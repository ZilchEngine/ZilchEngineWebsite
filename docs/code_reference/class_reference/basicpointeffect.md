 `Component` `Physics`



(NOTE) Common interface for all point effects. Used to attract or repel objects towards a central point. The strength of the effect is calculated as an interpolation between two strength values at two radial distances.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ EndCondition](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/basicpointeffect.md#endcondition-zilch-engine)|[physicseffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicseffect.md)|[pointforceeffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/pointforceeffect.md)|
| |[ InterpolationType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/basicpointeffect.md#interpolationtype-zilch-e)| |[pointgravityeffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/pointgravityeffect.md)|
| |[ LocalPositionOffset](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/basicpointeffect.md#localpositionoffset-zero)| | |
| |[ MaxDistance](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/basicpointeffect.md#maxdistance-zilch-engine)| | |
| |[ MinDistance](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/basicpointeffect.md#mindistance-zilch-engine)| | |
| |[ StrengthAtMax](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/basicpointeffect.md#strengthatmax-zilch-engin)| | |
| |[ StrengthAtMin](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/basicpointeffect.md#strengthatmin-zilch-engin)| | |


 #  Properties


---  
 #  EndCondition : [PhysicsEffectEndCondition](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#physicseffectendcondition)

> How the interpolation should be handled after max distance. ClampToMax will clamp to StrengthAtMax. NoEffect will ignore the effect. ContinueFalloff will continue the interpolation (this may go negative).
> ``` lang=cpp, name=Nada
> var EndCondition : PhysicsEffectEndCondition


---  
 #  InterpolationType : [PhysicsEffectInterpolationType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#physicseffectinterpolationtype)

> The type of interpolation used (e.g. Linear, Quadratic) for the effect.
> ``` lang=cpp, name=Nada
> var InterpolationType : PhysicsEffectInterpolationType


---  
 #  LocalPositionOffset : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The offset from the transform position (in local space) that the point effect will be applied at.
> ``` lang=cpp, name=Nada
> var LocalPositionOffset : Real3


---  
 #  MaxDistance : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The max distance that attenuation will happen at. If an object is between min and max distance, the value will be attenuated. If the object is further away, the effect strength will be determined by EndCondition.
> ``` lang=cpp, name=Nada
> var MaxDistance : Real


---  
 #  MinDistance : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The first distance at which attenuation will start. If an object is under the min distance, StrengthAtMin will be used. If an object is in between min and max, then it will attenuate.
> ``` lang=cpp, name=Nada
> var MinDistance : Real


---  
 #  StrengthAtMax : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The strength that this effect applies at the max distance.
> ``` lang=cpp, name=Nada
> var StrengthAtMax : Real


---  
 #  StrengthAtMin : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The strength that this effect applies at the min distance.
> ``` lang=cpp, name=Nada
> var StrengthAtMin : Real


---  
 #  Methods


---  
 

 
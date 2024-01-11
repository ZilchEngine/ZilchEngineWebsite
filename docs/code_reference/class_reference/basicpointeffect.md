 `Component` `Physics`



(NOTE) Common interface for all point effects. Used to attract or repel objects towards a central point. The strength of the effect is calculated as an interpolation between two strength values at two radial distances.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ EndCondition](basicpointeffect.md#endcondition-zilch-engine)|[physicseffect](physicseffect.md)|[pointforceeffect](pointforceeffect.md)|
| |[ InterpolationType](basicpointeffect.md#interpolationtype-zilch-e)| |[pointgravityeffect](pointgravityeffect.md)|
| |[ LocalPositionOffset](basicpointeffect.md#localpositionoffset-zero)| | |
| |[ MaxDistance](basicpointeffect.md#maxdistance-zilch-engine)| | |
| |[ MinDistance](basicpointeffect.md#mindistance-zilch-engine)| | |
| |[ StrengthAtMax](basicpointeffect.md#strengthatmax-zilch-engin)| | |
| |[ StrengthAtMin](basicpointeffect.md#strengthatmin-zilch-engin)| | |


 #  Properties


---  
 #  EndCondition : [PhysicsEffectEndCondition](../enum_reference.md#physicseffectendcondition)

> How the interpolation should be handled after max distance. ClampToMax will clamp to StrengthAtMax. NoEffect will ignore the effect. ContinueFalloff will continue the interpolation (this may go negative).
> ```TS:Nada
> var EndCondition : PhysicsEffectEndCondition


---  
 #  InterpolationType : [PhysicsEffectInterpolationType](../enum_reference.md#physicseffectinterpolationtype)

> The type of interpolation used (e.g. Linear, Quadratic) for the effect.
> ```TS:Nada
> var InterpolationType : PhysicsEffectInterpolationType


---  
 #  LocalPositionOffset : [real3](../nada_base_types/real3.md)

> The offset from the transform position (in local space) that the point effect will be applied at.
> ```TS:Nada
> var LocalPositionOffset : Real3


---  
 #  MaxDistance : [real](../nada_base_types/real.md)

> The max distance that attenuation will happen at. If an object is between min and max distance, the value will be attenuated. If the object is further away, the effect strength will be determined by EndCondition.
> ```TS:Nada
> var MaxDistance : Real


---  
 #  MinDistance : [real](../nada_base_types/real.md)

> The first distance at which attenuation will start. If an object is under the min distance, StrengthAtMin will be used. If an object is in between min and max, then it will attenuate.
> ```TS:Nada
> var MinDistance : Real


---  
 #  StrengthAtMax : [real](../nada_base_types/real.md)

> The strength that this effect applies at the max distance.
> ```TS:Nada
> var StrengthAtMax : Real


---  
 #  StrengthAtMin : [real](../nada_base_types/real.md)

> The strength that this effect applies at the min distance.
> ```TS:Nada
> var StrengthAtMin : Real


---  
 #  Methods


---  
 

 
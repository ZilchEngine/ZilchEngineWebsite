 `Component` `Physics`



(NOTE) A common interface for all effects in physics. An effect is something that typically applies a force and can be attached to a collider, rigid body, region, or even a space. This effect is applied every frame according to the rules of the object it is attached to.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Toggle](physicseffect.md#toggle-void)|[ Active](physicseffect.md#active-zilch-engine-docum)|[component](component.md)|[basicdirectioneffect](basicdirectioneffect.md)|
| |[ DebugDrawEffect](physicseffect.md#debugdraweffect-zilch-eng)| |[basicpointeffect](basicpointeffect.md)|
| |[ EffectType](physicseffect.md#effecttype-zilch-engine-d)| |[buoyancyeffect](buoyancyeffect.md)|
| |[ WakeUpOnChange](physicseffect.md#wakeuponchange-zilch-engi)| |[customphysicseffect](customphysicseffect.md)|
| | | |[drageffect](drageffect.md)|
| | | |[floweffect](floweffect.md)|
| | | |[thrusteffect](thrusteffect.md)|
| | | |[torqueeffect](torqueeffect.md)|
| | | |[vortexeffect](vortexeffect.md)|
| | | |[windeffect](windeffect.md)|


 #  Properties


---  
 #  Active : [boolean](../nada_base_types/boolean.md)

> Enable/disable this effect.
> ```TS:Nada
> var Active : Boolean


---  
 #  DebugDrawEffect : [boolean](../nada_base_types/boolean.md)

> Should the effect debug draw.
> ```TS:Nada
> var DebugDrawEffect : Boolean


---  
 #  EffectType : [PhysicsEffectType](../enum_reference.md#physicseffecttype)

 `read-only`

> What kind of effect this is (e.g. ForceEffect, GravityEffect, etc...).
> ```TS:Nada
> var EffectType : PhysicsEffectType


---  
 #  WakeUpOnChange : [boolean](../nada_base_types/boolean.md)

> Whether the object associated with this is woken up when any property is changed.
> ```TS:Nada
> var WakeUpOnChange : Boolean


---  
 #  Methods


---  
 #  Toggle : Void

> Toggles whether or not this effect is active.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Toggle()
> ``` 


---  
 

 
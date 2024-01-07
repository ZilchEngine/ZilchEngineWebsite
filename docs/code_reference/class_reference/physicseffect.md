 `Component` `Physics`



(NOTE) A common interface for all effects in physics. An effect is something that typically applies a force and can be attached to a collider, rigid body, region, or even a space. This effect is applied every frame according to the rules of the object it is attached to.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Toggle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicseffect.md#toggle-void)|[ Active](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicseffect.md#active-zilch-engine-docum)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)|[basicdirectioneffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/basicdirectioneffect.md)|
| |[ DebugDrawEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicseffect.md#debugdraweffect-zilch-eng)| |[basicpointeffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/basicpointeffect.md)|
| |[ EffectType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicseffect.md#effecttype-zilch-engine-d)| |[buoyancyeffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/buoyancyeffect.md)|
| |[ WakeUpOnChange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicseffect.md#wakeuponchange-zilch-engi)| |[customphysicseffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customphysicseffect.md)|
| | | |[drageffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/drageffect.md)|
| | | |[floweffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/floweffect.md)|
| | | |[thrusteffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/thrusteffect.md)|
| | | |[torqueeffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/torqueeffect.md)|
| | | |[vortexeffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/vortexeffect.md)|
| | | |[windeffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/windeffect.md)|


 #  Properties


---  
 #  Active : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Enable/disable this effect.
> ``` lang=cpp, name=Nada
> var Active : Boolean


---  
 #  DebugDrawEffect : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Should the effect debug draw.
> ``` lang=cpp, name=Nada
> var DebugDrawEffect : Boolean


---  
 #  EffectType : [PhysicsEffectType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#physicseffecttype)

 `read-only`

> What kind of effect this is (e.g. ForceEffect, GravityEffect, etc...).
> ``` lang=cpp, name=Nada
> var EffectType : PhysicsEffectType


---  
 #  WakeUpOnChange : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Whether the object associated with this is woken up when any property is changed.
> ``` lang=cpp, name=Nada
> var WakeUpOnChange : Boolean


---  
 #  Methods


---  
 #  Toggle : Void

> Toggles whether or not this effect is active.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Toggle()
> ``` 


---  
 

 
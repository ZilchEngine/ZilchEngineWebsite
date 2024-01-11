 `Component` `Physics`



(NOTE) Allows a cog to ignore certain effect types (such as gravity or drag) that are being applied to the entire space (effects on Space or LevelSettings).

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetIgnoreState](ignorespaceeffects.md#getignorestate-zilch-engi)|[ IgnoreBuoyancy](ignorespaceeffects.md#ignorebuoyancy-zilch-engi)|[component](component.md)| |
|[ Constructor](ignorespaceeffects.md#ignorespaceeffects-void)|[ IgnoreCustom](ignorespaceeffects.md#ignorecustom-zilch-engine)| | |
|[ SetIgnoreState](ignorespaceeffects.md#setignorestate-void)|[ IgnoreDrag](ignorespaceeffects.md#ignoredrag-zilch-engine-d)| | |
| |[ IgnoreFlow](ignorespaceeffects.md#ignoreflow-zilch-engine-d)| | |
| |[ IgnoreForce](ignorespaceeffects.md#ignoreforce-zilch-engine)| | |
| |[ IgnoreGravity](ignorespaceeffects.md#ignoregravity-zilch-engin)| | |
| |[ IgnorePointForce](ignorespaceeffects.md#ignorepointforce-zilch-en)| | |
| |[ IgnorePointGravity](ignorespaceeffects.md#ignorepointgravity-zero)| | |
| |[ IgnoreThrust](ignorespaceeffects.md#ignorethrust-zilch-engine)| | |
| |[ IgnoreTorque](ignorespaceeffects.md#ignoretorque-zilch-engine)| | |
| |[ IgnoreVortex](ignorespaceeffects.md#ignorevortex-zilch-engine)| | |
| |[ IgnoreWind](ignorespaceeffects.md#ignorewind-zilch-engine-d)| | |


 #  Properties


---  
 #  IgnoreBuoyancy : [boolean](../nada_base_types/boolean.md)

> Whether or not to ignore buoyancy effects.
> ```TS:Nada
> var IgnoreBuoyancy : Boolean


---  
 #  IgnoreCustom : [boolean](../nada_base_types/boolean.md)

> Whether or not to ignore custom effects.
> ```TS:Nada
> var IgnoreCustom : Boolean


---  
 #  IgnoreDrag : [boolean](../nada_base_types/boolean.md)

> Whether or not to ignore drag effects.
> ```TS:Nada
> var IgnoreDrag : Boolean


---  
 #  IgnoreFlow : [boolean](../nada_base_types/boolean.md)

> Whether or not to ignore flow effects.
> ```TS:Nada
> var IgnoreFlow : Boolean


---  
 #  IgnoreForce : [boolean](../nada_base_types/boolean.md)

> Whether or not to ignore force effects.
> ```TS:Nada
> var IgnoreForce : Boolean


---  
 #  IgnoreGravity : [boolean](../nada_base_types/boolean.md)

> Whether or not to ignore gravity effects.
> ```TS:Nada
> var IgnoreGravity : Boolean


---  
 #  IgnorePointForce : [boolean](../nada_base_types/boolean.md)

> Whether or not to ignore point force effects.
> ```TS:Nada
> var IgnorePointForce : Boolean


---  
 #  IgnorePointGravity : [boolean](../nada_base_types/boolean.md)

> Whether or not to ignore point gravity effects.
> ```TS:Nada
> var IgnorePointGravity : Boolean


---  
 #  IgnoreThrust : [boolean](../nada_base_types/boolean.md)

> Whether or not to ignore thrust effects.
> ```TS:Nada
> var IgnoreThrust : Boolean


---  
 #  IgnoreTorque : [boolean](../nada_base_types/boolean.md)

> Whether or not to ignore torque effects.
> ```TS:Nada
> var IgnoreTorque : Boolean


---  
 #  IgnoreVortex : [boolean](../nada_base_types/boolean.md)

> Whether or not to ignore vortex effects.
> ```TS:Nada
> var IgnoreVortex : Boolean


---  
 #  IgnoreWind : [boolean](../nada_base_types/boolean.md)

> Whether or not to ignore wind effects.
> ```TS:Nada
> var IgnoreWind : Boolean


---  
 #  Methods


---  
 #  GetIgnoreState : [boolean](../nada_base_types/boolean.md)

> Should the given effect type be ignored?
> |Name|Type|Description|
> |---|---|---|
> |effectType|[PhysicsEffectType](../enum_reference.md#physicseffecttype)| |
> ```TS:Nada
> function GetIgnoreState(effectType : PhysicsEffectType) : Boolean
> ``` 


---  
 #  IgnoreSpaceEffects : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function IgnoreSpaceEffects()
> ``` 


---  
 #  SetIgnoreState : Void

> Set if an effect type should be ignored.
> |Name|Type|Description|
> |---|---|---|
> |effectType|[PhysicsEffectType](../enum_reference.md#physicseffecttype)| |
> |ignore|[boolean](../nada_base_types/boolean.md)| |
> ```TS:Nada
> function SetIgnoreState(effectType : PhysicsEffectType, ignore : Boolean)
> ``` 


---  
 

 
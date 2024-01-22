 `Event` `Physics`



(NOTE) Event data for applying custom physics effects.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](customphysicseffectevent.md#customphysicseffectevent)|[Dt](customphysicseffectevent.md#dt-zilch-engine-documenta)|[event](event.md)| |
| |[Effect](customphysicseffectevent.md#effect-zilch-engine-docum)| | |
| |[RigidBody](customphysicseffectevent.md#rigidbody-zilch-engine-do)| | |


 #  Properties


---  
 #  Dt : [real](../nada_base_types/real.md)

> The timestep of the current physics frame (in seconds).
> ```TS:Nada
> var Dt : Real


---  
 #  Effect : [customphysicseffect](customphysicseffect.md)

> The effect that sent out this event.
> ```TS:Nada
> var Effect : CustomPhysicsEffect


---  
 #  RigidBody : [rigidbody](rigidbody.md)

> The RigidBody to apply forces to.
> ```TS:Nada
> var RigidBody : RigidBody


---  
 #  Methods


---  
 #  CustomPhysicsEffectEvent : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function CustomPhysicsEffectEvent()
> ``` 


---  
 

 
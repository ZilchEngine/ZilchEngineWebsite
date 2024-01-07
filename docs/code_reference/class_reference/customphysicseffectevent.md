 `Event` `Physics`



(NOTE) Event data for applying custom physics effects.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customphysicseffectevent.md#customphysicseffectevent)|[ Dt](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customphysicseffectevent.md#dt-zilch-engine-documenta)|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
| |[ Effect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customphysicseffectevent.md#effect-zilch-engine-docum)| | |
| |[ RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customphysicseffectevent.md#rigidbody-zilch-engine-do)| | |


 #  Properties


---  
 #  Dt : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The timestep of the current physics frame (in seconds).
> ``` lang=cpp, name=Nada
> var Dt : Real


---  
 #  Effect : [customphysicseffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customphysicseffect.md)

> The effect that sent out this event.
> ``` lang=cpp, name=Nada
> var Effect : CustomPhysicsEffect


---  
 #  RigidBody : [rigidbody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)

> The RigidBody to apply forces to.
> ``` lang=cpp, name=Nada
> var RigidBody : RigidBody


---  
 #  Methods


---  
 #  CustomPhysicsEffectEvent : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function CustomPhysicsEffectEvent()
> ``` 


---  
 

 
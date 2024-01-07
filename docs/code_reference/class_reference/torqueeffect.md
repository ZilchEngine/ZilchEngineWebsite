 `Component` `Physics`



(NOTE) Applies a torque to the center of mass of a body.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/torqueeffect.md#torqueeffect-void)|[ LocalTorque](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/torqueeffect.md#localtorque-zilch-engine)|[physicseffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicseffect.md)| |
| |[ TorqueAxis](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/torqueeffect.md#torqueaxis-zilch-engine-d)| | |
| |[ TorqueStrength](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/torqueeffect.md#torquestrength-zilch-engi)| | |
| |[ WorldTorqueAxis](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/torqueeffect.md#worldtorqueaxis-zilch-eng)| | |


 #  Properties


---  
 #  LocalTorque : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Determines if the torque is applied in local or world space.
> ``` lang=cpp, name=Nada
> var LocalTorque : Boolean


---  
 #  TorqueAxis : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The axis that the torque is being applied about.
> ``` lang=cpp, name=Nada
> var TorqueAxis : Real3


---  
 #  TorqueStrength : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The strength of the torque being applied.
> ``` lang=cpp, name=Nada
> var TorqueStrength : Real


---  
 #  WorldTorqueAxis : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

 `read-only`

> The axis of the torque in world space (can be used to manually add torque to a RigidBody).
> ``` lang=cpp, name=Nada
> var WorldTorqueAxis : Real3


---  
 #  Methods


---  
 #  TorqueEffect : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function TorqueEffect()
> ``` 


---  
 

 
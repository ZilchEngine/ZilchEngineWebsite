 `Component` `Physics`



(NOTE) Applies a torque to the center of mass of a body.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](torqueeffect.md#torqueeffect-void)|[LocalTorque](torqueeffect.md#localtorque-zilch-engine)|[physicseffect](physicseffect.md)| |
| |[TorqueAxis](torqueeffect.md#torqueaxis-zilch-engine-d)| | |
| |[TorqueStrength](torqueeffect.md#torquestrength-zilch-engi)| | |
| |[WorldTorqueAxis](torqueeffect.md#worldtorqueaxis-zilch-eng)| | |


 #  Properties


---  
 #  LocalTorque : [boolean](../nada_base_types/boolean.md)

> Determines if the torque is applied in local or world space.
> ```TS:Nada
> var LocalTorque : Boolean


---  
 #  TorqueAxis : [real3](../nada_base_types/real3.md)

> The axis that the torque is being applied about.
> ```TS:Nada
> var TorqueAxis : Real3


---  
 #  TorqueStrength : [real](../nada_base_types/real.md)

> The strength of the torque being applied.
> ```TS:Nada
> var TorqueStrength : Real


---  
 #  WorldTorqueAxis : [real3](../nada_base_types/real3.md)

 `read-only`

> The axis of the torque in world space (can be used to manually add torque to a RigidBody).
> ```TS:Nada
> var WorldTorqueAxis : Real3


---  
 #  Methods


---  
 #  TorqueEffect : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function TorqueEffect()
> ``` 


---  
 

 
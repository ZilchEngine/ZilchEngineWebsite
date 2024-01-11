 `Component` `Physics`



(NOTE) Applies a force to make an object move at a target speed in a given direction. This can also be used to pull the object towards the center of the flow (the axis in the flow direction centered at the effect). Used to model a river or a tractor beam.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](floweffect.md#floweffect-void)|[ AttractSpeed](floweffect.md#attractspeed-zilch-engine)|[physicseffect](physicseffect.md)| |
| |[ AttractToFlowCenter](floweffect.md#attracttoflowcenter-zero)| | |
| |[ FlowDirection](floweffect.md#flowdirection-zilch-engin)| | |
| |[ FlowSpeed](floweffect.md#flowspeed-zilch-engine-do)| | |
| |[ LocalForce](floweffect.md#localforce-zilch-engine-d)| | |
| |[ MaxAttractForce](floweffect.md#maxattractforce-zilch-eng)| | |
| |[ MaxFlowForce](floweffect.md#maxflowforce-zilch-engine)| | |
| |[ WorldFlowDirection](floweffect.md#worldflowdirection-zero)| | |


 #  Properties


---  
 #  AttractSpeed : [real](../nada_base_types/real.md)

> The target speed for an object to be pulled towards the center of the flow.
> ``` lang=cpp, name=Nada
> var AttractSpeed : Real


---  
 #  AttractToFlowCenter : [boolean](../nada_base_types/boolean.md)

> Determines if the flow field will attract objects towards the center of the field. This can be used to create a tractor beam effect that will keep the object inside of the flow field.
> ``` lang=cpp, name=Nada
> var AttractToFlowCenter : Boolean


---  
 #  FlowDirection : [real3](../nada_base_types/real3.md)

> The direction that the field is flowing. This can be defined in world or local space.
> ``` lang=cpp, name=Nada
> var FlowDirection : Real3


---  
 #  FlowSpeed : [real](../nada_base_types/real.md)

> The target speed of objects in the flow field.
> ``` lang=cpp, name=Nada
> var FlowSpeed : Real


---  
 #  LocalForce : [boolean](../nada_base_types/boolean.md)

> Determines if the flow direction is in the local space of the object.
> ``` lang=cpp, name=Nada
> var LocalForce : Boolean


---  
 #  MaxAttractForce : [real](../nada_base_types/real.md)

> The max force that can be used to reach the target attract speed.
> ``` lang=cpp, name=Nada
> var MaxAttractForce : Real


---  
 #  MaxFlowForce : [real](../nada_base_types/real.md)

> The max force that can be used to reach the target flow speed.
> ``` lang=cpp, name=Nada
> var MaxFlowForce : Real


---  
 #  WorldFlowDirection : [real3](../nada_base_types/real3.md)

 `read-only`

> The direction that the field is flowing in world space.
> ``` lang=cpp, name=Nada
> var WorldFlowDirection : Real3


---  
 #  Methods


---  
 #  FlowEffect : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function FlowEffect()
> ``` 


---  
 

 
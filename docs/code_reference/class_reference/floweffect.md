 `Component` `Physics`



(NOTE) Applies a force to make an object move at a target speed in a given direction. This can also be used to pull the object towards the center of the flow (the axis in the flow direction centered at the effect). Used to model a river or a tractor beam.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/floweffect.md#floweffect-void)|[ AttractSpeed](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/floweffect.md#attractspeed-zilch-engine)|[physicseffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicseffect.md)| |
| |[ AttractToFlowCenter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/floweffect.md#attracttoflowcenter-zero)| | |
| |[ FlowDirection](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/floweffect.md#flowdirection-zilch-engin)| | |
| |[ FlowSpeed](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/floweffect.md#flowspeed-zilch-engine-do)| | |
| |[ LocalForce](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/floweffect.md#localforce-zilch-engine-d)| | |
| |[ MaxAttractForce](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/floweffect.md#maxattractforce-zilch-eng)| | |
| |[ MaxFlowForce](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/floweffect.md#maxflowforce-zilch-engine)| | |
| |[ WorldFlowDirection](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/floweffect.md#worldflowdirection-zero)| | |


 #  Properties


---  
 #  AttractSpeed : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The target speed for an object to be pulled towards the center of the flow.
> ``` lang=cpp, name=Nada
> var AttractSpeed : Real


---  
 #  AttractToFlowCenter : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Determines if the flow field will attract objects towards the center of the field. This can be used to create a tractor beam effect that will keep the object inside of the flow field.
> ``` lang=cpp, name=Nada
> var AttractToFlowCenter : Boolean


---  
 #  FlowDirection : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The direction that the field is flowing. This can be defined in world or local space.
> ``` lang=cpp, name=Nada
> var FlowDirection : Real3


---  
 #  FlowSpeed : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The target speed of objects in the flow field.
> ``` lang=cpp, name=Nada
> var FlowSpeed : Real


---  
 #  LocalForce : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Determines if the flow direction is in the local space of the object.
> ``` lang=cpp, name=Nada
> var LocalForce : Boolean


---  
 #  MaxAttractForce : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The max force that can be used to reach the target attract speed.
> ``` lang=cpp, name=Nada
> var MaxAttractForce : Real


---  
 #  MaxFlowForce : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The max force that can be used to reach the target flow speed.
> ``` lang=cpp, name=Nada
> var MaxFlowForce : Real


---  
 #  WorldFlowDirection : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

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
 

 
 `Component` `Physics`



(NOTE) Applies a buoyancy force to an object in a given direction.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/buoyancyeffect.md#buoyancyeffect-void)|[ DebugDrawRuntime](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/buoyancyeffect.md#debugdrawruntime-zilch-en)|[physicseffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicseffect.md)| |
| |[ Density](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/buoyancyeffect.md#density-zilch-engine-docu)| | |
| |[ Detail](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/buoyancyeffect.md#detail-zilch-engine-docum)| | |
| |[ Gravity](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/buoyancyeffect.md#gravity-zilch-engine-docu)| | |


 #  Properties


---  
 #  DebugDrawRuntime : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Draw the points used to compute the buoyancy during run-time. This helps in debugging, but should be left off during normal run.
> ``` lang=cpp, name=Nada
> var DebugDrawRuntime : Boolean


---  
 #  Density : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The density of the fluid.
> ``` lang=cpp, name=Nada
> var Density : Real


---  
 #  Detail : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> The amount of points to subdivide each object into for sampling (total points is Detail^3)
> ``` lang=cpp, name=Nada
> var Detail : Integer


---  
 #  Gravity : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The direction of gravity in world-space.
> ``` lang=cpp, name=Nada
> var Gravity : Real3


---  
 #  Methods


---  
 #  BuoyancyEffect : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function BuoyancyEffect()
> ``` 


---  
 

 
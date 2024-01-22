 `Component` `Physics`



(NOTE) Applies a buoyancy force to an object in a given direction.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](buoyancyeffect.md#buoyancyeffect-void)|[DebugDrawRuntime](buoyancyeffect.md#debugdrawruntime-zilch-en)|[physicseffect](physicseffect.md)| |
| |[Density](buoyancyeffect.md#density-zilch-engine-docu)| | |
| |[Detail](buoyancyeffect.md#detail-zilch-engine-docum)| | |
| |[Gravity](buoyancyeffect.md#gravity-zilch-engine-docu)| | |


 #  Properties


---  
 #  DebugDrawRuntime : [boolean](../nada_base_types/boolean.md)

> Draw the points used to compute the buoyancy during run-time. This helps in debugging, but should be left off during normal run.
> ```TS:Nada
> var DebugDrawRuntime : Boolean


---  
 #  Density : [real](../nada_base_types/real.md)

> The density of the fluid.
> ```TS:Nada
> var Density : Real


---  
 #  Detail : [integer](../nada_base_types/integer.md)

> The amount of points to subdivide each object into for sampling (total points is Detail^3)
> ```TS:Nada
> var Detail : Integer


---  
 #  Gravity : [real3](../nada_base_types/real3.md)

> The direction of gravity in world-space.
> ```TS:Nada
> var Gravity : Real3


---  
 #  Methods


---  
 #  BuoyancyEffect : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function BuoyancyEffect()
> ``` 


---  
 

 
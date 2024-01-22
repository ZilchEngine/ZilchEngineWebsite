 `Component` `Physics`



(NOTE) Applies a wind force in a given direction. The wind force is calculated from the squared wind speed and is scaled by the approximate surface area of the object in the direction of the force.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](windeffect.md#windeffect-void)|[LocalSpaceDirection](windeffect.md#localspacedirection-zero)|[physicseffect](physicseffect.md)| |
| |[WindDirection](windeffect.md#winddirection-zilch-engin)| | |
| |[WindSpeed](windeffect.md#windspeed-zilch-engine-do)| | |
| |[WorldWindDirection](windeffect.md#worldwinddirection-zero)| | |


 #  Properties


---  
 #  LocalSpaceDirection : [boolean](../nada_base_types/boolean.md)

> Determines if the wind's direction is a local or world-space vector.
> ```TS:Nada
> var LocalSpaceDirection : Boolean


---  
 #  WindDirection : [real3](../nada_base_types/real3.md)

> The direction that the wind is blowing.
> ```TS:Nada
> var WindDirection : Real3


---  
 #  WindSpeed : [real](../nada_base_types/real.md)

> The speed that the wind is blowing.
> ```TS:Nada
> var WindSpeed : Real


---  
 #  WorldWindDirection : [real3](../nada_base_types/real3.md)

 `read-only`

> The direction of the wind in world space.
> ```TS:Nada
> var WorldWindDirection : Real3


---  
 #  Methods


---  
 #  WindEffect : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function WindEffect()
> ``` 


---  
 

 
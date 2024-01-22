 `Component` `Physics`



(NOTE) Represents a ball and socket joint. A position joint constrains the two anchor points on each object to be equal. Limits, motors, and springs typically should not be used. Add on definitions: Limit: A limit will provide a min/max translation on every axis (x,y,z) that the objects must be between. Motor: A motor will attempt to drive the translation in the positive direction on every axis. Spring: A spring will make the translation on every axis springy at the bounds.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](positionjoint.md#positionjoint-void)|[LocalPointA](positionjoint.md#localpointa-zilch-engine)|[joint](joint.md)| |
|[SetWorldPoints](positionjoint.md#setworldpoints-void)|[LocalPointB](positionjoint.md#localpointb-zilch-engine)| | |
| |[WorldPointA](positionjoint.md#worldpointa-zilch-engine)| | |
| |[WorldPointB](positionjoint.md#worldpointb-zilch-engine)| | |


 #  Properties


---  
 #  LocalPointA : [real3](../nada_base_types/real3.md)

> The local point of the anchor on object A . 
> ```TS:Nada
> var LocalPointA : Real3


---  
 #  LocalPointB : [real3](../nada_base_types/real3.md)

> The local point of the anchor on object B . 
> ```TS:Nada
> var LocalPointB : Real3


---  
 #  WorldPointA : [real3](../nada_base_types/real3.md)

> The position of the anchor on object A given a position in world space 
> ```TS:Nada
> var WorldPointA : Real3


---  
 #  WorldPointB : [real3](../nada_base_types/real3.md)

> The position of the anchor on object B given a position in world space 
> ```TS:Nada
> var WorldPointB : Real3


---  
 #  Methods


---  
 #  PositionJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function PositionJoint()
> ``` 


---  
 #  SetWorldPoints : Void

> Sets the position of the anchor on object A and B given a position in world space 
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function SetWorldPoints(point : Real3)
> ``` 


---  
 

 
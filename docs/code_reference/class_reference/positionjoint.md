 `Component` `Physics`



(NOTE) Represents a ball and socket joint. A position joint constrains the two anchor points on each object to be equal. Limits, motors, and springs typically should not be used. Add on definitions: Limit: A limit will provide a min/max translation on every axis (x,y,z) that the objects must be between. Motor: A motor will attempt to drive the translation in the positive direction on every axis. Spring: A spring will make the translation on every axis springy at the bounds.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/positionjoint.md#positionjoint-void)|[ LocalPointA](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/positionjoint.md#localpointa-zilch-engine)|[joint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/joint.md)| |
|[ SetWorldPoints](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/positionjoint.md#setworldpoints-void)|[ LocalPointB](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/positionjoint.md#localpointb-zilch-engine)| | |
| |[ WorldPointA](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/positionjoint.md#worldpointa-zilch-engine)| | |
| |[ WorldPointB](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/positionjoint.md#worldpointb-zilch-engine)| | |


 #  Properties


---  
 #  LocalPointA : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The local point of the anchor on object A . 
> ``` lang=cpp, name=Nada
> var LocalPointA : Real3


---  
 #  LocalPointB : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The local point of the anchor on object B . 
> ``` lang=cpp, name=Nada
> var LocalPointB : Real3


---  
 #  WorldPointA : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The position of the anchor on object A given a position in world space 
> ``` lang=cpp, name=Nada
> var WorldPointA : Real3


---  
 #  WorldPointB : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The position of the anchor on object B given a position in world space 
> ``` lang=cpp, name=Nada
> var WorldPointB : Real3


---  
 #  Methods


---  
 #  PositionJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function PositionJoint()
> ``` 


---  
 #  SetWorldPoints : Void

> Sets the position of the anchor on object A and B given a position in world space 
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function SetWorldPoints(point : Real3)
> ``` 


---  
 

 
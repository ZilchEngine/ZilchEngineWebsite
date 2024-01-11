 `Component` `Physics`



(NOTE) A revolute joint is used to create a wheel or a hinge. This is the 2d version of RevoluteJoint. This joint is used in 2d mode for increased performance and stability. The motor axis is automatically set to the z axis, as that is the only axis objects can rotate about. Also, the translation on the z axis is ignored so that objects can be arbitrarily far apart. Add on definitions: Limit: A limit will provide a min/max angle on the motor axis. Motor: A motor will turn the objects about the motor axis. Spring: A spring will make the motor axis springy at the limits.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](revolutejoint2d.md#revolutejoint2d-void)|[ LocalPointA](revolutejoint2d.md#localpointa-zilch-engine)|[joint](joint.md)| |
|[ SetWorldPoints](revolutejoint2d.md#setworldpoints-void)|[ LocalPointB](revolutejoint2d.md#localpointb-zilch-engine)| | |
| |[ WorldPointA](revolutejoint2d.md#worldpointa-zilch-engine)| | |
| |[ WorldPointB](revolutejoint2d.md#worldpointb-zilch-engine)| | |


 #  Properties


---  
 #  LocalPointA : [real3](../nada_base_types/real3.md)

> The local point of the anchor on object A . 
> ``` lang=cpp, name=Nada
> var LocalPointA : Real3


---  
 #  LocalPointB : [real3](../nada_base_types/real3.md)

> The local point of the anchor on object B . 
> ``` lang=cpp, name=Nada
> var LocalPointB : Real3


---  
 #  WorldPointA : [real3](../nada_base_types/real3.md)

> The position of the anchor on object A given a position in world space 
> ``` lang=cpp, name=Nada
> var WorldPointA : Real3


---  
 #  WorldPointB : [real3](../nada_base_types/real3.md)

> The position of the anchor on object B given a position in world space 
> ``` lang=cpp, name=Nada
> var WorldPointB : Real3


---  
 #  Methods


---  
 #  RevoluteJoint2d : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function RevoluteJoint2d()
> ``` 


---  
 #  SetWorldPoints : Void

> Sets the position of the anchor on object A and B given a position in world space 
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](../nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function SetWorldPoints(point : Real3)
> ``` 


---  
 

 
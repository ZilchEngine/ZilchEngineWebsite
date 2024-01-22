 `Component` `Physics`



(NOTE) A universal joint locks positional movement of two points together as well as locking rotation about one axis. This means it is a joint that constrains four axes and leaves two free rotational axes. This joint is most useful to model something like a arm or leg that has a large range of rotational movement.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[SetWorldPoints](universaljoint.md#setworldpoints-void)|[LocalAxis0OfBodyA](universaljoint.md#localaxis0ofbodya-zilch-e)|[joint](joint.md)| |
|[Constructor](universaljoint.md#universaljoint-void)|[LocalAxis0OfBodyB](universaljoint.md#localaxis0ofbodyb-zilch-e)| | |
| |[LocalAxis1OfBodyA](universaljoint.md#localaxis1ofbodya-zilch-e)| | |
| |[LocalAxis1OfBodyB](universaljoint.md#localaxis1ofbodyb-zilch-e)| | |
| |[LocalPointA](universaljoint.md#localpointa-zilch-engine)| | |
| |[LocalPointB](universaljoint.md#localpointb-zilch-engine)| | |
| |[WorldPointA](universaljoint.md#worldpointa-zilch-engine)| | |
| |[WorldPointB](universaljoint.md#worldpointb-zilch-engine)| | |


 #  Properties


---  
 #  LocalAxis0OfBodyA : [real3](../nada_base_types/real3.md)

> One of the two axes in local space of object A that the objects are allowed to rotate about.
> ```TS:Nada
> var LocalAxis0OfBodyA : Real3


---  
 #  LocalAxis0OfBodyB : [real3](../nada_base_types/real3.md)

> One of the two axes in local space of object B that the objects are allowed to rotate about.
> ```TS:Nada
> var LocalAxis0OfBodyB : Real3


---  
 #  LocalAxis1OfBodyA : [real3](../nada_base_types/real3.md)

> One of the two axes in local space of object A that the objects are allowed to rotate about.
> ```TS:Nada
> var LocalAxis1OfBodyA : Real3


---  
 #  LocalAxis1OfBodyB : [real3](../nada_base_types/real3.md)

> One of the two axes in local space of object B that the objects are allowed to rotate about.
> ```TS:Nada
> var LocalAxis1OfBodyB : Real3


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
 #  SetWorldPoints : Void

> Sets the position of the anchor on object A and B given a position in world space 
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function SetWorldPoints(point : Real3)
> ``` 


---  
 #  UniversalJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function UniversalJoint()
> ``` 


---  
 

 
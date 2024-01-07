 `Component` `Physics`



(NOTE) A universal joint locks positional movement of two points together as well as locking rotation about one axis. This means it is a joint that constrains four axes and leaves two free rotational axes. This joint is most useful to model something like a arm or leg that has a large range of rotational movement.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ SetWorldPoints](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/universaljoint.md#setworldpoints-void)|[ LocalAxis0OfBodyA](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/universaljoint.md#localaxis0ofbodya-zilch-e)|[joint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/joint.md)| |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/universaljoint.md#universaljoint-void)|[ LocalAxis0OfBodyB](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/universaljoint.md#localaxis0ofbodyb-zilch-e)| | |
| |[ LocalAxis1OfBodyA](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/universaljoint.md#localaxis1ofbodya-zilch-e)| | |
| |[ LocalAxis1OfBodyB](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/universaljoint.md#localaxis1ofbodyb-zilch-e)| | |
| |[ LocalPointA](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/universaljoint.md#localpointa-zilch-engine)| | |
| |[ LocalPointB](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/universaljoint.md#localpointb-zilch-engine)| | |
| |[ WorldPointA](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/universaljoint.md#worldpointa-zilch-engine)| | |
| |[ WorldPointB](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/universaljoint.md#worldpointb-zilch-engine)| | |


 #  Properties


---  
 #  LocalAxis0OfBodyA : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> One of the two axes in local space of object A that the objects are allowed to rotate about.
> ``` lang=cpp, name=Nada
> var LocalAxis0OfBodyA : Real3


---  
 #  LocalAxis0OfBodyB : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> One of the two axes in local space of object B that the objects are allowed to rotate about.
> ``` lang=cpp, name=Nada
> var LocalAxis0OfBodyB : Real3


---  
 #  LocalAxis1OfBodyA : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> One of the two axes in local space of object A that the objects are allowed to rotate about.
> ``` lang=cpp, name=Nada
> var LocalAxis1OfBodyA : Real3


---  
 #  LocalAxis1OfBodyB : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> One of the two axes in local space of object B that the objects are allowed to rotate about.
> ``` lang=cpp, name=Nada
> var LocalAxis1OfBodyB : Real3


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
 #  SetWorldPoints : Void

> Sets the position of the anchor on object A and B given a position in world space 
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function SetWorldPoints(point : Real3)
> ``` 


---  
 #  UniversalJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function UniversalJoint()
> ``` 


---  
 

 
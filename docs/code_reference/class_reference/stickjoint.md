 `Component` `Physics`



(NOTE) A stick joint is used to simulate a rope or a stick. This joint forces a constant distance between the anchor points on the objects. If there is no limit, this behaves as a stick. If there is a limit, then this behaves as a rope. Motors and springs are also applied to the axis of the rope. Add on definitions: Limit: A limit will provide a min/max distance that the anchors can be between. Motor: A motor will push/pull the objects in the direction of the rope. The motor will not have any effect unless a limit or spring is present. Spring: A spring will make the rope behave spring-like at its boundaries.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ SetWorldPoints](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/stickjoint.md#setworldpoints-void)|[ Length](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/stickjoint.md#length-zilch-engine-docum)|[joint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/joint.md)| |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/stickjoint.md#stickjoint-void)|[ LocalPointA](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/stickjoint.md#localpointa-zilch-engine)| | |
| |[ LocalPointB](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/stickjoint.md#localpointb-zilch-engine)| | |
| |[ WorldPointA](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/stickjoint.md#worldpointa-zilch-engine)| | |
| |[ WorldPointB](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/stickjoint.md#worldpointb-zilch-engine)| | |


 #  Properties


---  
 #  Length : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The desired length between the anchor points of object A and B.
> ``` lang=cpp, name=Nada
> var Length : Real


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
 #  StickJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function StickJoint()
> ``` 


---  
 

 
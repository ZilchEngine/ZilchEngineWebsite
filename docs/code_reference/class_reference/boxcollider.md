 `Component` `Physics`



(NOTE) Defines the collision volume of a box defined by a size on each axis.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md#boxcollider-void)|[ HalfSize](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md#halfsize-zilch-engine-doc)|[collider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md)| |
| |[ Size](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md#size-zilch-engine-documen)| | |
| |[ WorldSize](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md#worldsize-zilch-engine-do)| | |


 #  Properties


---  
 #  HalfSize : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The half size (from the center to the upper-right corner) on each axis of the box in local space. Used to make the box's size match a model or some other volume without needing to scale the transform (also avoids non-uniform scale issues).
> ``` lang=cpp, name=Nada
> var HalfSize : Real3


---  
 #  Size : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The size (from min to max) on each axis of the box in local space. Used to make the box's size match a model or some other volume without needing to scale the transform (also avoids non-uniform scale issues).
> ``` lang=cpp, name=Nada
> var Size : Real3


---  
 #  WorldSize : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

 `read-only`

> The size of the box after the transform is applied (scale and rotation).
> ``` lang=cpp, name=Nada
> var WorldSize : Real3


---  
 #  Methods


---  
 #  BoxCollider : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function BoxCollider()
> ``` 


---  
 

 
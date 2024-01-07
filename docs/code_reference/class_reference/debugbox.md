 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/debugbox.md#debugbox-void)|[ Color](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/debugbox.md#color-zilch-engine-docume)| | |
| |[ Filled](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/debugbox.md#filled-zilch-engine-docum)| | |
| |[ HalfExtents](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/debugbox.md#halfextents-zilch-engine)| | |
| |[ OnTop](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/debugbox.md#ontop-zilch-engine-docume)| | |
| |[ Position](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/debugbox.md#position-zilch-engine-doc)| | |
| |[ Rotation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/debugbox.md#rotation-zilch-engine-doc)| | |
| |[ ViewAligned](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/debugbox.md#viewaligned-zilch-engine)| | |
| |[ ViewScaled](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/debugbox.md#viewscaled-zilch-engine-d)| | |
| |[ ViewScaleOffset](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/debugbox.md#viewscaleoffset-zilch-eng)| | |


 #  Properties


---  
 #  Color : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

> 
> ``` lang=cpp, name=Nada
> var Color : Real4


---  
 #  Filled : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var Filled : Boolean


---  
 #  HalfExtents : [real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)

> 
> ``` lang=cpp, name=Nada
> var HalfExtents : Real2


---  
 #  OnTop : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var OnTop : Boolean


---  
 #  Position : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> 
> ``` lang=cpp, name=Nada
> var Position : Real3


---  
 #  Rotation : [quaternion](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/quaternion.md)

> 
> ``` lang=cpp, name=Nada
> var Rotation : Quaternion


---  
 #  ViewAligned : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var ViewAligned : Boolean


---  
 #  ViewScaled : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var ViewScaled : Boolean


---  
 #  ViewScaleOffset : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> 
> ``` lang=cpp, name=Nada
> var ViewScaleOffset : Real3


---  
 #  Methods


---  
 #  DebugBox : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function DebugBox()
> ``` 


---  
 #  DebugBox : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |aabb|[aabb](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md)| |
> ``` lang=cpp, name=Nada
> function DebugBox(aabb : Aabb)
> ``` 


---  
 #  DebugBox : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |halfExtents|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function DebugBox(position : Real3, halfExtents : Real)
> ``` 


---  
 #  DebugBox : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |halfExtents|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |rotation|[quaternion](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/quaternion.md)| |
> ``` lang=cpp, name=Nada
> function DebugBox(position : Real3, halfExtents : Real, rotation : Quaternion)
> ``` 


---  
 #  DebugBox : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |halfExtents|[real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)| |
> ``` lang=cpp, name=Nada
> function DebugBox(position : Real3, halfExtents : Real2)
> ``` 


---  
 #  DebugBox : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |halfExtents|[real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)| |
> |rotation|[quaternion](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/quaternion.md)| |
> ``` lang=cpp, name=Nada
> function DebugBox(position : Real3, halfExtents : Real2, rotation : Quaternion)
> ``` 


---  
 

 
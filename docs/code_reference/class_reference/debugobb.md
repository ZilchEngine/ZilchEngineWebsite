 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](debugobb.md#debugobb-void)|[ Color](debugobb.md#color-zilch-engine-docume)| | |
| |[ Corners](debugobb.md#corners-zilch-engine-docu)| | |
| |[ Filled](debugobb.md#filled-zilch-engine-docum)| | |
| |[ HalfExtents](debugobb.md#halfextents-zilch-engine)| | |
| |[ OnTop](debugobb.md#ontop-zilch-engine-docume)| | |
| |[ Position](debugobb.md#position-zilch-engine-doc)| | |
| |[ Rotation](debugobb.md#rotation-zilch-engine-doc)| | |
| |[ ViewAligned](debugobb.md#viewaligned-zilch-engine)| | |
| |[ ViewScaled](debugobb.md#viewscaled-zilch-engine-d)| | |
| |[ ViewScaleOffset](debugobb.md#viewscaleoffset-zilch-eng)| | |


 #  Properties


---  
 #  Color : [real4](../nada_base_types/real4.md)

> 
> ``` lang=cpp, name=Nada
> var Color : Real4


---  
 #  Corners : [boolean](../nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var Corners : Boolean


---  
 #  Filled : [boolean](../nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var Filled : Boolean


---  
 #  HalfExtents : [real3](../nada_base_types/real3.md)

> 
> ``` lang=cpp, name=Nada
> var HalfExtents : Real3


---  
 #  OnTop : [boolean](../nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var OnTop : Boolean


---  
 #  Position : [real3](../nada_base_types/real3.md)

> 
> ``` lang=cpp, name=Nada
> var Position : Real3


---  
 #  Rotation : [quaternion](../nada_base_types/quaternion.md)

> 
> ``` lang=cpp, name=Nada
> var Rotation : Quaternion


---  
 #  ViewAligned : [boolean](../nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var ViewAligned : Boolean


---  
 #  ViewScaled : [boolean](../nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var ViewScaled : Boolean


---  
 #  ViewScaleOffset : [real3](../nada_base_types/real3.md)

> 
> ``` lang=cpp, name=Nada
> var ViewScaleOffset : Real3


---  
 #  Methods


---  
 #  DebugObb : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function DebugObb()
> ``` 


---  
 #  DebugObb : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |aabb|[aabb](aabb.md)| |
> ``` lang=cpp, name=Nada
> function DebugObb(aabb : Aabb)
> ``` 


---  
 #  DebugObb : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[real3](../nada_base_types/real3.md)| |
> |halfExtents|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function DebugObb(position : Real3, halfExtents : Real)
> ``` 


---  
 #  DebugObb : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[real3](../nada_base_types/real3.md)| |
> |halfExtents|[real](../nada_base_types/real.md)| |
> |rotation|[quaternion](../nada_base_types/quaternion.md)| |
> ``` lang=cpp, name=Nada
> function DebugObb(position : Real3, halfExtents : Real, rotation : Quaternion)
> ``` 


---  
 #  DebugObb : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[real3](../nada_base_types/real3.md)| |
> |halfExtents|[real3](../nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function DebugObb(position : Real3, halfExtents : Real3)
> ``` 


---  
 #  DebugObb : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[real3](../nada_base_types/real3.md)| |
> |halfExtents|[real3](../nada_base_types/real3.md)| |
> |rotation|[quaternion](../nada_base_types/quaternion.md)| |
> ``` lang=cpp, name=Nada
> function DebugObb(position : Real3, halfExtents : Real3, rotation : Quaternion)
> ``` 


---  
 #  DebugObb : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[real3](../nada_base_types/real3.md)| |
> |halfExtents|[real3](../nada_base_types/real3.md)| |
> |rotation|[real3x3](../nada_base_types/real3x3.md)| |
> ``` lang=cpp, name=Nada
> function DebugObb(position : Real3, halfExtents : Real3, rotation : Real3x3)
> ``` 


---  
 

 
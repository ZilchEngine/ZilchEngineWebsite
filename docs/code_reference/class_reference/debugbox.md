 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](debugbox.md#debugbox-void)|[Color](debugbox.md#color-zilch-engine-docume)| | |
| |[Filled](debugbox.md#filled-zilch-engine-docum)| | |
| |[HalfExtents](debugbox.md#halfextents-zilch-engine)| | |
| |[OnTop](debugbox.md#ontop-zilch-engine-docume)| | |
| |[Position](debugbox.md#position-zilch-engine-doc)| | |
| |[Rotation](debugbox.md#rotation-zilch-engine-doc)| | |
| |[ViewAligned](debugbox.md#viewaligned-zilch-engine)| | |
| |[ViewScaled](debugbox.md#viewscaled-zilch-engine-d)| | |
| |[ViewScaleOffset](debugbox.md#viewscaleoffset-zilch-eng)| | |


 #  Properties


---  
 #  Color : [real4](../nada_base_types/real4.md)

> 
> ```TS:Nada
> var Color : Real4


---  
 #  Filled : [boolean](../nada_base_types/boolean.md)

> 
> ```TS:Nada
> var Filled : Boolean


---  
 #  HalfExtents : [real2](../nada_base_types/real2.md)

> 
> ```TS:Nada
> var HalfExtents : Real2


---  
 #  OnTop : [boolean](../nada_base_types/boolean.md)

> 
> ```TS:Nada
> var OnTop : Boolean


---  
 #  Position : [real3](../nada_base_types/real3.md)

> 
> ```TS:Nada
> var Position : Real3


---  
 #  Rotation : [quaternion](../nada_base_types/quaternion.md)

> 
> ```TS:Nada
> var Rotation : Quaternion


---  
 #  ViewAligned : [boolean](../nada_base_types/boolean.md)

> 
> ```TS:Nada
> var ViewAligned : Boolean


---  
 #  ViewScaled : [boolean](../nada_base_types/boolean.md)

> 
> ```TS:Nada
> var ViewScaled : Boolean


---  
 #  ViewScaleOffset : [real3](../nada_base_types/real3.md)

> 
> ```TS:Nada
> var ViewScaleOffset : Real3


---  
 #  Methods


---  
 #  DebugBox : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function DebugBox()
> ``` 


---  
 #  DebugBox : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |aabb|[aabb](aabb.md)| |
> ```TS:Nada
> function DebugBox(aabb : Aabb)
> ``` 


---  
 #  DebugBox : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[real3](../nada_base_types/real3.md)| |
> |halfExtents|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function DebugBox(position : Real3, halfExtents : Real)
> ``` 


---  
 #  DebugBox : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[real3](../nada_base_types/real3.md)| |
> |halfExtents|[real](../nada_base_types/real.md)| |
> |rotation|[quaternion](../nada_base_types/quaternion.md)| |
> ```TS:Nada
> function DebugBox(position : Real3, halfExtents : Real, rotation : Quaternion)
> ``` 


---  
 #  DebugBox : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[real3](../nada_base_types/real3.md)| |
> |halfExtents|[real2](../nada_base_types/real2.md)| |
> ```TS:Nada
> function DebugBox(position : Real3, halfExtents : Real2)
> ``` 


---  
 #  DebugBox : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[real3](../nada_base_types/real3.md)| |
> |halfExtents|[real2](../nada_base_types/real2.md)| |
> |rotation|[quaternion](../nada_base_types/quaternion.md)| |
> ```TS:Nada
> function DebugBox(position : Real3, halfExtents : Real2, rotation : Quaternion)
> ``` 


---  
 

 
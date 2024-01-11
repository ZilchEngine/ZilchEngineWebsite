 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](debugcylinder.md#debugcylinder-void)|[ Color](debugcylinder.md#color-zilch-engine-docume)| | |
| |[ End](debugcylinder.md#end-zilch-engine-document)| | |
| |[ OnTop](debugcylinder.md#ontop-zilch-engine-docume)| | |
| |[ Radius](debugcylinder.md#radius-zilch-engine-docum)| | |
| |[ Start](debugcylinder.md#start-zilch-engine-docume)| | |
| |[ ViewAligned](debugcylinder.md#viewaligned-zilch-engine)| | |
| |[ ViewScaled](debugcylinder.md#viewscaled-zilch-engine-d)| | |
| |[ ViewScaleOffset](debugcylinder.md#viewscaleoffset-zilch-eng)| | |


 #  Properties


---  
 #  Color : [real4](../nada_base_types/real4.md)

> 
> ``` lang=cpp, name=Nada
> var Color : Real4


---  
 #  End : [real3](../nada_base_types/real3.md)

> 
> ``` lang=cpp, name=Nada
> var End : Real3


---  
 #  OnTop : [boolean](../nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var OnTop : Boolean


---  
 #  Radius : [real](../nada_base_types/real.md)

> 
> ``` lang=cpp, name=Nada
> var Radius : Real


---  
 #  Start : [real3](../nada_base_types/real3.md)

> 
> ``` lang=cpp, name=Nada
> var Start : Real3


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
 #  DebugCylinder : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function DebugCylinder()
> ``` 


---  
 #  DebugCylinder : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |start|[real3](../nada_base_types/real3.md)| |
> |end|[real3](../nada_base_types/real3.md)| |
> |radius|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function DebugCylinder(start : Real3, end : Real3, radius : Real)
> ``` 


---  
 #  DebugCylinder : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[real3](../nada_base_types/real3.md)| |
> |axis|[real3](../nada_base_types/real3.md)| |
> |height|[real](../nada_base_types/real.md)| |
> |radius|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function DebugCylinder(position : Real3, axis : Real3, height : Real, radius : Real)
> ``` 


---  
 

 
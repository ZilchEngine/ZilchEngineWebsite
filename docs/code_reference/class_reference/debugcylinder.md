 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/debugcylinder.md#debugcylinder-void)|[ Color](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/debugcylinder.md#color-zilch-engine-docume)| | |
| |[ End](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/debugcylinder.md#end-zilch-engine-document)| | |
| |[ OnTop](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/debugcylinder.md#ontop-zilch-engine-docume)| | |
| |[ Radius](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/debugcylinder.md#radius-zilch-engine-docum)| | |
| |[ Start](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/debugcylinder.md#start-zilch-engine-docume)| | |
| |[ ViewAligned](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/debugcylinder.md#viewaligned-zilch-engine)| | |
| |[ ViewScaled](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/debugcylinder.md#viewscaled-zilch-engine-d)| | |
| |[ ViewScaleOffset](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/debugcylinder.md#viewscaleoffset-zilch-eng)| | |


 #  Properties


---  
 #  Color : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

> 
> ``` lang=cpp, name=Nada
> var Color : Real4


---  
 #  End : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> 
> ``` lang=cpp, name=Nada
> var End : Real3


---  
 #  OnTop : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var OnTop : Boolean


---  
 #  Radius : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> 
> ``` lang=cpp, name=Nada
> var Radius : Real


---  
 #  Start : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> 
> ``` lang=cpp, name=Nada
> var Start : Real3


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
> |start|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |end|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |radius|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function DebugCylinder(start : Real3, end : Real3, radius : Real)
> ``` 


---  
 #  DebugCylinder : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |axis|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |height|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |radius|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function DebugCylinder(position : Real3, axis : Real3, height : Real, radius : Real)
> ``` 


---  
 

 
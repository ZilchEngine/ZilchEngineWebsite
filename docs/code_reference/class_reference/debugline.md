 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](debugline.md#debugline-void)|[ BoxHeads](debugline.md#boxheads-zilch-engine-doc)| | |
| |[ Color](debugline.md#color-zilch-engine-docume)| | |
| |[ DualHeads](debugline.md#dualheads-zilch-engine-do)| | |
| |[ End](debugline.md#end-zilch-engine-document)| | |
| |[ Filled](debugline.md#filled-zilch-engine-docum)| | |
| |[ HeadSize](debugline.md#headsize-zilch-engine-doc)| | |
| |[ OnTop](debugline.md#ontop-zilch-engine-docume)| | |
| |[ Start](debugline.md#start-zilch-engine-docume)| | |
| |[ ViewAligned](debugline.md#viewaligned-zilch-engine)| | |
| |[ ViewScaled](debugline.md#viewscaled-zilch-engine-d)| | |
| |[ ViewScaleOffset](debugline.md#viewscaleoffset-zilch-eng)| | |


 #  Properties


---  
 #  BoxHeads : [boolean](../nada_base_types/boolean.md)

> 
> ```TS:Nada
> var BoxHeads : Boolean


---  
 #  Color : [real4](../nada_base_types/real4.md)

> 
> ```TS:Nada
> var Color : Real4


---  
 #  DualHeads : [boolean](../nada_base_types/boolean.md)

> 
> ```TS:Nada
> var DualHeads : Boolean


---  
 #  End : [real3](../nada_base_types/real3.md)

> 
> ```TS:Nada
> var End : Real3


---  
 #  Filled : [boolean](../nada_base_types/boolean.md)

> 
> ```TS:Nada
> var Filled : Boolean


---  
 #  HeadSize : [real](../nada_base_types/real.md)

> 
> ```TS:Nada
> var HeadSize : Real


---  
 #  OnTop : [boolean](../nada_base_types/boolean.md)

> 
> ```TS:Nada
> var OnTop : Boolean


---  
 #  Start : [real3](../nada_base_types/real3.md)

> 
> ```TS:Nada
> var Start : Real3


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
 #  DebugLine : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function DebugLine()
> ``` 


---  
 #  DebugLine : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |ray|[ray](ray.md)| |
> ```TS:Nada
> function DebugLine(ray : Ray)
> ``` 


---  
 #  DebugLine : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |ray|[ray](ray.md)| |
> |t|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function DebugLine(ray : Ray, t : Real)
> ``` 


---  
 #  DebugLine : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |start|[real3](../nada_base_types/real3.md)| |
> |end|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function DebugLine(start : Real3, end : Real3)
> ``` 


---  
 #  DebugLine : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |start|[real3](../nada_base_types/real3.md)| |
> |end|[real3](../nada_base_types/real3.md)| |
> |headSize|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function DebugLine(start : Real3, end : Real3, headSize : Real)
> ``` 


---  
 #  DebugLine : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |segment|[segment](segment.md)| |
> ```TS:Nada
> function DebugLine(segment : Segment)
> ``` 


---  
 

 
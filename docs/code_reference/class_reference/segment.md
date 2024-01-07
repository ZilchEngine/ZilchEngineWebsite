 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetPoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/segment.md#getpoint-zilch-engine-doc)|[ End](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/segment.md#end-zilch-engine-document)| | |
|[ GetTValue](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/segment.md#gettvalue-zilch-engine-do)|[ Start](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/segment.md#start-zilch-engine-docume)| | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/segment.md#segment-void)| | | |


 #  Properties


---  
 #  End : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> 
> ``` lang=cpp, name=Nada
> var End : Real3


---  
 #  Start : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> 
> ``` lang=cpp, name=Nada
> var Start : Real3


---  
 #  Methods


---  
 #  GetPoint : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Returns the point at the given t-value.
> |Name|Type|Description|
> |---|---|---|
> |tValue|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function GetPoint(tValue : Real) : Real3
> ``` 


---  
 #  GetTValue : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Returns the t-value that would result in the given point projected onto the segment.
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function GetTValue(point : Real3) : Real
> ``` 


---  
 #  Segment : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Segment()
> ``` 


---  
 #  Segment : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |start|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |end|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function Segment(start : Real3, end : Real3)
> ``` 


---  
 #  Segment : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[segment](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/segment.md)| |
> ``` lang=cpp, name=Nada
> function Segment(p0 : Segment)
> ``` 


---  
 

 
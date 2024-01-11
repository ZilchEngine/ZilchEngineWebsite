 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetPoint](segment.md#getpoint-zilch-engine-doc)|[ End](segment.md#end-zilch-engine-document)| | |
|[ GetTValue](segment.md#gettvalue-zilch-engine-do)|[ Start](segment.md#start-zilch-engine-docume)| | |
|[ Constructor](segment.md#segment-void)| | | |


 #  Properties


---  
 #  End : [real3](../nada_base_types/real3.md)

> 
> ``` lang=cpp, name=Nada
> var End : Real3


---  
 #  Start : [real3](../nada_base_types/real3.md)

> 
> ``` lang=cpp, name=Nada
> var Start : Real3


---  
 #  Methods


---  
 #  GetPoint : [real3](../nada_base_types/real3.md)

> Returns the point at the given t-value.
> |Name|Type|Description|
> |---|---|---|
> |tValue|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function GetPoint(tValue : Real) : Real3
> ``` 


---  
 #  GetTValue : [real](../nada_base_types/real.md)

> Returns the t-value that would result in the given point projected onto the segment.
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](../nada_base_types/real3.md)| |
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
> |start|[real3](../nada_base_types/real3.md)| |
> |end|[real3](../nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function Segment(start : Real3, end : Real3)
> ``` 


---  
 #  Segment : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[segment](segment.md)| |
> ``` lang=cpp, name=Nada
> function Segment(p0 : Segment)
> ``` 


---  
 

 
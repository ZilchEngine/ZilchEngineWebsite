 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Parse](byte.md#parse-zilch-engine-docume)|[ PositiveMax](byte.md#positivemax-zilch-engine)| | |
| |[ PositiveValueClosestToZero](byte.md#positivevalueclosesttoze)| | |


 #  Properties


---  
 #  PositiveMax : [byte](byte.md)

 `read-only` `static`

> The largest (most positive) value that can be represented by a Byte.
> ``` lang=cpp, name=Nada
> var PositiveMax : Byte


---  
 #  PositiveValueClosestToZero : [byte](byte.md)

 `read-only` `static`

> The positive value closest to zero that can be represented by a Byte.
> ``` lang=cpp, name=Nada
> var PositiveValueClosestToZero : Byte


---  
 #  Methods


---  
 #  Parse : [byte](byte.md)

 `static`

> Attempt to convert the given StringRange to a Byte. If parsing fails 0 is returned.
> |Name|Type|Description|
> |---|---|---|
> |p0|[stringrange](stringrange.md)| |
> ``` lang=cpp, name=Nada
> function Parse(p0 : StringRange) : Byte
> ``` 


---  
 

 
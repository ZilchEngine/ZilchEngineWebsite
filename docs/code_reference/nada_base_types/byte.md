 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Parse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/byte.md#parse-zilch-engine-docume)|[ PositiveMax](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/byte.md#positivemax-zilch-engine)| | |
| |[ PositiveValueClosestToZero](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/byte.md#positivevalueclosesttoze)| | |


 #  Properties


---  
 #  PositiveMax : [byte](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/byte.md)

 `read-only` `static`

> The largest (most positive) value that can be represented by a Byte.
> ``` lang=cpp, name=Nada
> var PositiveMax : Byte


---  
 #  PositiveValueClosestToZero : [byte](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/byte.md)

 `read-only` `static`

> The positive value closest to zero that can be represented by a Byte.
> ``` lang=cpp, name=Nada
> var PositiveValueClosestToZero : Byte


---  
 #  Methods


---  
 #  Parse : [byte](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/byte.md)

 `static`

> Attempt to convert the given StringRange to a Byte. If parsing fails 0 is returned.
> |Name|Type|Description|
> |---|---|---|
> |p0|[stringrange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/stringrange.md)| |
> ``` lang=cpp, name=Nada
> function Parse(p0 : StringRange) : Byte
> ``` 


---  
 

 
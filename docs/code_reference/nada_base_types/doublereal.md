 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Parse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/doublereal.md#parse-zilch-engine-docume)|[ NegativeMin](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/doublereal.md#negativemin-zilch-engine)| | |
| |[ NegativeValueClosestToZero](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/doublereal.md#negativevalueclosesttoze)| | |
| |[ PositiveMax](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/doublereal.md#positivemax-zilch-engine)| | |
| |[ PositiveValueClosestToZero](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/doublereal.md#positivevalueclosesttoze)| | |


 #  Properties


---  
 #  NegativeMin : [doublereal](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/doublereal.md)

 `read-only` `static`

> The smallest (most negative) value that can be represented by a DoubleReal.
> ``` lang=cpp, name=Nada
> var NegativeMin : DoubleReal


---  
 #  NegativeValueClosestToZero : [doublereal](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/doublereal.md)

 `read-only` `static`

> The negative value closest to zero that can be represented by a DoubleReal.
> ``` lang=cpp, name=Nada
> var NegativeValueClosestToZero : DoubleReal


---  
 #  PositiveMax : [doublereal](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/doublereal.md)

 `read-only` `static`

> The largest (most positive) value that can be represented by a DoubleReal.
> ``` lang=cpp, name=Nada
> var PositiveMax : DoubleReal


---  
 #  PositiveValueClosestToZero : [doublereal](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/doublereal.md)

 `read-only` `static`

> The positive value closest to zero that can be represented by a DoubleReal.
> ``` lang=cpp, name=Nada
> var PositiveValueClosestToZero : DoubleReal


---  
 #  Methods


---  
 #  Parse : [doublereal](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/doublereal.md)

 `static`

> Attempt to convert the given StringRange to a DoubleReal. If parsing fails 0 is returned.
> |Name|Type|Description|
> |---|---|---|
> |p0|[stringrange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/stringrange.md)| |
> ``` lang=cpp, name=Nada
> function Parse(p0 : StringRange) : DoubleReal
> ``` 


---  
 

 
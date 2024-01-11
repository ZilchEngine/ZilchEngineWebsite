 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Parse](doubleinteger.md#parse-zilch-engine-docume)|[ NegativeMin](doubleinteger.md#negativemin-zilch-engine)| | |
| |[ NegativeValueClosestToZero](doubleinteger.md#negativevalueclosesttoze)| | |
| |[ PositiveMax](doubleinteger.md#positivemax-zilch-engine)| | |
| |[ PositiveValueClosestToZero](doubleinteger.md#positivevalueclosesttoze)| | |


 #  Properties


---  
 #  NegativeMin : [doubleinteger](doubleinteger.md)

 `read-only` `static`

> The smallest (most negative) value that can be represented by a DoubleInteger.
> ``` lang=cpp, name=Nada
> var NegativeMin : DoubleInteger


---  
 #  NegativeValueClosestToZero : [doubleinteger](doubleinteger.md)

 `read-only` `static`

> The negative value closest to zero that can be represented by a DoubleInteger.
> ``` lang=cpp, name=Nada
> var NegativeValueClosestToZero : DoubleInteger


---  
 #  PositiveMax : [doubleinteger](doubleinteger.md)

 `read-only` `static`

> The largest (most positive) value that can be represented by a DoubleInteger.
> ``` lang=cpp, name=Nada
> var PositiveMax : DoubleInteger


---  
 #  PositiveValueClosestToZero : [doubleinteger](doubleinteger.md)

 `read-only` `static`

> The positive value closest to zero that can be represented by a DoubleInteger.
> ``` lang=cpp, name=Nada
> var PositiveValueClosestToZero : DoubleInteger


---  
 #  Methods


---  
 #  Parse : [doubleinteger](doubleinteger.md)

 `static`

> Attempt to convert the given StringRange to a DoubleInteger. If parsing fails 0 is returned.
> |Name|Type|Description|
> |---|---|---|
> |p0|[stringrange](stringrange.md)| |
> ``` lang=cpp, name=Nada
> function Parse(p0 : StringRange) : DoubleInteger
> ``` 


---  
 

 
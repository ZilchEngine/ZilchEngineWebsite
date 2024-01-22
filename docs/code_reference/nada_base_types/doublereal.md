 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Parse](doublereal.md#parse-zilch-engine-docume)|[NegativeMin](doublereal.md#negativemin-zilch-engine)| | |
| |[NegativeValueClosestToZero](doublereal.md#negativevalueclosesttoze)| | |
| |[PositiveMax](doublereal.md#positivemax-zilch-engine)| | |
| |[PositiveValueClosestToZero](doublereal.md#positivevalueclosesttoze)| | |


 #  Properties


---  
 #  NegativeMin : [doublereal](doublereal.md)

 `read-only` `static`

> The smallest (most negative) value that can be represented by a DoubleReal.
> ```TS:Nada
> var NegativeMin : DoubleReal


---  
 #  NegativeValueClosestToZero : [doublereal](doublereal.md)

 `read-only` `static`

> The negative value closest to zero that can be represented by a DoubleReal.
> ```TS:Nada
> var NegativeValueClosestToZero : DoubleReal


---  
 #  PositiveMax : [doublereal](doublereal.md)

 `read-only` `static`

> The largest (most positive) value that can be represented by a DoubleReal.
> ```TS:Nada
> var PositiveMax : DoubleReal


---  
 #  PositiveValueClosestToZero : [doublereal](doublereal.md)

 `read-only` `static`

> The positive value closest to zero that can be represented by a DoubleReal.
> ```TS:Nada
> var PositiveValueClosestToZero : DoubleReal


---  
 #  Methods


---  
 #  Parse : [doublereal](doublereal.md)

 `static`

> Attempt to convert the given StringRange to a DoubleReal. If parsing fails 0 is returned.
> |Name|Type|Description|
> |---|---|---|
> |p0|[stringrange](stringrange.md)| |
> ```TS:Nada
> function Parse(p0 : StringRange) : DoubleReal
> ``` 


---  
 

 
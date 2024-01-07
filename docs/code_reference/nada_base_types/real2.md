 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Get](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md#get-zilch-engine-document)|[ Count](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md#count-zilch-engine-docume)| | |
|[ GetAxis](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md#getaxis-zilch-engine-docu)|[ NegativeMin](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md#negativemin-zilch-engine)| | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md#real2-void)|[ NegativeValueClosestToZero](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md#negativevalueclosesttoze)| | |
|[ Set](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md#set-void)|[ One](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md#one-zilch-engine-document)| | |
| |[ PositiveMax](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md#positivemax-zilch-engine)| | |
| |[ PositiveValueClosestToZero](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md#positivevalueclosesttoze)| | |
| |[ XAxis](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md#xaxis-zilch-engine-docume)| | |
| |[ YAxis](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md#yaxis-zilch-engine-docume)| | |
| |[ Zero](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md#zilch-zilch-engine-documen)| | |


 #  Properties


---  
 #  Count : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Count : Integer


---  
 #  NegativeMin : [real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)

 `read-only` `static`

> The smallest (most negative) value that can be represented by a Real.
> ``` lang=cpp, name=Nada
> var NegativeMin : Real2


---  
 #  NegativeValueClosestToZero : [real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)

 `read-only` `static`

> The negative value closest to zero that can be represented by a Real.
> ``` lang=cpp, name=Nada
> var NegativeValueClosestToZero : Real2


---  
 #  One : [real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)

 `read-only` `static`

> The one vector (a vector containing all ones).
> ``` lang=cpp, name=Nada
> var One : Real2


---  
 #  PositiveMax : [real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)

 `read-only` `static`

> The largest (most positive) value that can be represented by a Real.
> ``` lang=cpp, name=Nada
> var PositiveMax : Real2


---  
 #  PositiveValueClosestToZero : [real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)

 `read-only` `static`

> The positive value closest to zero that can be represented by a Real.
> ``` lang=cpp, name=Nada
> var PositiveValueClosestToZero : Real2


---  
 #  XAxis : [real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var XAxis : Real2


---  
 #  YAxis : [real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var YAxis : Real2


---  
 #  Zero : [real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)

 `read-only` `static`

> The zero vector (a vector containing all zeroes).
> ``` lang=cpp, name=Nada
> var Zero : Real2


---  
 #  Methods


---  
 #  Get : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Get(p0 : Integer) : Real
> ``` 


---  
 #  GetAxis : [real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)

 `static`

> Returns an axis vector from the given index (ie. 0 is XAxis, 1 is YAxis, etc...
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function GetAxis(p0 : Integer) : Real2
> ``` 


---  
 #  Real2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Real2()
> ``` 


---  
 #  Real2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |scalar|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function Real2(scalar : Real)
> ``` 


---  
 #  Real2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |p1|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function Real2(p0 : Real, p1 : Real)
> ``` 


---  
 #  Real2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)| |
> ``` lang=cpp, name=Nada
> function Real2(p0 : Real2)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |p1|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function Set(p0 : Integer, p1 : Real)
> ``` 


---  
 

 
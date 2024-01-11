 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Get](real2.md#get-zilch-engine-document)|[ Count](real2.md#count-zilch-engine-docume)| | |
|[ GetAxis](real2.md#getaxis-zilch-engine-docu)|[ NegativeMin](real2.md#negativemin-zilch-engine)| | |
|[ Constructor](real2.md#real2-void)|[ NegativeValueClosestToZero](real2.md#negativevalueclosesttoze)| | |
|[ Set](real2.md#set-void)|[ One](real2.md#one-zilch-engine-document)| | |
| |[ PositiveMax](real2.md#positivemax-zilch-engine)| | |
| |[ PositiveValueClosestToZero](real2.md#positivevalueclosesttoze)| | |
| |[ XAxis](real2.md#xaxis-zilch-engine-docume)| | |
| |[ YAxis](real2.md#yaxis-zilch-engine-docume)| | |
| |[ Zero](real2.md#zilch-zilch-engine-documen)| | |


 #  Properties


---  
 #  Count : [integer](integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Count : Integer


---  
 #  NegativeMin : [real2](real2.md)

 `read-only` `static`

> The smallest (most negative) value that can be represented by a Real.
> ``` lang=cpp, name=Nada
> var NegativeMin : Real2


---  
 #  NegativeValueClosestToZero : [real2](real2.md)

 `read-only` `static`

> The negative value closest to zero that can be represented by a Real.
> ``` lang=cpp, name=Nada
> var NegativeValueClosestToZero : Real2


---  
 #  One : [real2](real2.md)

 `read-only` `static`

> The one vector (a vector containing all ones).
> ``` lang=cpp, name=Nada
> var One : Real2


---  
 #  PositiveMax : [real2](real2.md)

 `read-only` `static`

> The largest (most positive) value that can be represented by a Real.
> ``` lang=cpp, name=Nada
> var PositiveMax : Real2


---  
 #  PositiveValueClosestToZero : [real2](real2.md)

 `read-only` `static`

> The positive value closest to zero that can be represented by a Real.
> ``` lang=cpp, name=Nada
> var PositiveValueClosestToZero : Real2


---  
 #  XAxis : [real2](real2.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var XAxis : Real2


---  
 #  YAxis : [real2](real2.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var YAxis : Real2


---  
 #  Zero : [real2](real2.md)

 `read-only` `static`

> The zero vector (a vector containing all zeroes).
> ``` lang=cpp, name=Nada
> var Zero : Real2


---  
 #  Methods


---  
 #  Get : [real](real.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function Get(p0 : Integer) : Real
> ``` 


---  
 #  GetAxis : [real2](real2.md)

 `static`

> Returns an axis vector from the given index (ie. 0 is XAxis, 1 is YAxis, etc...
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
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
> |scalar|[real](real.md)| |
> ``` lang=cpp, name=Nada
> function Real2(scalar : Real)
> ``` 


---  
 #  Real2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real](real.md)| |
> |p1|[real](real.md)| |
> ``` lang=cpp, name=Nada
> function Real2(p0 : Real, p1 : Real)
> ``` 


---  
 #  Real2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real2](real2.md)| |
> ``` lang=cpp, name=Nada
> function Real2(p0 : Real2)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> |p1|[real](real.md)| |
> ``` lang=cpp, name=Nada
> function Set(p0 : Integer, p1 : Real)
> ``` 


---  
 

 
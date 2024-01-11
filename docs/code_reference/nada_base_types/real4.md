 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Get](real4.md#get-zilch-engine-document)|[ Count](real4.md#count-zilch-engine-docume)| | |
|[ GetAxis](real4.md#getaxis-zilch-engine-docu)|[ NegativeMin](real4.md#negativemin-zilch-engine)| | |
|[ Constructor](real4.md#real4-void)|[ NegativeValueClosestToZero](real4.md#negativevalueclosesttoze)| | |
|[ Set](real4.md#set-void)|[ One](real4.md#one-zilch-engine-document)| | |
| |[ PositiveMax](real4.md#positivemax-zilch-engine)| | |
| |[ PositiveValueClosestToZero](real4.md#positivevalueclosesttoze)| | |
| |[ WAxis](real4.md#waxis-zilch-engine-docume)| | |
| |[ XAxis](real4.md#xaxis-zilch-engine-docume)| | |
| |[ YAxis](real4.md#yaxis-zilch-engine-docume)| | |
| |[ ZAxis](real4.md#zaxis-zilch-engine-docume)| | |
| |[ Zero](real4.md#zilch-zilch-engine-documen)| | |


 #  Properties


---  
 #  Count : [integer](integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Count : Integer


---  
 #  NegativeMin : [real4](real4.md)

 `read-only` `static`

> The smallest (most negative) value that can be represented by a Real.
> ``` lang=cpp, name=Nada
> var NegativeMin : Real4


---  
 #  NegativeValueClosestToZero : [real4](real4.md)

 `read-only` `static`

> The negative value closest to zero that can be represented by a Real.
> ``` lang=cpp, name=Nada
> var NegativeValueClosestToZero : Real4


---  
 #  One : [real4](real4.md)

 `read-only` `static`

> The one vector (a vector containing all ones).
> ``` lang=cpp, name=Nada
> var One : Real4


---  
 #  PositiveMax : [real4](real4.md)

 `read-only` `static`

> The largest (most positive) value that can be represented by a Real.
> ``` lang=cpp, name=Nada
> var PositiveMax : Real4


---  
 #  PositiveValueClosestToZero : [real4](real4.md)

 `read-only` `static`

> The positive value closest to zero that can be represented by a Real.
> ``` lang=cpp, name=Nada
> var PositiveValueClosestToZero : Real4


---  
 #  WAxis : [real4](real4.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var WAxis : Real4


---  
 #  XAxis : [real4](real4.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var XAxis : Real4


---  
 #  YAxis : [real4](real4.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var YAxis : Real4


---  
 #  ZAxis : [real4](real4.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var ZAxis : Real4


---  
 #  Zero : [real4](real4.md)

 `read-only` `static`

> The zero vector (a vector containing all zeroes).
> ``` lang=cpp, name=Nada
> var Zero : Real4


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
 #  GetAxis : [real4](real4.md)

 `static`

> Returns an axis vector from the given index (ie. 0 is XAxis, 1 is YAxis, etc...
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function GetAxis(p0 : Integer) : Real4
> ``` 


---  
 #  Real4 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Real4()
> ``` 


---  
 #  Real4 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |scalar|[real](real.md)| |
> ``` lang=cpp, name=Nada
> function Real4(scalar : Real)
> ``` 


---  
 #  Real4 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real](real.md)| |
> |p1|[real](real.md)| |
> |p2|[real](real.md)| |
> |p3|[real](real.md)| |
> ``` lang=cpp, name=Nada
> function Real4(p0 : Real, p1 : Real, p2 : Real, p3 : Real)
> ``` 


---  
 #  Real4 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real](real.md)| |
> |p1|[real](real.md)| |
> |p2|[real2](real2.md)| |
> ``` lang=cpp, name=Nada
> function Real4(p0 : Real, p1 : Real, p2 : Real2)
> ``` 


---  
 #  Real4 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real](real.md)| |
> |p1|[real2](real2.md)| |
> |p2|[real](real.md)| |
> ``` lang=cpp, name=Nada
> function Real4(p0 : Real, p1 : Real2, p2 : Real)
> ``` 


---  
 #  Real4 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real](real.md)| |
> |p1|[real3](real3.md)| |
> ``` lang=cpp, name=Nada
> function Real4(p0 : Real, p1 : Real3)
> ``` 


---  
 #  Real4 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real2](real2.md)| |
> |p1|[real](real.md)| |
> |p2|[real](real.md)| |
> ``` lang=cpp, name=Nada
> function Real4(p0 : Real2, p1 : Real, p2 : Real)
> ``` 


---  
 #  Real4 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real2](real2.md)| |
> |p1|[real2](real2.md)| |
> ``` lang=cpp, name=Nada
> function Real4(p0 : Real2, p1 : Real2)
> ``` 


---  
 #  Real4 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real3](real3.md)| |
> |p1|[real](real.md)| |
> ``` lang=cpp, name=Nada
> function Real4(p0 : Real3, p1 : Real)
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
 

 
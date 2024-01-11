 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Get](real3.md#get-zilch-engine-document)|[ Count](real3.md#count-zilch-engine-docume)| | |
|[ GetAxis](real3.md#getaxis-zilch-engine-docu)|[ NegativeMin](real3.md#negativemin-zilch-engine)| | |
|[ Constructor](real3.md#real3-void)|[ NegativeValueClosestToZero](real3.md#negativevalueclosesttoze)| | |
|[ Set](real3.md#set-void)|[ One](real3.md#one-zilch-engine-document)| | |
| |[ PositiveMax](real3.md#positivemax-zilch-engine)| | |
| |[ PositiveValueClosestToZero](real3.md#positivevalueclosesttoze)| | |
| |[ XAxis](real3.md#xaxis-zilch-engine-docume)| | |
| |[ YAxis](real3.md#yaxis-zilch-engine-docume)| | |
| |[ ZAxis](real3.md#zaxis-zilch-engine-docume)| | |
| |[ Zero](real3.md#zilch-zilch-engine-documen)| | |


 #  Properties


---  
 #  Count : [integer](integer.md)

 `read-only`

> 
> ```TS:Nada
> var Count : Integer


---  
 #  NegativeMin : [real3](real3.md)

 `read-only` `static`

> The smallest (most negative) value that can be represented by a Real.
> ```TS:Nada
> var NegativeMin : Real3


---  
 #  NegativeValueClosestToZero : [real3](real3.md)

 `read-only` `static`

> The negative value closest to zero that can be represented by a Real.
> ```TS:Nada
> var NegativeValueClosestToZero : Real3


---  
 #  One : [real3](real3.md)

 `read-only` `static`

> The one vector (a vector containing all ones).
> ```TS:Nada
> var One : Real3


---  
 #  PositiveMax : [real3](real3.md)

 `read-only` `static`

> The largest (most positive) value that can be represented by a Real.
> ```TS:Nada
> var PositiveMax : Real3


---  
 #  PositiveValueClosestToZero : [real3](real3.md)

 `read-only` `static`

> The positive value closest to zero that can be represented by a Real.
> ```TS:Nada
> var PositiveValueClosestToZero : Real3


---  
 #  XAxis : [real3](real3.md)

 `read-only` `static`

> 
> ```TS:Nada
> var XAxis : Real3


---  
 #  YAxis : [real3](real3.md)

 `read-only` `static`

> 
> ```TS:Nada
> var YAxis : Real3


---  
 #  ZAxis : [real3](real3.md)

 `read-only` `static`

> 
> ```TS:Nada
> var ZAxis : Real3


---  
 #  Zero : [real3](real3.md)

 `read-only` `static`

> The zero vector (a vector containing all zeroes).
> ```TS:Nada
> var Zero : Real3


---  
 #  Methods


---  
 #  Get : [real](real.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> ```TS:Nada
> function Get(p0 : Integer) : Real
> ``` 


---  
 #  GetAxis : [real3](real3.md)

 `static`

> Returns an axis vector from the given index (ie. 0 is XAxis, 1 is YAxis, etc...
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> ```TS:Nada
> function GetAxis(p0 : Integer) : Real3
> ``` 


---  
 #  Real3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Real3()
> ``` 


---  
 #  Real3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |scalar|[real](real.md)| |
> ```TS:Nada
> function Real3(scalar : Real)
> ``` 


---  
 #  Real3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real](real.md)| |
> |p1|[real](real.md)| |
> |p2|[real](real.md)| |
> ```TS:Nada
> function Real3(p0 : Real, p1 : Real, p2 : Real)
> ``` 


---  
 #  Real3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real](real.md)| |
> |p1|[real2](real2.md)| |
> ```TS:Nada
> function Real3(p0 : Real, p1 : Real2)
> ``` 


---  
 #  Real3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real2](real2.md)| |
> |p1|[real](real.md)| |
> ```TS:Nada
> function Real3(p0 : Real2, p1 : Real)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> |p1|[real](real.md)| |
> ```TS:Nada
> function Set(p0 : Integer, p1 : Real)
> ``` 


---  
 

 
 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Get](real.md#get-zilch-engine-document)|[Count](real.md#count-zilch-engine-docume)| | |
|[GetAxis](real.md#getaxis-zilch-engine-docu)|[NegativeMin](real.md#negativemin-zilch-engine)| | |
|[Parse](real.md#parse-zilch-engine-docume)|[NegativeValueClosestToZero](real.md#negativevalueclosesttoze)| | |
|[Constructor](real.md#real-void)|[One](real.md#one-zilch-engine-document)| | |
|[Reinterpret](real.md#reinterpret-zilch-engine)|[PositiveMax](real.md#positivemax-zilch-engine)| | |
|[Set](real.md#set-void)|[PositiveValueClosestToZero](real.md#positivevalueclosesttoze)| | |
| |[XAxis](real.md#xaxis-zilch-engine-docume)| | |
| |[Zero](real.md#zilch-zilch-engine-documen)| | |


 #  Properties


---  
 #  Count : [integer](integer.md)

 `read-only`

> 
> ```TS:Nada
> var Count : Integer


---  
 #  NegativeMin : [real](real.md)

 `read-only` `static`

> The smallest (most negative) value that can be represented by a Real.
> ```TS:Nada
> var NegativeMin : Real


---  
 #  NegativeValueClosestToZero : [real](real.md)

 `read-only` `static`

> The negative value closest to zero that can be represented by a Real.
> ```TS:Nada
> var NegativeValueClosestToZero : Real


---  
 #  One : [real](real.md)

 `read-only` `static`

> The one vector (a vector containing all ones).
> ```TS:Nada
> var One : Real


---  
 #  PositiveMax : [real](real.md)

 `read-only` `static`

> The largest (most positive) value that can be represented by a Real.
> ```TS:Nada
> var PositiveMax : Real


---  
 #  PositiveValueClosestToZero : [real](real.md)

 `read-only` `static`

> The positive value closest to zero that can be represented by a Real.
> ```TS:Nada
> var PositiveValueClosestToZero : Real


---  
 #  XAxis : [real](real.md)

 `read-only` `static`

> 
> ```TS:Nada
> var XAxis : Real


---  
 #  Zero : [real](real.md)

 `read-only` `static`

> The zero vector (a vector containing all zeroes).
> ```TS:Nada
> var Zero : Real


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
 #  GetAxis : [real](real.md)

 `static`

> Returns an axis vector from the given index (ie. 0 is XAxis, 1 is YAxis, etc...
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> ```TS:Nada
> function GetAxis(p0 : Integer) : Real
> ``` 


---  
 #  Parse : [real](real.md)

 `static`

> Attempt to convert the given StringRange to a Real. If parsing fails 0 is returned.
> |Name|Type|Description|
> |---|---|---|
> |p0|[stringrange](stringrange.md)| |
> ```TS:Nada
> function Parse(p0 : StringRange) : Real
> ``` 


---  
 #  Real : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Real()
> ``` 


---  
 #  Real : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |scalar|[real](real.md)| |
> ```TS:Nada
> function Real(scalar : Real)
> ``` 


---  
 #  Reinterpret : [real](real.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> ```TS:Nada
> function Reinterpret(p0 : Integer) : Real
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
 

 
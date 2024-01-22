 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Get](integer3.md#get-zilch-engine-document)|[Count](integer3.md#count-zilch-engine-docume)| | |
|[GetAxis](integer3.md#getaxis-zilch-engine-docu)|[NegativeMin](integer3.md#negativemin-zilch-engine)| | |
|[Constructor](integer3.md#integer3-void)|[NegativeValueClosestToZero](integer3.md#negativevalueclosesttoze)| | |
|[Set](integer3.md#set-void)|[One](integer3.md#one-zilch-engine-document)| | |
| |[PositiveMax](integer3.md#positivemax-zilch-engine)| | |
| |[PositiveValueClosestToZero](integer3.md#positivevalueclosesttoze)| | |
| |[XAxis](integer3.md#xaxis-zilch-engine-docume)| | |
| |[YAxis](integer3.md#yaxis-zilch-engine-docume)| | |
| |[ZAxis](integer3.md#zaxis-zilch-engine-docume)| | |
| |[Zero](integer3.md#zilch-zilch-engine-documen)| | |


 #  Properties


---  
 #  Count : [integer](integer.md)

 `read-only`

> 
> ```TS:Nada
> var Count : Integer


---  
 #  NegativeMin : [integer3](integer3.md)

 `read-only` `static`

> The smallest (most negative) value that can be represented by an Integer.
> ```TS:Nada
> var NegativeMin : Integer3


---  
 #  NegativeValueClosestToZero : [integer3](integer3.md)

 `read-only` `static`

> The negative value closest to zero that can be represented by an Integer.
> ```TS:Nada
> var NegativeValueClosestToZero : Integer3


---  
 #  One : [integer3](integer3.md)

 `read-only` `static`

> The one vector (a vector containing all ones).
> ```TS:Nada
> var One : Integer3


---  
 #  PositiveMax : [integer3](integer3.md)

 `read-only` `static`

> The largest (most positive) value that can be represented by an Integer.
> ```TS:Nada
> var PositiveMax : Integer3


---  
 #  PositiveValueClosestToZero : [integer3](integer3.md)

 `read-only` `static`

> The positive value closest to zero that can be represented by an Integer.
> ```TS:Nada
> var PositiveValueClosestToZero : Integer3


---  
 #  XAxis : [integer3](integer3.md)

 `read-only` `static`

> 
> ```TS:Nada
> var XAxis : Integer3


---  
 #  YAxis : [integer3](integer3.md)

 `read-only` `static`

> 
> ```TS:Nada
> var YAxis : Integer3


---  
 #  ZAxis : [integer3](integer3.md)

 `read-only` `static`

> 
> ```TS:Nada
> var ZAxis : Integer3


---  
 #  Zero : [integer3](integer3.md)

 `read-only` `static`

> The zero vector (a vector containing all zeroes).
> ```TS:Nada
> var Zero : Integer3


---  
 #  Methods


---  
 #  Get : [integer](integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> ```TS:Nada
> function Get(p0 : Integer) : Integer
> ``` 


---  
 #  GetAxis : [integer3](integer3.md)

 `static`

> Returns an axis vector from the given index (ie. 0 is XAxis, 1 is YAxis, etc...
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> ```TS:Nada
> function GetAxis(p0 : Integer) : Integer3
> ``` 


---  
 #  Integer3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Integer3()
> ``` 


---  
 #  Integer3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |scalar|[integer](integer.md)| |
> ```TS:Nada
> function Integer3(scalar : Integer)
> ``` 


---  
 #  Integer3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> |p1|[integer](integer.md)| |
> |p2|[integer](integer.md)| |
> ```TS:Nada
> function Integer3(p0 : Integer, p1 : Integer, p2 : Integer)
> ``` 


---  
 #  Integer3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> |p1|[integer2](integer2.md)| |
> ```TS:Nada
> function Integer3(p0 : Integer, p1 : Integer2)
> ``` 


---  
 #  Integer3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer2](integer2.md)| |
> |p1|[integer](integer.md)| |
> ```TS:Nada
> function Integer3(p0 : Integer2, p1 : Integer)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> |p1|[integer](integer.md)| |
> ```TS:Nada
> function Set(p0 : Integer, p1 : Integer)
> ``` 


---  
 

 
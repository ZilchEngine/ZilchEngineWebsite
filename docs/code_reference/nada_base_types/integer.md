 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Get](integer.md#get-zilch-engine-document)|[ Count](integer.md#count-zilch-engine-docume)| | |
|[ GetAxis](integer.md#getaxis-zilch-engine-docu)|[ NegativeMin](integer.md#negativemin-zilch-engine)| | |
|[ Constructor](integer.md#integer-void)|[ NegativeValueClosestToZero](integer.md#negativevalueclosesttoze)| | |
|[ Parse](integer.md#parse-zilch-engine-docume)|[ One](integer.md#one-zilch-engine-document)| | |
|[ Reinterpret](integer.md#reinterpret-zilch-engine)|[ PositiveMax](integer.md#positivemax-zilch-engine)| | |
|[ Set](integer.md#set-void)|[ PositiveValueClosestToZero](integer.md#positivevalueclosesttoze)| | |
| |[ XAxis](integer.md#xaxis-zilch-engine-docume)| | |
| |[ Zero](integer.md#zilch-zilch-engine-documen)| | |


 #  Properties


---  
 #  Count : [integer](integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Count : Integer


---  
 #  NegativeMin : [integer](integer.md)

 `read-only` `static`

> The smallest (most negative) value that can be represented by an Integer.
> ``` lang=cpp, name=Nada
> var NegativeMin : Integer


---  
 #  NegativeValueClosestToZero : [integer](integer.md)

 `read-only` `static`

> The negative value closest to zero that can be represented by an Integer.
> ``` lang=cpp, name=Nada
> var NegativeValueClosestToZero : Integer


---  
 #  One : [integer](integer.md)

 `read-only` `static`

> The one vector (a vector containing all ones).
> ``` lang=cpp, name=Nada
> var One : Integer


---  
 #  PositiveMax : [integer](integer.md)

 `read-only` `static`

> The largest (most positive) value that can be represented by an Integer.
> ``` lang=cpp, name=Nada
> var PositiveMax : Integer


---  
 #  PositiveValueClosestToZero : [integer](integer.md)

 `read-only` `static`

> The positive value closest to zero that can be represented by an Integer.
> ``` lang=cpp, name=Nada
> var PositiveValueClosestToZero : Integer


---  
 #  XAxis : [integer](integer.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var XAxis : Integer


---  
 #  Zero : [integer](integer.md)

 `read-only` `static`

> The zero vector (a vector containing all zeroes).
> ``` lang=cpp, name=Nada
> var Zero : Integer


---  
 #  Methods


---  
 #  Get : [integer](integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function Get(p0 : Integer) : Integer
> ``` 


---  
 #  GetAxis : [integer](integer.md)

 `static`

> Returns an axis vector from the given index (ie. 0 is XAxis, 1 is YAxis, etc...
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function GetAxis(p0 : Integer) : Integer
> ``` 


---  
 #  Integer : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Integer()
> ``` 


---  
 #  Integer : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |scalar|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function Integer(scalar : Integer)
> ``` 


---  
 #  Parse : [integer](integer.md)

 `static`

> Attempt to convert the given StringRange to an Integer. If parsing fails 0 is returned.
> |Name|Type|Description|
> |---|---|---|
> |p0|[stringrange](stringrange.md)| |
> ``` lang=cpp, name=Nada
> function Parse(p0 : StringRange) : Integer
> ``` 


---  
 #  Reinterpret : [integer](integer.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real](real.md)| |
> ``` lang=cpp, name=Nada
> function Reinterpret(p0 : Real) : Integer
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> |p1|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function Set(p0 : Integer, p1 : Integer)
> ``` 


---  
 

 
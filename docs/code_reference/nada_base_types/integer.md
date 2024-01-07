 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Get](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md#get-zilch-engine-document)|[ Count](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md#count-zilch-engine-docume)| | |
|[ GetAxis](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md#getaxis-zilch-engine-docu)|[ NegativeMin](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md#negativemin-zilch-engine)| | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md#integer-void)|[ NegativeValueClosestToZero](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md#negativevalueclosesttoze)| | |
|[ Parse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md#parse-zilch-engine-docume)|[ One](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md#one-zilch-engine-document)| | |
|[ Reinterpret](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md#reinterpret-zilch-engine)|[ PositiveMax](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md#positivemax-zilch-engine)| | |
|[ Set](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md#set-void)|[ PositiveValueClosestToZero](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md#positivevalueclosesttoze)| | |
| |[ XAxis](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md#xaxis-zilch-engine-docume)| | |
| |[ Zero](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md#zilch-zilch-engine-documen)| | |


 #  Properties


---  
 #  Count : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Count : Integer


---  
 #  NegativeMin : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only` `static`

> The smallest (most negative) value that can be represented by an Integer.
> ``` lang=cpp, name=Nada
> var NegativeMin : Integer


---  
 #  NegativeValueClosestToZero : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only` `static`

> The negative value closest to zero that can be represented by an Integer.
> ``` lang=cpp, name=Nada
> var NegativeValueClosestToZero : Integer


---  
 #  One : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only` `static`

> The one vector (a vector containing all ones).
> ``` lang=cpp, name=Nada
> var One : Integer


---  
 #  PositiveMax : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only` `static`

> The largest (most positive) value that can be represented by an Integer.
> ``` lang=cpp, name=Nada
> var PositiveMax : Integer


---  
 #  PositiveValueClosestToZero : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only` `static`

> The positive value closest to zero that can be represented by an Integer.
> ``` lang=cpp, name=Nada
> var PositiveValueClosestToZero : Integer


---  
 #  XAxis : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var XAxis : Integer


---  
 #  Zero : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only` `static`

> The zero vector (a vector containing all zeroes).
> ``` lang=cpp, name=Nada
> var Zero : Integer


---  
 #  Methods


---  
 #  Get : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Get(p0 : Integer) : Integer
> ``` 


---  
 #  GetAxis : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `static`

> Returns an axis vector from the given index (ie. 0 is XAxis, 1 is YAxis, etc...
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
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
> |scalar|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Integer(scalar : Integer)
> ``` 


---  
 #  Parse : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `static`

> Attempt to convert the given StringRange to an Integer. If parsing fails 0 is returned.
> |Name|Type|Description|
> |---|---|---|
> |p0|[stringrange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/stringrange.md)| |
> ``` lang=cpp, name=Nada
> function Parse(p0 : StringRange) : Integer
> ``` 


---  
 #  Reinterpret : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function Reinterpret(p0 : Real) : Integer
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |p1|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Set(p0 : Integer, p1 : Integer)
> ``` 


---  
 

 
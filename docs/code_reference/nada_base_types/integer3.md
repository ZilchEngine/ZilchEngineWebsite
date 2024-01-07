 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Get](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer3.md#get-zilch-engine-document)|[ Count](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer3.md#count-zilch-engine-docume)| | |
|[ GetAxis](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer3.md#getaxis-zilch-engine-docu)|[ NegativeMin](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer3.md#negativemin-zilch-engine)| | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer3.md#integer3-void)|[ NegativeValueClosestToZero](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer3.md#negativevalueclosesttoze)| | |
|[ Set](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer3.md#set-void)|[ One](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer3.md#one-zilch-engine-document)| | |
| |[ PositiveMax](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer3.md#positivemax-zilch-engine)| | |
| |[ PositiveValueClosestToZero](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer3.md#positivevalueclosesttoze)| | |
| |[ XAxis](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer3.md#xaxis-zilch-engine-docume)| | |
| |[ YAxis](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer3.md#yaxis-zilch-engine-docume)| | |
| |[ ZAxis](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer3.md#zaxis-zilch-engine-docume)| | |
| |[ Zero](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer3.md#zilch-zilch-engine-documen)| | |


 #  Properties


---  
 #  Count : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Count : Integer


---  
 #  NegativeMin : [integer3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer3.md)

 `read-only` `static`

> The smallest (most negative) value that can be represented by an Integer.
> ``` lang=cpp, name=Nada
> var NegativeMin : Integer3


---  
 #  NegativeValueClosestToZero : [integer3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer3.md)

 `read-only` `static`

> The negative value closest to zero that can be represented by an Integer.
> ``` lang=cpp, name=Nada
> var NegativeValueClosestToZero : Integer3


---  
 #  One : [integer3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer3.md)

 `read-only` `static`

> The one vector (a vector containing all ones).
> ``` lang=cpp, name=Nada
> var One : Integer3


---  
 #  PositiveMax : [integer3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer3.md)

 `read-only` `static`

> The largest (most positive) value that can be represented by an Integer.
> ``` lang=cpp, name=Nada
> var PositiveMax : Integer3


---  
 #  PositiveValueClosestToZero : [integer3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer3.md)

 `read-only` `static`

> The positive value closest to zero that can be represented by an Integer.
> ``` lang=cpp, name=Nada
> var PositiveValueClosestToZero : Integer3


---  
 #  XAxis : [integer3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer3.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var XAxis : Integer3


---  
 #  YAxis : [integer3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer3.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var YAxis : Integer3


---  
 #  ZAxis : [integer3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer3.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var ZAxis : Integer3


---  
 #  Zero : [integer3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer3.md)

 `read-only` `static`

> The zero vector (a vector containing all zeroes).
> ``` lang=cpp, name=Nada
> var Zero : Integer3


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
 #  GetAxis : [integer3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer3.md)

 `static`

> Returns an axis vector from the given index (ie. 0 is XAxis, 1 is YAxis, etc...
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function GetAxis(p0 : Integer) : Integer3
> ``` 


---  
 #  Integer3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Integer3()
> ``` 


---  
 #  Integer3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |scalar|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Integer3(scalar : Integer)
> ``` 


---  
 #  Integer3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |p1|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |p2|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Integer3(p0 : Integer, p1 : Integer, p2 : Integer)
> ``` 


---  
 #  Integer3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |p1|[integer2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md)| |
> ``` lang=cpp, name=Nada
> function Integer3(p0 : Integer, p1 : Integer2)
> ``` 


---  
 #  Integer3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md)| |
> |p1|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Integer3(p0 : Integer2, p1 : Integer)
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
 

 
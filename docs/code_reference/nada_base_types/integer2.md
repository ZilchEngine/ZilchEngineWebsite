 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Get](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md#get-zilch-engine-document)|[ Count](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md#count-zilch-engine-docume)| | |
|[ GetAxis](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md#getaxis-zilch-engine-docu)|[ NegativeMin](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md#negativemin-zilch-engine)| | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md#integer2-void)|[ NegativeValueClosestToZero](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md#negativevalueclosesttoze)| | |
|[ Set](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md#set-void)|[ One](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md#one-zilch-engine-document)| | |
| |[ PositiveMax](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md#positivemax-zilch-engine)| | |
| |[ PositiveValueClosestToZero](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md#positivevalueclosesttoze)| | |
| |[ XAxis](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md#xaxis-zilch-engine-docume)| | |
| |[ YAxis](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md#yaxis-zilch-engine-docume)| | |
| |[ Zero](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md#zilch-zilch-engine-documen)| | |


 #  Properties


---  
 #  Count : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Count : Integer


---  
 #  NegativeMin : [integer2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md)

 `read-only` `static`

> The smallest (most negative) value that can be represented by an Integer.
> ``` lang=cpp, name=Nada
> var NegativeMin : Integer2


---  
 #  NegativeValueClosestToZero : [integer2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md)

 `read-only` `static`

> The negative value closest to zero that can be represented by an Integer.
> ``` lang=cpp, name=Nada
> var NegativeValueClosestToZero : Integer2


---  
 #  One : [integer2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md)

 `read-only` `static`

> The one vector (a vector containing all ones).
> ``` lang=cpp, name=Nada
> var One : Integer2


---  
 #  PositiveMax : [integer2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md)

 `read-only` `static`

> The largest (most positive) value that can be represented by an Integer.
> ``` lang=cpp, name=Nada
> var PositiveMax : Integer2


---  
 #  PositiveValueClosestToZero : [integer2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md)

 `read-only` `static`

> The positive value closest to zero that can be represented by an Integer.
> ``` lang=cpp, name=Nada
> var PositiveValueClosestToZero : Integer2


---  
 #  XAxis : [integer2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var XAxis : Integer2


---  
 #  YAxis : [integer2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var YAxis : Integer2


---  
 #  Zero : [integer2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md)

 `read-only` `static`

> The zero vector (a vector containing all zeroes).
> ``` lang=cpp, name=Nada
> var Zero : Integer2


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
 #  GetAxis : [integer2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md)

 `static`

> Returns an axis vector from the given index (ie. 0 is XAxis, 1 is YAxis, etc...
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function GetAxis(p0 : Integer) : Integer2
> ``` 


---  
 #  Integer2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Integer2()
> ``` 


---  
 #  Integer2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |scalar|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Integer2(scalar : Integer)
> ``` 


---  
 #  Integer2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |p1|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Integer2(p0 : Integer, p1 : Integer)
> ``` 


---  
 #  Integer2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md)| |
> ``` lang=cpp, name=Nada
> function Integer2(p0 : Integer2)
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
 

 
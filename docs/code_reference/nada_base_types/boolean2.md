 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean2.md#boolean2-void)|[ Count](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean2.md#count-zilch-engine-docume)| | |
|[ Get](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean2.md#get-zilch-engine-document)|[ One](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean2.md#one-zilch-engine-document)| | |
|[ GetAxis](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean2.md#getaxis-zilch-engine-docu)|[ XAxis](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean2.md#xaxis-zilch-engine-docume)| | |
|[ Set](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean2.md#set-void)|[ YAxis](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean2.md#yaxis-zilch-engine-docume)| | |
| |[ Zero](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean2.md#zilch-zilch-engine-documen)| | |


 #  Properties


---  
 #  Count : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Count : Integer


---  
 #  One : [boolean2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean2.md)

 `read-only` `static`

> The one vector (a vector containing all ones).
> ``` lang=cpp, name=Nada
> var One : Boolean2


---  
 #  XAxis : [boolean2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean2.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var XAxis : Boolean2


---  
 #  YAxis : [boolean2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean2.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var YAxis : Boolean2


---  
 #  Zero : [boolean2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean2.md)

 `read-only` `static`

> The zero vector (a vector containing all zeroes).
> ``` lang=cpp, name=Nada
> var Zero : Boolean2


---  
 #  Methods


---  
 #  Boolean2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Boolean2()
> ``` 


---  
 #  Boolean2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |scalar|[boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)| |
> ``` lang=cpp, name=Nada
> function Boolean2(scalar : Boolean)
> ``` 


---  
 #  Boolean2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)| |
> |p1|[boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)| |
> ``` lang=cpp, name=Nada
> function Boolean2(p0 : Boolean, p1 : Boolean)
> ``` 


---  
 #  Boolean2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[boolean2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean2.md)| |
> ``` lang=cpp, name=Nada
> function Boolean2(p0 : Boolean2)
> ``` 


---  
 #  Get : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Get(p0 : Integer) : Boolean
> ``` 


---  
 #  GetAxis : [boolean2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean2.md)

 `static`

> Returns an axis vector from the given index (ie. 0 is XAxis, 1 is YAxis, etc...
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function GetAxis(p0 : Integer) : Boolean2
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |p1|[boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)| |
> ``` lang=cpp, name=Nada
> function Set(p0 : Integer, p1 : Boolean)
> ``` 


---  
 

 
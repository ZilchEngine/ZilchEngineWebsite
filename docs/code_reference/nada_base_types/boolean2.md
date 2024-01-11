 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](boolean2.md#boolean2-void)|[ Count](boolean2.md#count-zilch-engine-docume)| | |
|[ Get](boolean2.md#get-zilch-engine-document)|[ One](boolean2.md#one-zilch-engine-document)| | |
|[ GetAxis](boolean2.md#getaxis-zilch-engine-docu)|[ XAxis](boolean2.md#xaxis-zilch-engine-docume)| | |
|[ Set](boolean2.md#set-void)|[ YAxis](boolean2.md#yaxis-zilch-engine-docume)| | |
| |[ Zero](boolean2.md#zilch-zilch-engine-documen)| | |


 #  Properties


---  
 #  Count : [integer](integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Count : Integer


---  
 #  One : [boolean2](boolean2.md)

 `read-only` `static`

> The one vector (a vector containing all ones).
> ``` lang=cpp, name=Nada
> var One : Boolean2


---  
 #  XAxis : [boolean2](boolean2.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var XAxis : Boolean2


---  
 #  YAxis : [boolean2](boolean2.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var YAxis : Boolean2


---  
 #  Zero : [boolean2](boolean2.md)

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
> |scalar|[boolean](boolean.md)| |
> ``` lang=cpp, name=Nada
> function Boolean2(scalar : Boolean)
> ``` 


---  
 #  Boolean2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[boolean](boolean.md)| |
> |p1|[boolean](boolean.md)| |
> ``` lang=cpp, name=Nada
> function Boolean2(p0 : Boolean, p1 : Boolean)
> ``` 


---  
 #  Boolean2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[boolean2](boolean2.md)| |
> ``` lang=cpp, name=Nada
> function Boolean2(p0 : Boolean2)
> ``` 


---  
 #  Get : [boolean](boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function Get(p0 : Integer) : Boolean
> ``` 


---  
 #  GetAxis : [boolean2](boolean2.md)

 `static`

> Returns an axis vector from the given index (ie. 0 is XAxis, 1 is YAxis, etc...
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function GetAxis(p0 : Integer) : Boolean2
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> |p1|[boolean](boolean.md)| |
> ``` lang=cpp, name=Nada
> function Set(p0 : Integer, p1 : Boolean)
> ``` 


---  
 

 
 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](boolean.md#boolean-void)|[ Count](boolean.md#count-zilch-engine-docume)| | |
|[ Get](boolean.md#get-zilch-engine-document)|[ One](boolean.md#one-zilch-engine-document)| | |
|[ GetAxis](boolean.md#getaxis-zilch-engine-docu)|[ XAxis](boolean.md#xaxis-zilch-engine-docume)| | |
|[ Set](boolean.md#set-void)|[ Zero](boolean.md#zilch-zilch-engine-documen)| | |


 #  Properties


---  
 #  Count : [integer](integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Count : Integer


---  
 #  One : [boolean](boolean.md)

 `read-only` `static`

> The one vector (a vector containing all ones).
> ``` lang=cpp, name=Nada
> var One : Boolean


---  
 #  XAxis : [boolean](boolean.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var XAxis : Boolean


---  
 #  Zero : [boolean](boolean.md)

 `read-only` `static`

> The zero vector (a vector containing all zeroes).
> ``` lang=cpp, name=Nada
> var Zero : Boolean


---  
 #  Methods


---  
 #  Boolean : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Boolean()
> ``` 


---  
 #  Boolean : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |scalar|[boolean](boolean.md)| |
> ``` lang=cpp, name=Nada
> function Boolean(scalar : Boolean)
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
 #  GetAxis : [boolean](boolean.md)

 `static`

> Returns an axis vector from the given index (ie. 0 is XAxis, 1 is YAxis, etc...
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function GetAxis(p0 : Integer) : Boolean
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
 

 
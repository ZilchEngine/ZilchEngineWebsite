 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](boolean3.md#boolean3-void)|[Count](boolean3.md#count-zilch-engine-docume)| | |
|[Get](boolean3.md#get-zilch-engine-document)|[One](boolean3.md#one-zilch-engine-document)| | |
|[GetAxis](boolean3.md#getaxis-zilch-engine-docu)|[XAxis](boolean3.md#xaxis-zilch-engine-docume)| | |
|[Set](boolean3.md#set-void)|[YAxis](boolean3.md#yaxis-zilch-engine-docume)| | |
| |[ZAxis](boolean3.md#zaxis-zilch-engine-docume)| | |
| |[Zero](boolean3.md#zilch-zilch-engine-documen)| | |


 #  Properties


---  
 #  Count : [integer](integer.md)

 `read-only`

> 
> ```TS:Nada
> var Count : Integer


---  
 #  One : [boolean3](boolean3.md)

 `read-only` `static`

> The one vector (a vector containing all ones).
> ```TS:Nada
> var One : Boolean3


---  
 #  XAxis : [boolean3](boolean3.md)

 `read-only` `static`

> 
> ```TS:Nada
> var XAxis : Boolean3


---  
 #  YAxis : [boolean3](boolean3.md)

 `read-only` `static`

> 
> ```TS:Nada
> var YAxis : Boolean3


---  
 #  ZAxis : [boolean3](boolean3.md)

 `read-only` `static`

> 
> ```TS:Nada
> var ZAxis : Boolean3


---  
 #  Zero : [boolean3](boolean3.md)

 `read-only` `static`

> The zero vector (a vector containing all zeroes).
> ```TS:Nada
> var Zero : Boolean3


---  
 #  Methods


---  
 #  Boolean3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Boolean3()
> ``` 


---  
 #  Boolean3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |scalar|[boolean](boolean.md)| |
> ```TS:Nada
> function Boolean3(scalar : Boolean)
> ``` 


---  
 #  Boolean3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[boolean](boolean.md)| |
> |p1|[boolean](boolean.md)| |
> |p2|[boolean](boolean.md)| |
> ```TS:Nada
> function Boolean3(p0 : Boolean, p1 : Boolean, p2 : Boolean)
> ``` 


---  
 #  Boolean3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[boolean](boolean.md)| |
> |p1|[boolean2](boolean2.md)| |
> ```TS:Nada
> function Boolean3(p0 : Boolean, p1 : Boolean2)
> ``` 


---  
 #  Boolean3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[boolean2](boolean2.md)| |
> |p1|[boolean](boolean.md)| |
> ```TS:Nada
> function Boolean3(p0 : Boolean2, p1 : Boolean)
> ``` 


---  
 #  Get : [boolean](boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> ```TS:Nada
> function Get(p0 : Integer) : Boolean
> ``` 


---  
 #  GetAxis : [boolean3](boolean3.md)

 `static`

> Returns an axis vector from the given index (ie. 0 is XAxis, 1 is YAxis, etc...
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> ```TS:Nada
> function GetAxis(p0 : Integer) : Boolean3
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> |p1|[boolean](boolean.md)| |
> ```TS:Nada
> function Set(p0 : Integer, p1 : Boolean)
> ``` 


---  
 

 
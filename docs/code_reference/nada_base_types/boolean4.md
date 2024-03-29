 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](boolean4.md#boolean4-void)|[Count](boolean4.md#count-zilch-engine-docume)| | |
|[Get](boolean4.md#get-zilch-engine-document)|[One](boolean4.md#one-zilch-engine-document)| | |
|[GetAxis](boolean4.md#getaxis-zilch-engine-docu)|[WAxis](boolean4.md#waxis-zilch-engine-docume)| | |
|[Set](boolean4.md#set-void)|[XAxis](boolean4.md#xaxis-zilch-engine-docume)| | |
| |[YAxis](boolean4.md#yaxis-zilch-engine-docume)| | |
| |[ZAxis](boolean4.md#zaxis-zilch-engine-docume)| | |
| |[Zero](boolean4.md#zilch-zilch-engine-documen)| | |


 #  Properties


---  
 #  Count : [integer](integer.md)

 `read-only`

> 
> ```TS:Nada
> var Count : Integer


---  
 #  One : [boolean4](boolean4.md)

 `read-only` `static`

> The one vector (a vector containing all ones).
> ```TS:Nada
> var One : Boolean4


---  
 #  WAxis : [boolean4](boolean4.md)

 `read-only` `static`

> 
> ```TS:Nada
> var WAxis : Boolean4


---  
 #  XAxis : [boolean4](boolean4.md)

 `read-only` `static`

> 
> ```TS:Nada
> var XAxis : Boolean4


---  
 #  YAxis : [boolean4](boolean4.md)

 `read-only` `static`

> 
> ```TS:Nada
> var YAxis : Boolean4


---  
 #  ZAxis : [boolean4](boolean4.md)

 `read-only` `static`

> 
> ```TS:Nada
> var ZAxis : Boolean4


---  
 #  Zero : [boolean4](boolean4.md)

 `read-only` `static`

> The zero vector (a vector containing all zeroes).
> ```TS:Nada
> var Zero : Boolean4


---  
 #  Methods


---  
 #  Boolean4 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Boolean4()
> ``` 


---  
 #  Boolean4 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |scalar|[boolean](boolean.md)| |
> ```TS:Nada
> function Boolean4(scalar : Boolean)
> ``` 


---  
 #  Boolean4 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[boolean](boolean.md)| |
> |p1|[boolean](boolean.md)| |
> |p2|[boolean](boolean.md)| |
> |p3|[boolean](boolean.md)| |
> ```TS:Nada
> function Boolean4(p0 : Boolean, p1 : Boolean, p2 : Boolean, p3 : Boolean)
> ``` 


---  
 #  Boolean4 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[boolean](boolean.md)| |
> |p1|[boolean](boolean.md)| |
> |p2|[boolean2](boolean2.md)| |
> ```TS:Nada
> function Boolean4(p0 : Boolean, p1 : Boolean, p2 : Boolean2)
> ``` 


---  
 #  Boolean4 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[boolean](boolean.md)| |
> |p1|[boolean2](boolean2.md)| |
> |p2|[boolean](boolean.md)| |
> ```TS:Nada
> function Boolean4(p0 : Boolean, p1 : Boolean2, p2 : Boolean)
> ``` 


---  
 #  Boolean4 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[boolean](boolean.md)| |
> |p1|[boolean3](boolean3.md)| |
> ```TS:Nada
> function Boolean4(p0 : Boolean, p1 : Boolean3)
> ``` 


---  
 #  Boolean4 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[boolean2](boolean2.md)| |
> |p1|[boolean](boolean.md)| |
> |p2|[boolean](boolean.md)| |
> ```TS:Nada
> function Boolean4(p0 : Boolean2, p1 : Boolean, p2 : Boolean)
> ``` 


---  
 #  Boolean4 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[boolean2](boolean2.md)| |
> |p1|[boolean2](boolean2.md)| |
> ```TS:Nada
> function Boolean4(p0 : Boolean2, p1 : Boolean2)
> ``` 


---  
 #  Boolean4 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[boolean3](boolean3.md)| |
> |p1|[boolean](boolean.md)| |
> ```TS:Nada
> function Boolean4(p0 : Boolean3, p1 : Boolean)
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
 #  GetAxis : [boolean4](boolean4.md)

 `static`

> Returns an axis vector from the given index (ie. 0 is XAxis, 1 is YAxis, etc...
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> ```TS:Nada
> function GetAxis(p0 : Integer) : Boolean4
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
 

 
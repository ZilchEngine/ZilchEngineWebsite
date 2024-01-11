 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Get](integer2x3.md#get-zilch-engine-document)|[ Count](integer2x3.md#count-zilch-engine-docume)| | |
|[ GetByIndex](integer2x3.md#getbyindex-zilch-engine-d)|[ CountX](integer2x3.md#countx-zilch-engine-docum)| | |
|[ Constructor](integer2x3.md#integer2x3-void)|[ CountY](integer2x3.md#county-zilch-engine-docum)| | |
|[ Set](integer2x3.md#set-void)|[ M00](integer2x3.md#m00-zilch-engine-document)| | |
|[ SetByIndex](integer2x3.md#setbyindex-void)|[ M01](integer2x3.md#m01-zilch-engine-document)| | |
| |[ M02](integer2x3.md#m02-zilch-engine-document)| | |
| |[ M10](integer2x3.md#m10-zilch-engine-document)| | |
| |[ M11](integer2x3.md#m11-zilch-engine-document)| | |
| |[ M12](integer2x3.md#m12-zilch-engine-document)| | |


 #  Properties


---  
 #  Count : [integer](integer.md)

 `read-only`

> 
> ```TS:Nada
> var Count : Integer


---  
 #  CountX : [integer](integer.md)

 `read-only`

> 
> ```TS:Nada
> var CountX : Integer


---  
 #  CountY : [integer](integer.md)

 `read-only`

> 
> ```TS:Nada
> var CountY : Integer


---  
 #  M00 : [integer](integer.md)

> 
> ```TS:Nada
> var M00 : Integer


---  
 #  M01 : [integer](integer.md)

> 
> ```TS:Nada
> var M01 : Integer


---  
 #  M02 : [integer](integer.md)

> 
> ```TS:Nada
> var M02 : Integer


---  
 #  M10 : [integer](integer.md)

> 
> ```TS:Nada
> var M10 : Integer


---  
 #  M11 : [integer](integer.md)

> 
> ```TS:Nada
> var M11 : Integer


---  
 #  M12 : [integer](integer.md)

> 
> ```TS:Nada
> var M12 : Integer


---  
 #  Methods


---  
 #  Get : [integer3](integer3.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](integer.md)| |
> ```TS:Nada
> function Get(y : Integer) : Integer3
> ``` 


---  
 #  Get : [integer](integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](integer.md)| |
> |x|[integer](integer.md)| |
> ```TS:Nada
> function Get(y : Integer, x : Integer) : Integer
> ``` 


---  
 #  GetByIndex : [integer](integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](integer.md)| |
> ```TS:Nada
> function GetByIndex(index : Integer) : Integer
> ``` 


---  
 #  Integer2x3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Integer2x3()
> ``` 


---  
 #  Integer2x3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> ```TS:Nada
> function Integer2x3(p0 : Integer)
> ``` 


---  
 #  Integer2x3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |m00|[integer](integer.md)| |
> |m01|[integer](integer.md)| |
> |m02|[integer](integer.md)| |
> |m10|[integer](integer.md)| |
> |m11|[integer](integer.md)| |
> |m12|[integer](integer.md)| |
> ```TS:Nada
> function Integer2x3(m00 : Integer, m01 : Integer, m02 : Integer, m10 : Integer, m11 : Integer, m12 : Integer)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](integer.md)| |
> |x|[integer](integer.md)| |
> |value|[integer](integer.md)| |
> ```TS:Nada
> function Set(y : Integer, x : Integer, value : Integer)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](integer.md)| |
> |value|[integer3](integer3.md)| |
> ```TS:Nada
> function Set(y : Integer, value : Integer3)
> ``` 


---  
 #  SetByIndex : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](integer.md)| |
> |value|[integer](integer.md)| |
> ```TS:Nada
> function SetByIndex(index : Integer, value : Integer)
> ``` 


---  
 

 
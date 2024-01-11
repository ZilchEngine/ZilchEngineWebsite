 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](boolean2x2.md#boolean2x2-void)|[ Count](boolean2x2.md#count-zilch-engine-docume)| | |
|[ Get](boolean2x2.md#get-zilch-engine-document)|[ CountX](boolean2x2.md#countx-zilch-engine-docum)| | |
|[ GetByIndex](boolean2x2.md#getbyindex-zilch-engine-d)|[ CountY](boolean2x2.md#county-zilch-engine-docum)| | |
|[ Set](boolean2x2.md#set-void)|[ M00](boolean2x2.md#m00-zilch-engine-document)| | |
|[ SetByIndex](boolean2x2.md#setbyindex-void)|[ M01](boolean2x2.md#m01-zilch-engine-document)| | |
| |[ M10](boolean2x2.md#m10-zilch-engine-document)| | |
| |[ M11](boolean2x2.md#m11-zilch-engine-document)| | |


 #  Properties


---  
 #  Count : [integer](integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Count : Integer


---  
 #  CountX : [integer](integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var CountX : Integer


---  
 #  CountY : [integer](integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var CountY : Integer


---  
 #  M00 : [boolean](boolean.md)

> 
> ``` lang=cpp, name=Nada
> var M00 : Boolean


---  
 #  M01 : [boolean](boolean.md)

> 
> ``` lang=cpp, name=Nada
> var M01 : Boolean


---  
 #  M10 : [boolean](boolean.md)

> 
> ``` lang=cpp, name=Nada
> var M10 : Boolean


---  
 #  M11 : [boolean](boolean.md)

> 
> ``` lang=cpp, name=Nada
> var M11 : Boolean


---  
 #  Methods


---  
 #  Boolean2x2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Boolean2x2()
> ``` 


---  
 #  Boolean2x2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[boolean](boolean.md)| |
> ``` lang=cpp, name=Nada
> function Boolean2x2(p0 : Boolean)
> ``` 


---  
 #  Boolean2x2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |m00|[boolean](boolean.md)| |
> |m01|[boolean](boolean.md)| |
> |m10|[boolean](boolean.md)| |
> |m11|[boolean](boolean.md)| |
> ``` lang=cpp, name=Nada
> function Boolean2x2(m00 : Boolean, m01 : Boolean, m10 : Boolean, m11 : Boolean)
> ``` 


---  
 #  Get : [boolean2](boolean2.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function Get(y : Integer) : Boolean2
> ``` 


---  
 #  Get : [boolean](boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](integer.md)| |
> |x|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function Get(y : Integer, x : Integer) : Boolean
> ``` 


---  
 #  GetByIndex : [boolean](boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function GetByIndex(index : Integer) : Boolean
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](integer.md)| |
> |value|[boolean2](boolean2.md)| |
> ``` lang=cpp, name=Nada
> function Set(y : Integer, value : Boolean2)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](integer.md)| |
> |x|[integer](integer.md)| |
> |value|[boolean](boolean.md)| |
> ``` lang=cpp, name=Nada
> function Set(y : Integer, x : Integer, value : Boolean)
> ``` 


---  
 #  SetByIndex : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](integer.md)| |
> |value|[boolean](boolean.md)| |
> ``` lang=cpp, name=Nada
> function SetByIndex(index : Integer, value : Boolean)
> ``` 


---  
 

 
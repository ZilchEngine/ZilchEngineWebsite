 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Get](integer2x2.md#get-zilch-engine-document)|[ Count](integer2x2.md#count-zilch-engine-docume)| | |
|[ GetByIndex](integer2x2.md#getbyindex-zilch-engine-d)|[ CountX](integer2x2.md#countx-zilch-engine-docum)| | |
|[ Constructor](integer2x2.md#integer2x2-void)|[ CountY](integer2x2.md#county-zilch-engine-docum)| | |
|[ Set](integer2x2.md#set-void)|[ M00](integer2x2.md#m00-zilch-engine-document)| | |
|[ SetByIndex](integer2x2.md#setbyindex-void)|[ M01](integer2x2.md#m01-zilch-engine-document)| | |
| |[ M10](integer2x2.md#m10-zilch-engine-document)| | |
| |[ M11](integer2x2.md#m11-zilch-engine-document)| | |


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
 #  M00 : [integer](integer.md)

> 
> ``` lang=cpp, name=Nada
> var M00 : Integer


---  
 #  M01 : [integer](integer.md)

> 
> ``` lang=cpp, name=Nada
> var M01 : Integer


---  
 #  M10 : [integer](integer.md)

> 
> ``` lang=cpp, name=Nada
> var M10 : Integer


---  
 #  M11 : [integer](integer.md)

> 
> ``` lang=cpp, name=Nada
> var M11 : Integer


---  
 #  Methods


---  
 #  Get : [integer2](integer2.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function Get(y : Integer) : Integer2
> ``` 


---  
 #  Get : [integer](integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](integer.md)| |
> |x|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function Get(y : Integer, x : Integer) : Integer
> ``` 


---  
 #  GetByIndex : [integer](integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function GetByIndex(index : Integer) : Integer
> ``` 


---  
 #  Integer2x2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Integer2x2()
> ``` 


---  
 #  Integer2x2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function Integer2x2(p0 : Integer)
> ``` 


---  
 #  Integer2x2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |m00|[integer](integer.md)| |
> |m01|[integer](integer.md)| |
> |m10|[integer](integer.md)| |
> |m11|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function Integer2x2(m00 : Integer, m01 : Integer, m10 : Integer, m11 : Integer)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](integer.md)| |
> |x|[integer](integer.md)| |
> |value|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function Set(y : Integer, x : Integer, value : Integer)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](integer.md)| |
> |value|[integer2](integer2.md)| |
> ``` lang=cpp, name=Nada
> function Set(y : Integer, value : Integer2)
> ``` 


---  
 #  SetByIndex : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](integer.md)| |
> |value|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function SetByIndex(index : Integer, value : Integer)
> ``` 


---  
 

 
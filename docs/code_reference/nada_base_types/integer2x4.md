 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Get](integer2x4.md#get-zilch-engine-document)|[ Count](integer2x4.md#count-zilch-engine-docume)| | |
|[ GetByIndex](integer2x4.md#getbyindex-zilch-engine-d)|[ CountX](integer2x4.md#countx-zilch-engine-docum)| | |
|[ Constructor](integer2x4.md#integer2x4-void)|[ CountY](integer2x4.md#county-zilch-engine-docum)| | |
|[ Set](integer2x4.md#set-void)|[ M00](integer2x4.md#m00-zilch-engine-document)| | |
|[ SetByIndex](integer2x4.md#setbyindex-void)|[ M01](integer2x4.md#m01-zilch-engine-document)| | |
| |[ M02](integer2x4.md#m02-zilch-engine-document)| | |
| |[ M03](integer2x4.md#m03-zilch-engine-document)| | |
| |[ M10](integer2x4.md#m10-zilch-engine-document)| | |
| |[ M11](integer2x4.md#m11-zilch-engine-document)| | |
| |[ M12](integer2x4.md#m12-zilch-engine-document)| | |
| |[ M13](integer2x4.md#m13-zilch-engine-document)| | |


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
 #  M02 : [integer](integer.md)

> 
> ``` lang=cpp, name=Nada
> var M02 : Integer


---  
 #  M03 : [integer](integer.md)

> 
> ``` lang=cpp, name=Nada
> var M03 : Integer


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
 #  M12 : [integer](integer.md)

> 
> ``` lang=cpp, name=Nada
> var M12 : Integer


---  
 #  M13 : [integer](integer.md)

> 
> ``` lang=cpp, name=Nada
> var M13 : Integer


---  
 #  Methods


---  
 #  Get : [integer4](integer4.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function Get(y : Integer) : Integer4
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
 #  Integer2x4 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Integer2x4()
> ``` 


---  
 #  Integer2x4 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function Integer2x4(p0 : Integer)
> ``` 


---  
 #  Integer2x4 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |m00|[integer](integer.md)| |
> |m01|[integer](integer.md)| |
> |m02|[integer](integer.md)| |
> |m03|[integer](integer.md)| |
> |m10|[integer](integer.md)| |
> |m11|[integer](integer.md)| |
> |m12|[integer](integer.md)| |
> |m13|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function Integer2x4(m00 : Integer, m01 : Integer, m02 : Integer, m03 : Integer, m10 : Integer, m11 : Integer, m12 : Integer, m13 : Integer)
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
> |value|[integer4](integer4.md)| |
> ``` lang=cpp, name=Nada
> function Set(y : Integer, value : Integer4)
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
 

 
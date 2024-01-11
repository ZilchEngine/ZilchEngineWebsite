 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Get](real3x4.md#get-zilch-engine-document)|[ Count](real3x4.md#count-zilch-engine-docume)| | |
|[ GetByIndex](real3x4.md#getbyindex-zilch-engine-d)|[ CountX](real3x4.md#countx-zilch-engine-docum)| | |
|[ Constructor](real3x4.md#real3x4-void)|[ CountY](real3x4.md#county-zilch-engine-docum)| | |
|[ Set](real3x4.md#set-void)|[ M00](real3x4.md#m00-zilch-engine-document)| | |
|[ SetByIndex](real3x4.md#setbyindex-void)|[ M01](real3x4.md#m01-zilch-engine-document)| | |
| |[ M02](real3x4.md#m02-zilch-engine-document)| | |
| |[ M03](real3x4.md#m03-zilch-engine-document)| | |
| |[ M10](real3x4.md#m10-zilch-engine-document)| | |
| |[ M11](real3x4.md#m11-zilch-engine-document)| | |
| |[ M12](real3x4.md#m12-zilch-engine-document)| | |
| |[ M13](real3x4.md#m13-zilch-engine-document)| | |
| |[ M20](real3x4.md#m20-zilch-engine-document)| | |
| |[ M21](real3x4.md#m21-zilch-engine-document)| | |
| |[ M22](real3x4.md#m22-zilch-engine-document)| | |
| |[ M23](real3x4.md#m23-zilch-engine-document)| | |


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
 #  M00 : [real](real.md)

> 
> ``` lang=cpp, name=Nada
> var M00 : Real


---  
 #  M01 : [real](real.md)

> 
> ``` lang=cpp, name=Nada
> var M01 : Real


---  
 #  M02 : [real](real.md)

> 
> ``` lang=cpp, name=Nada
> var M02 : Real


---  
 #  M03 : [real](real.md)

> 
> ``` lang=cpp, name=Nada
> var M03 : Real


---  
 #  M10 : [real](real.md)

> 
> ``` lang=cpp, name=Nada
> var M10 : Real


---  
 #  M11 : [real](real.md)

> 
> ``` lang=cpp, name=Nada
> var M11 : Real


---  
 #  M12 : [real](real.md)

> 
> ``` lang=cpp, name=Nada
> var M12 : Real


---  
 #  M13 : [real](real.md)

> 
> ``` lang=cpp, name=Nada
> var M13 : Real


---  
 #  M20 : [real](real.md)

> 
> ``` lang=cpp, name=Nada
> var M20 : Real


---  
 #  M21 : [real](real.md)

> 
> ``` lang=cpp, name=Nada
> var M21 : Real


---  
 #  M22 : [real](real.md)

> 
> ``` lang=cpp, name=Nada
> var M22 : Real


---  
 #  M23 : [real](real.md)

> 
> ``` lang=cpp, name=Nada
> var M23 : Real


---  
 #  Methods


---  
 #  Get : [real4](real4.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function Get(y : Integer) : Real4
> ``` 


---  
 #  Get : [real](real.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](integer.md)| |
> |x|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function Get(y : Integer, x : Integer) : Real
> ``` 


---  
 #  GetByIndex : [real](real.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function GetByIndex(index : Integer) : Real
> ``` 


---  
 #  Real3x4 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Real3x4()
> ``` 


---  
 #  Real3x4 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real](real.md)| |
> ``` lang=cpp, name=Nada
> function Real3x4(p0 : Real)
> ``` 


---  
 #  Real3x4 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |m00|[real](real.md)| |
> |m01|[real](real.md)| |
> |m02|[real](real.md)| |
> |m03|[real](real.md)| |
> |m10|[real](real.md)| |
> |m11|[real](real.md)| |
> |m12|[real](real.md)| |
> |m13|[real](real.md)| |
> |m20|[real](real.md)| |
> |m21|[real](real.md)| |
> |m22|[real](real.md)| |
> |m23|[real](real.md)| |
> ``` lang=cpp, name=Nada
> function Real3x4(m00 : Real, m01 : Real, m02 : Real, m03 : Real, m10 : Real, m11 : Real, m12 : Real, m13 : Real, m20 : Real, m21 : Real, m22 : Real, m23 : Real)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](integer.md)| |
> |x|[integer](integer.md)| |
> |value|[real](real.md)| |
> ``` lang=cpp, name=Nada
> function Set(y : Integer, x : Integer, value : Real)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](integer.md)| |
> |value|[real4](real4.md)| |
> ``` lang=cpp, name=Nada
> function Set(y : Integer, value : Real4)
> ``` 


---  
 #  SetByIndex : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](integer.md)| |
> |value|[real](real.md)| |
> ``` lang=cpp, name=Nada
> function SetByIndex(index : Integer, value : Real)
> ``` 


---  
 

 
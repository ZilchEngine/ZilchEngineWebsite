 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Get](real3x3.md#get-zilch-engine-document)|[Count](real3x3.md#count-zilch-engine-docume)| | |
|[GetByIndex](real3x3.md#getbyindex-zilch-engine-d)|[CountX](real3x3.md#countx-zilch-engine-docum)| | |
|[Constructor](real3x3.md#real3x3-void)|[CountY](real3x3.md#county-zilch-engine-docum)| | |
|[Set](real3x3.md#set-void)|[M00](real3x3.md#m00-zilch-engine-document)| | |
|[SetByIndex](real3x3.md#setbyindex-void)|[M01](real3x3.md#m01-zilch-engine-document)| | |
| |[M02](real3x3.md#m02-zilch-engine-document)| | |
| |[M10](real3x3.md#m10-zilch-engine-document)| | |
| |[M11](real3x3.md#m11-zilch-engine-document)| | |
| |[M12](real3x3.md#m12-zilch-engine-document)| | |
| |[M20](real3x3.md#m20-zilch-engine-document)| | |
| |[M21](real3x3.md#m21-zilch-engine-document)| | |
| |[M22](real3x3.md#m22-zilch-engine-document)| | |


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
 #  M00 : [real](real.md)

> 
> ```TS:Nada
> var M00 : Real


---  
 #  M01 : [real](real.md)

> 
> ```TS:Nada
> var M01 : Real


---  
 #  M02 : [real](real.md)

> 
> ```TS:Nada
> var M02 : Real


---  
 #  M10 : [real](real.md)

> 
> ```TS:Nada
> var M10 : Real


---  
 #  M11 : [real](real.md)

> 
> ```TS:Nada
> var M11 : Real


---  
 #  M12 : [real](real.md)

> 
> ```TS:Nada
> var M12 : Real


---  
 #  M20 : [real](real.md)

> 
> ```TS:Nada
> var M20 : Real


---  
 #  M21 : [real](real.md)

> 
> ```TS:Nada
> var M21 : Real


---  
 #  M22 : [real](real.md)

> 
> ```TS:Nada
> var M22 : Real


---  
 #  Methods


---  
 #  Get : [real3](real3.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](integer.md)| |
> ```TS:Nada
> function Get(y : Integer) : Real3
> ``` 


---  
 #  Get : [real](real.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](integer.md)| |
> |x|[integer](integer.md)| |
> ```TS:Nada
> function Get(y : Integer, x : Integer) : Real
> ``` 


---  
 #  GetByIndex : [real](real.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](integer.md)| |
> ```TS:Nada
> function GetByIndex(index : Integer) : Real
> ``` 


---  
 #  Real3x3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Real3x3()
> ``` 


---  
 #  Real3x3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real](real.md)| |
> ```TS:Nada
> function Real3x3(p0 : Real)
> ``` 


---  
 #  Real3x3 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |m00|[real](real.md)| |
> |m01|[real](real.md)| |
> |m02|[real](real.md)| |
> |m10|[real](real.md)| |
> |m11|[real](real.md)| |
> |m12|[real](real.md)| |
> |m20|[real](real.md)| |
> |m21|[real](real.md)| |
> |m22|[real](real.md)| |
> ```TS:Nada
> function Real3x3(m00 : Real, m01 : Real, m02 : Real, m10 : Real, m11 : Real, m12 : Real, m20 : Real, m21 : Real, m22 : Real)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](integer.md)| |
> |x|[integer](integer.md)| |
> |value|[real](real.md)| |
> ```TS:Nada
> function Set(y : Integer, x : Integer, value : Real)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](integer.md)| |
> |value|[real3](real3.md)| |
> ```TS:Nada
> function Set(y : Integer, value : Real3)
> ``` 


---  
 #  SetByIndex : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](integer.md)| |
> |value|[real](real.md)| |
> ```TS:Nada
> function SetByIndex(index : Integer, value : Real)
> ``` 


---  
 

 
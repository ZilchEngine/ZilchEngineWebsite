 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Get](real4x2.md#get-zilch-engine-document)|[Count](real4x2.md#count-zilch-engine-docume)| | |
|[GetByIndex](real4x2.md#getbyindex-zilch-engine-d)|[CountX](real4x2.md#countx-zilch-engine-docum)| | |
|[Constructor](real4x2.md#real4x2-void)|[CountY](real4x2.md#county-zilch-engine-docum)| | |
|[Set](real4x2.md#set-void)|[M00](real4x2.md#m00-zilch-engine-document)| | |
|[SetByIndex](real4x2.md#setbyindex-void)|[M01](real4x2.md#m01-zilch-engine-document)| | |
| |[M10](real4x2.md#m10-zilch-engine-document)| | |
| |[M11](real4x2.md#m11-zilch-engine-document)| | |
| |[M20](real4x2.md#m20-zilch-engine-document)| | |
| |[M21](real4x2.md#m21-zilch-engine-document)| | |
| |[M30](real4x2.md#m30-zilch-engine-document)| | |
| |[M31](real4x2.md#m31-zilch-engine-document)| | |


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
 #  M30 : [real](real.md)

> 
> ```TS:Nada
> var M30 : Real


---  
 #  M31 : [real](real.md)

> 
> ```TS:Nada
> var M31 : Real


---  
 #  Methods


---  
 #  Get : [real2](real2.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](integer.md)| |
> ```TS:Nada
> function Get(y : Integer) : Real2
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
 #  Real4x2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Real4x2()
> ``` 


---  
 #  Real4x2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real](real.md)| |
> ```TS:Nada
> function Real4x2(p0 : Real)
> ``` 


---  
 #  Real4x2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |m00|[real](real.md)| |
> |m01|[real](real.md)| |
> |m10|[real](real.md)| |
> |m11|[real](real.md)| |
> |m20|[real](real.md)| |
> |m21|[real](real.md)| |
> |m30|[real](real.md)| |
> |m31|[real](real.md)| |
> ```TS:Nada
> function Real4x2(m00 : Real, m01 : Real, m10 : Real, m11 : Real, m20 : Real, m21 : Real, m30 : Real, m31 : Real)
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
> |value|[real2](real2.md)| |
> ```TS:Nada
> function Set(y : Integer, value : Real2)
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
 

 
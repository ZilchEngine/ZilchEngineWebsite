 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Get](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2x2.md#get-zilch-engine-document)|[ Count](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2x2.md#count-zilch-engine-docume)| | |
|[ GetByIndex](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2x2.md#getbyindex-zilch-engine-d)|[ CountX](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2x2.md#countx-zilch-engine-docum)| | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2x2.md#real2x2-void)|[ CountY](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2x2.md#county-zilch-engine-docum)| | |
|[ Set](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2x2.md#set-void)|[ M00](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2x2.md#m00-zilch-engine-document)| | |
|[ SetByIndex](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2x2.md#setbyindex-void)|[ M01](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2x2.md#m01-zilch-engine-document)| | |
| |[ M10](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2x2.md#m10-zilch-engine-document)| | |
| |[ M11](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2x2.md#m11-zilch-engine-document)| | |


 #  Properties


---  
 #  Count : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Count : Integer


---  
 #  CountX : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var CountX : Integer


---  
 #  CountY : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var CountY : Integer


---  
 #  M00 : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> 
> ``` lang=cpp, name=Nada
> var M00 : Real


---  
 #  M01 : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> 
> ``` lang=cpp, name=Nada
> var M01 : Real


---  
 #  M10 : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> 
> ``` lang=cpp, name=Nada
> var M10 : Real


---  
 #  M11 : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> 
> ``` lang=cpp, name=Nada
> var M11 : Real


---  
 #  Methods


---  
 #  Get : [real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Get(y : Integer) : Real2
> ``` 


---  
 #  Get : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |x|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Get(y : Integer, x : Integer) : Real
> ``` 


---  
 #  GetByIndex : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function GetByIndex(index : Integer) : Real
> ``` 


---  
 #  Real2x2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Real2x2()
> ``` 


---  
 #  Real2x2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function Real2x2(p0 : Real)
> ``` 


---  
 #  Real2x2 : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |m00|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |m01|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |m10|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |m11|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function Real2x2(m00 : Real, m01 : Real, m10 : Real, m11 : Real)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |x|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |value|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function Set(y : Integer, x : Integer, value : Real)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |y|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |value|[real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)| |
> ``` lang=cpp, name=Nada
> function Set(y : Integer, value : Real2)
> ``` 


---  
 #  SetByIndex : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |value|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function SetByIndex(index : Integer, value : Real)
> ``` 


---  
 

 
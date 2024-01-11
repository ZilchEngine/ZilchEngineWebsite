 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ IsA](type.md#isa-zilch-engine-document)|[ IsAny](type.md#isany-zilch-engine-docume)|[reflectionobject](reflectionobject.md)|[anytype](anytype.md)|
|[ IsCastableTo](type.md#iscastableto-zilch-engine)|[ IsDelegate](type.md#isdelegate-zilch-engine-d)| |[boundtype](boundtype.md)|
|[ IsRawCastableTo](type.md#israwcastableto-zilch-eng)|[ IsEnum](type.md#isenum-zilch-engine-docum)| |[delegatetype](delegatetype.md)|
| |[ IsEnumOrFlags](type.md#isenumorflags-zilch-engin)| |[indirectiontype](indirectiontype.md)|
| |[ IsFlags](type.md#isflags-zilch-engine-docu)| | |
| |[ IsHandle](type.md#ishandle-zilch-engine-doc)| | |
| |[ IsValue](type.md#isvalue-zilch-engine-docu)| | |
| |[ Library](type.md#library-zilch-engine-docu)| | |
| |[ Name](type.md#name-zilch-engine-documen)| | |


 #  Properties


---  
 #  IsAny : [boolean](boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var IsAny : Boolean


---  
 #  IsDelegate : [boolean](boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var IsDelegate : Boolean


---  
 #  IsEnum : [boolean](boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var IsEnum : Boolean


---  
 #  IsEnumOrFlags : [boolean](boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var IsEnumOrFlags : Boolean


---  
 #  IsFlags : [boolean](boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var IsFlags : Boolean


---  
 #  IsHandle : [boolean](boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var IsHandle : Boolean


---  
 #  IsValue : [boolean](boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var IsValue : Boolean


---  
 #  Library : [library](library.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Library : Library


---  
 #  Name : [string](string.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Name : String


---  
 #  Methods


---  
 #  IsA : [boolean](boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |baseType|[type](type.md)| |
> ``` lang=cpp, name=Nada
> function IsA(baseType : Type) : Boolean
> ``` 


---  
 #  IsCastableTo : [boolean](boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |toType|[type](type.md)| |
> ``` lang=cpp, name=Nada
> function IsCastableTo(toType : Type) : Boolean
> ``` 


---  
 #  IsRawCastableTo : [boolean](boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |toType|[type](type.md)| |
> ``` lang=cpp, name=Nada
> function IsRawCastableTo(toType : Type) : Boolean
> ``` 


---  
 

 
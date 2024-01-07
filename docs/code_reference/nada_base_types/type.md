 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ IsA](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/type.md#isa-zilch-engine-document)|[ IsAny](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/type.md#isany-zilch-engine-docume)|[reflectionobject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/reflectionobject.md)|[anytype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/anytype.md)|
|[ IsCastableTo](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/type.md#iscastableto-zilch-engine)|[ IsDelegate](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/type.md#isdelegate-zilch-engine-d)| |[boundtype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boundtype.md)|
|[ IsRawCastableTo](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/type.md#israwcastableto-zilch-eng)|[ IsEnum](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/type.md#isenum-zilch-engine-docum)| |[delegatetype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/delegatetype.md)|
| |[ IsEnumOrFlags](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/type.md#isenumorflags-zilch-engin)| |[indirectiontype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/indirectiontype.md)|
| |[ IsFlags](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/type.md#isflags-zilch-engine-docu)| | |
| |[ IsHandle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/type.md#ishandle-zilch-engine-doc)| | |
| |[ IsValue](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/type.md#isvalue-zilch-engine-docu)| | |
| |[ Library](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/type.md#library-zilch-engine-docu)| | |
| |[ Name](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/type.md#name-zilch-engine-documen)| | |


 #  Properties


---  
 #  IsAny : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var IsAny : Boolean


---  
 #  IsDelegate : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var IsDelegate : Boolean


---  
 #  IsEnum : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var IsEnum : Boolean


---  
 #  IsEnumOrFlags : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var IsEnumOrFlags : Boolean


---  
 #  IsFlags : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var IsFlags : Boolean


---  
 #  IsHandle : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var IsHandle : Boolean


---  
 #  IsValue : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var IsValue : Boolean


---  
 #  Library : [library](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/library.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Library : Library


---  
 #  Name : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Name : String


---  
 #  Methods


---  
 #  IsA : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |baseType|[type](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/type.md)| |
> ``` lang=cpp, name=Nada
> function IsA(baseType : Type) : Boolean
> ``` 


---  
 #  IsCastableTo : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |toType|[type](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/type.md)| |
> ``` lang=cpp, name=Nada
> function IsCastableTo(toType : Type) : Boolean
> ``` 


---  
 #  IsRawCastableTo : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |toType|[type](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/type.md)| |
> ``` lang=cpp, name=Nada
> function IsRawCastableTo(toType : Type) : Boolean
> ``` 


---  
 

 
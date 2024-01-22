 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[GetConstructor](boundtype.md#getconstructor-zilch-engi)|[BaseType](boundtype.md#basetype-zilch-engine-doc)|[type](type.md)| |
|[GetField](boundtype.md#getfield-zilch-engine-doc)|[DefaultConstructor](boundtype.md#defaultconstructor-zero)| | |
|[GetFunction](boundtype.md#getfunction-zilch-engine)|[Destructor](boundtype.md#destructor-zilch-engine-d)| | |
|[GetGetterSetter](boundtype.md#getgettersetter-zilch-eng)|[Fields](boundtype.md#fields-zilch-engine-docum)| | |
|[GetMember](boundtype.md#getmember-zilch-engine-do)|[Functions](boundtype.md#functions-zilch-engine-do)| | |
|[GetProperty](boundtype.md#getproperty-zilch-engine)|[GetterSetters](boundtype.md#gettersetters-zilch-engin)| | |
|[InstantiatePreConstructedObject](boundtype.md#instantiatepreconstructe)|[IsNative](boundtype.md#isnative-zilch-engine-doc)| | |
| |[IsTypeOrBaseNative](boundtype.md#istypeorbasenative-zero)| | |
| |[Members](boundtype.md#members-zilch-engine-docu)| | |
| |[PreConstructor](boundtype.md#preconstructor-zilch-engi)| | |
| |[Properties](boundtype.md#properties-zilch-engine-d)| | |
| |[TemplateBaseName](boundtype.md#templatebasename-zilch-en)| | |


 #  Properties


---  
 #  BaseType : [boundtype](boundtype.md)

 `read-only`

> 
> ```TS:Nada
> var BaseType : BoundType


---  
 #  DefaultConstructor : [function](function.md)

 `read-only`

> 
> ```TS:Nada
> var DefaultConstructor : Function


---  
 #  Destructor : [function](function.md)

 `read-only`

> 
> ```TS:Nada
> var Destructor : Function


---  
 #  Fields : [fieldrange](fieldrange.md)

 `read-only`

> 
> ```TS:Nada
> var Fields : FieldRange


---  
 #  Functions : [functionrange](functionrange.md)

 `read-only`

> 
> ```TS:Nada
> var Functions : FunctionRange


---  
 #  GetterSetters : [gettersetterrange](gettersetterrange.md)

 `read-only`

> 
> ```TS:Nada
> var GetterSetters : GetterSetterRange


---  
 #  IsNative : [boolean](boolean.md)

 `read-only`

> 
> ```TS:Nada
> var IsNative : Boolean


---  
 #  IsTypeOrBaseNative : [boolean](boolean.md)

 `read-only`

> 
> ```TS:Nada
> var IsTypeOrBaseNative : Boolean


---  
 #  Members : [memberrange](memberrange.md)

 `read-only`

> 
> ```TS:Nada
> var Members : MemberRange


---  
 #  PreConstructor : [function](function.md)

 `read-only`

> 
> ```TS:Nada
> var PreConstructor : Function


---  
 #  Properties : [propertyrange](propertyrange.md)

 `read-only`

> 
> ```TS:Nada
> var Properties : PropertyRange


---  
 #  TemplateBaseName : [string](string.md)

 `read-only`

> 
> ```TS:Nada
> var TemplateBaseName : String


---  
 #  Methods


---  
 #  GetConstructor : [function](function.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |signatureType|[delegatetype](delegatetype.md)| |
> |inherited|[boolean](boolean.md)| |
> ```TS:Nada
> function GetConstructor(signatureType : DelegateType, inherited : Boolean) : Function
> ``` 


---  
 #  GetField : [field](field.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](string.md)| |
> ```TS:Nada
> function GetField(name : String) : Field
> ``` 


---  
 #  GetField : [field](field.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](string.md)| |
> |options|[Members](../flags_reference.md#members)| |
> ```TS:Nada
> function GetField(name : String, options : Members) : Field
> ``` 


---  
 #  GetField : [field](field.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](string.md)| |
> |declaredType|[type](type.md)| |
> |options|[Members](../flags_reference.md#members)| |
> ```TS:Nada
> function GetField(name : String, declaredType : Type, options : Members) : Field
> ``` 


---  
 #  GetFunction : [function](function.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](string.md)| |
> ```TS:Nada
> function GetFunction(name : String) : Function
> ``` 


---  
 #  GetFunction : [function](function.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](string.md)| |
> |signatureType|[delegatetype](delegatetype.md)| |
> |options|[Members](../flags_reference.md#members)| |
> ```TS:Nada
> function GetFunction(name : String, signatureType : DelegateType, options : Members) : Function
> ``` 


---  
 #  GetFunction : [function](function.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](string.md)| |
> |options|[Members](../flags_reference.md#members)| |
> ```TS:Nada
> function GetFunction(name : String, options : Members) : Function
> ``` 


---  
 #  GetGetterSetter : [gettersetter](gettersetter.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](string.md)| |
> ```TS:Nada
> function GetGetterSetter(name : String) : GetterSetter
> ``` 


---  
 #  GetGetterSetter : [gettersetter](gettersetter.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](string.md)| |
> |options|[Members](../flags_reference.md#members)| |
> ```TS:Nada
> function GetGetterSetter(name : String, options : Members) : GetterSetter
> ``` 


---  
 #  GetGetterSetter : [gettersetter](gettersetter.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](string.md)| |
> |declaredType|[type](type.md)| |
> |options|[Members](../flags_reference.md#members)| |
> ```TS:Nada
> function GetGetterSetter(name : String, declaredType : Type, options : Members) : GetterSetter
> ``` 


---  
 #  GetMember : [member](member.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](string.md)| |
> ```TS:Nada
> function GetMember(name : String) : Member
> ``` 


---  
 #  GetMember : [member](member.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](string.md)| |
> |options|[Members](../flags_reference.md#members)| |
> ```TS:Nada
> function GetMember(name : String, options : Members) : Member
> ``` 


---  
 #  GetMember : [member](member.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](string.md)| |
> |declaredType|[type](type.md)| |
> |options|[Members](../flags_reference.md#members)| |
> ```TS:Nada
> function GetMember(name : String, declaredType : Type, options : Members) : Member
> ``` 


---  
 #  GetProperty : Property

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](string.md)| |
> ```TS:Nada
> function GetProperty(name : String) : Property
> ``` 


---  
 #  GetProperty : Property

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](string.md)| |
> |options|[Members](../flags_reference.md#members)| |
> ```TS:Nada
> function GetProperty(name : String, options : Members) : Property
> ``` 


---  
 #  GetProperty : Property

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](string.md)| |
> |declaredType|[type](type.md)| |
> |options|[Members](../flags_reference.md#members)| |
> ```TS:Nada
> function GetProperty(name : String, declaredType : Type, options : Members) : Property
> ``` 


---  
 #  InstantiatePreConstructedObject : T

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function InstantiatePreConstructedObject() : T
> ``` 


---  
 

 
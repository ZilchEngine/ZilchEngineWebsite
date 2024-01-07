 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Add](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/array_t .md#add-void)|[ All](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/array_t .md#all-zilch-engine-document)| | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/array_t .md#array-t-void)|[ Capacity](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/array_t .md#capacity-zilch-engine-doc)| | |
|[ Clear](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/array_t .md#clear-void)|[ Count](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/array_t .md#count-zilch-engine-docume)| | |
|[ Copy](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/array_t .md#copy-zilch-engine-documen)|[ LastIndex](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/array_t .md#lastindex-zilch-engine-do)| | |
|[ FindFirstIndex](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/array_t .md#findfirstindex-zilch-engi)| | | |
|[ Get](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/array_t .md#get-zilch-engine-document)| | | |
|[ Insert](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/array_t .md#insert-void)| | | |
|[ Pop](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/array_t .md#pop-zilch-engine-document)| | | |
|[ Push](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/array_t .md#push-void)| | | |
|[ Range](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/array_t .md#range-zilch-engine-docume)| | | |
|[ RemoveAll](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/array_t .md#removeall-zilch-engine-do)| | | |
|[ RemoveAt](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/array_t .md#removeat-void)| | | |
|[ RemoveFirst](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/array_t .md#removefirst-zilch-engine)| | | |
|[ RemoveSwap](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/array_t .md#removeswap-void)| | | |
|[ Reserve](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/array_t .md#reserve-void)| | | |
|[ Resize](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/array_t .md#resize-void)| | | |
|[ Set](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/array_t .md#set-void)| | | |
|[ Sort](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/array_t .md#sort-void)| | | |


 #  Properties


---  
 #  All : ArrayRange[T]

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var All : ArrayRange[T]


---  
 #  Capacity : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Capacity : Integer


---  
 #  Count : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Count : Integer


---  
 #  LastIndex : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var LastIndex : Integer


---  
 #  Methods


---  
 #  Add : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|T| |
> ``` lang=cpp, name=Nada
> function Add(p0 : T)
> ``` 


---  
 #  Array[T] : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Array[T]()
> ``` 


---  
 #  Array[T] : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |size|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Array[T](size : Integer)
> ``` 


---  
 #  Array[T] : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |size|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |defaultValue|T| |
> ``` lang=cpp, name=Nada
> function Array[T](size : Integer, defaultValue : T)
> ``` 


---  
 #  Clear : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Clear()
> ``` 


---  
 #  Copy : Array[T]

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Copy() : Array[T]
> ``` 


---  
 #  FindFirstIndex : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |value|T| |
> ``` lang=cpp, name=Nada
> function FindFirstIndex(value : T) : Integer
> ``` 


---  
 #  Get : T

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Get(index : Integer) : T
> ``` 


---  
 #  Insert : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |value|T| |
> ``` lang=cpp, name=Nada
> function Insert(index : Integer, value : T)
> ``` 


---  
 #  Pop : T

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Pop() : T
> ``` 


---  
 #  Push : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|T| |
> ``` lang=cpp, name=Nada
> function Push(p0 : T)
> ``` 


---  
 #  Range : ArrayRange[T]

> 
> |Name|Type|Description|
> |---|---|---|
> |start|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |count|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Range(start : Integer, count : Integer) : ArrayRange[T]
> ``` 


---  
 #  RemoveAll : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |value|T| |
> ``` lang=cpp, name=Nada
> function RemoveAll(value : T) : Integer
> ``` 


---  
 #  RemoveAt : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function RemoveAt(index : Integer)
> ``` 


---  
 #  RemoveFirst : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |value|T| |
> ``` lang=cpp, name=Nada
> function RemoveFirst(value : T) : Boolean
> ``` 


---  
 #  RemoveSwap : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function RemoveSwap(index : Integer)
> ``` 


---  
 #  Reserve : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |capacity|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Reserve(capacity : Integer)
> ``` 


---  
 #  Resize : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |size|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Resize(size : Integer)
> ``` 


---  
 #  Resize : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |size|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |defaultValue|T| |
> ``` lang=cpp, name=Nada
> function Resize(size : Integer, defaultValue : T)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |value|T| |
> ``` lang=cpp, name=Nada
> function Set(index : Integer, value : T)
> ``` 


---  
 #  Sort : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |compare|delegate(left:any,right:any):[boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)| |
> ``` lang=cpp, name=Nada
> function Sort(compare : delegate(left:any,right:any):Boolean)
> ``` 


---  
 #  Sort : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |compare|delegate(left:any,right:any):[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Sort(compare : delegate(left:any,right:any):Integer)
> ``` 


---  
 

 
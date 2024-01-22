 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Add](array_t .md#add-void)|[All](array_t .md#all-zilch-engine-document)| | |
|[Constructor](array_t .md#array-t-void)|[Capacity](array_t .md#capacity-zilch-engine-doc)| | |
|[Clear](array_t .md#clear-void)|[Count](array_t .md#count-zilch-engine-docume)| | |
|[Copy](array_t .md#copy-zilch-engine-documen)|[LastIndex](array_t .md#lastindex-zilch-engine-do)| | |
|[FindFirstIndex](array_t .md#findfirstindex-zilch-engi)| | | |
|[Get](array_t .md#get-zilch-engine-document)| | | |
|[Insert](array_t .md#insert-void)| | | |
|[Pop](array_t .md#pop-zilch-engine-document)| | | |
|[Push](array_t .md#push-void)| | | |
|[Range](array_t .md#range-zilch-engine-docume)| | | |
|[RemoveAll](array_t .md#removeall-zilch-engine-do)| | | |
|[RemoveAt](array_t .md#removeat-void)| | | |
|[RemoveFirst](array_t .md#removefirst-zilch-engine)| | | |
|[RemoveSwap](array_t .md#removeswap-void)| | | |
|[Reserve](array_t .md#reserve-void)| | | |
|[Resize](array_t .md#resize-void)| | | |
|[Set](array_t .md#set-void)| | | |
|[Sort](array_t .md#sort-void)| | | |


 #  Properties


---  
 #  All : ArrayRange[T]

 `read-only`

> 
> ```TS:Nada
> var All : ArrayRange[T]


---  
 #  Capacity : [integer](integer.md)

 `read-only`

> 
> ```TS:Nada
> var Capacity : Integer


---  
 #  Count : [integer](integer.md)

 `read-only`

> 
> ```TS:Nada
> var Count : Integer


---  
 #  LastIndex : [integer](integer.md)

 `read-only`

> 
> ```TS:Nada
> var LastIndex : Integer


---  
 #  Methods


---  
 #  Add : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|T| |
> ```TS:Nada
> function Add(p0 : T)
> ``` 


---  
 #  Array[T] : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Array[T]()
> ``` 


---  
 #  Array[T] : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |size|[integer](integer.md)| |
> ```TS:Nada
> function Array[T](size : Integer)
> ``` 


---  
 #  Array[T] : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |size|[integer](integer.md)| |
> |defaultValue|T| |
> ```TS:Nada
> function Array[T](size : Integer, defaultValue : T)
> ``` 


---  
 #  Clear : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Clear()
> ``` 


---  
 #  Copy : Array[T]

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Copy() : Array[T]
> ``` 


---  
 #  FindFirstIndex : [integer](integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |value|T| |
> ```TS:Nada
> function FindFirstIndex(value : T) : Integer
> ``` 


---  
 #  Get : T

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](integer.md)| |
> ```TS:Nada
> function Get(index : Integer) : T
> ``` 


---  
 #  Insert : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](integer.md)| |
> |value|T| |
> ```TS:Nada
> function Insert(index : Integer, value : T)
> ``` 


---  
 #  Pop : T

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Pop() : T
> ``` 


---  
 #  Push : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|T| |
> ```TS:Nada
> function Push(p0 : T)
> ``` 


---  
 #  Range : ArrayRange[T]

> 
> |Name|Type|Description|
> |---|---|---|
> |start|[integer](integer.md)| |
> |count|[integer](integer.md)| |
> ```TS:Nada
> function Range(start : Integer, count : Integer) : ArrayRange[T]
> ``` 


---  
 #  RemoveAll : [integer](integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |value|T| |
> ```TS:Nada
> function RemoveAll(value : T) : Integer
> ``` 


---  
 #  RemoveAt : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](integer.md)| |
> ```TS:Nada
> function RemoveAt(index : Integer)
> ``` 


---  
 #  RemoveFirst : [boolean](boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |value|T| |
> ```TS:Nada
> function RemoveFirst(value : T) : Boolean
> ``` 


---  
 #  RemoveSwap : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](integer.md)| |
> ```TS:Nada
> function RemoveSwap(index : Integer)
> ``` 


---  
 #  Reserve : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |capacity|[integer](integer.md)| |
> ```TS:Nada
> function Reserve(capacity : Integer)
> ``` 


---  
 #  Resize : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |size|[integer](integer.md)| |
> ```TS:Nada
> function Resize(size : Integer)
> ``` 


---  
 #  Resize : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |size|[integer](integer.md)| |
> |defaultValue|T| |
> ```TS:Nada
> function Resize(size : Integer, defaultValue : T)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](integer.md)| |
> |value|T| |
> ```TS:Nada
> function Set(index : Integer, value : T)
> ``` 


---  
 #  Sort : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |compare|delegate(left:any,right:any):[boolean](boolean.md)| |
> ```TS:Nada
> function Sort(compare : delegate(left:any,right:any):Boolean)
> ``` 


---  
 #  Sort : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |compare|delegate(left:any,right:any):[integer](integer.md)| |
> ```TS:Nada
> function Sort(compare : delegate(left:any,right:any):Integer)
> ``` 


---  
 

 
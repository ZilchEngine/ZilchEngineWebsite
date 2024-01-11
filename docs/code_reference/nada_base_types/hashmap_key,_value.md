 `Core`

(NOTE) Hash Map is an Associative Hashed Container.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key, value /#add-void | Add]]|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key, value /#all-zilch-engine-document | All]]|HashedContainer<Pair<KeyType,DataType>,PairHashAdapter<Hasher,KeyType,DataType>,Allocator>| |
|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key, value /#clear-void | Clear]]|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key, value /#count-zilch-engine-docume | Count]]| | |
|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key, value /#contains-zilch-engine-doc | Contains]]|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key, value /#keys-zilch-engine-documen | Keys]]| | |
|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key, value /#get-zilch-engine-document | Get]]|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key, value /#values-zilch-engine-docum | Values]]| | |
|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key, value /#getordefault-zilch-engine | GetOrDefault]]| | | |
|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key, value /#getorerror-zilch-engine-d | GetOrError]]| | | |
|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key, value /#hashmap-key, value-void | Constructor]]| | | |
|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key, value /#removeorerror-void | RemoveOrError]]| | | |
|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key, value /#removeorignore-zilch-engi | RemoveOrIgnore]]| | | |
|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key, value /#set-zilch-engine-document | Set]]| | | |
|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key, value /#setorerror-void | SetOrError]]| | | |
|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key, value /#setorignore-zilch-engine | SetOrIgnore]]| | | |
|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key, value /#setoroverwrite-zilch-engi | SetOrOverwrite]]| | | |


 #  Properties


---  
 #  All : HashMapRange[Key,Value]

 `read-only`

> 
> ```TS:Nada
> var All : HashMapRange[Key, Value]


---  
 #  Count : [integer](integer.md)

 `read-only`

> 
> ```TS:Nada
> var Count : Integer


---  
 #  Keys : HashMapKeyRange[Key]

 `read-only`

> 
> ```TS:Nada
> var Keys : HashMapKeyRange[Key]


---  
 #  Values : HashMapValueRange[Value]

 `read-only`

> 
> ```TS:Nada
> var Values : HashMapValueRange[Value]


---  
 #  Methods


---  
 #  Add : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ||Value| |
> ```TS:Nada
> function Add( : Key,  : Value)
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
 #  Contains : [boolean](boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ```TS:Nada
> function Contains( : Key) : Boolean
> ``` 


---  
 #  Get : Value

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ```TS:Nada
> function Get( : Key) : Value
> ``` 


---  
 #  GetOrDefault : Value

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ```TS:Nada
> function GetOrDefault( : Key) : Value
> ``` 


---  
 #  GetOrDefault : Value

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ||Value| |
> ```TS:Nada
> function GetOrDefault( : Key,  : Value) : Value
> ``` 


---  
 #  GetOrError : Value

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ```TS:Nada
> function GetOrError( : Key) : Value
> ``` 


---  
 #  HashMap[Key, Value] : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function HashMap[Key, Value]()
> ``` 


---  
 #  RemoveOrError : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ```TS:Nada
> function RemoveOrError( : Key)
> ``` 


---  
 #  RemoveOrIgnore : [boolean](boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ```TS:Nada
> function RemoveOrIgnore( : Key) : Boolean
> ``` 


---  
 #  Set : [boolean](boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ||Value| |
> ```TS:Nada
> function Set( : Key,  : Value) : Boolean
> ``` 


---  
 #  SetOrError : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ||Value| |
> ```TS:Nada
> function SetOrError( : Key,  : Value)
> ``` 


---  
 #  SetOrIgnore : [boolean](boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ||Value| |
> ```TS:Nada
> function SetOrIgnore( : Key,  : Value) : Boolean
> ``` 


---  
 #  SetOrOverwrite : [boolean](boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ||Value| |
> ```TS:Nada
> function SetOrOverwrite( : Key,  : Value) : Boolean
> ``` 


---  
 

 
 `Core`(NOTE) Hash Map is an Associative Hashed Container.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key,value /#add-void | Add]]|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key,value /#all-zilch-engine-document | All]]|HashedContainer<Pair<KeyType,DataType>,PairHashAdapter<Hasher,KeyType,DataType>,Allocator>| |
|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key,value /#clear-void | Clear]]|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key,value /#count-zilch-engine-docume | Count]]| | |
|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key,value /#contains-zilch-engine-doc | Contains]]|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key,value /#keys-zilch-engine-documen | Keys]]| | |
|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key,value /#get-zilch-engine-document | Get]]|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key,value /#values-zilch-engine-docum | Values]]| | |
|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key,value /#getordefault-zilch-engine | GetOrDefault]]| | | |
|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key,value /#getorerror-zilch-engine-d | GetOrError]]| | | |
|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key,value /#hashmap-key,value-void | Constructor]]| | | |
|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key,value /#removeorerror-void | RemoveOrError]]| | | |
|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key,value /#removeorignore-zilch-engi | RemoveOrIgnore]]| | | |
|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key,value /#set-zilch-engine-document | Set]]| | | |
|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key,value /#setorerror-void | SetOrError]]| | | |
|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key,value /#setorignore-zilch-engine | SetOrIgnore]]| | | |
|[[zilch_engine_documentation/code_reference/nada_base_types/hashmap_key,value /#setoroverwrite-zilch-engi | SetOrOverwrite]]| | | |


 #  Properties


---  
 #  All : HashMapRange[Key,Value]

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var All : HashMapRange[Key,Value]


---  
 #  Count : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Count : Integer


---  
 #  Keys : HashMapKeyRange[Key]

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Keys : HashMapKeyRange[Key]


---  
 #  Values : HashMap[Value]

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Values : HashMap[Value]


---  
 #  Methods


---  
 #  Add : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ||Value| |
> ``` lang=cpp, name=Nada
> function Add( : Key,  : Value)
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
 #  Contains : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ``` lang=cpp, name=Nada
> function Contains( : Key) : Boolean
> ``` 


---  
 #  Get : Value

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ``` lang=cpp, name=Nada
> function Get( : Key) : Value
> ``` 


---  
 #  GetOrDefault : Value

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ``` lang=cpp, name=Nada
> function GetOrDefault( : Key) : Value
> ``` 


---  
 #  GetOrDefault : Value

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ||Value| |
> ``` lang=cpp, name=Nada
> function GetOrDefault( : Key,  : Value) : Value
> ``` 


---  
 #  GetOrError : Value

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ``` lang=cpp, name=Nada
> function GetOrError( : Key) : Value
> ``` 


---  
 #  HashMap[Key,Value] : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function HashMap[Key,Value]()
> ``` 


---  
 #  RemoveOrError : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ``` lang=cpp, name=Nada
> function RemoveOrError( : Key)
> ``` 


---  
 #  RemoveOrIgnore : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ``` lang=cpp, name=Nada
> function RemoveOrIgnore( : Key) : Boolean
> ``` 


---  
 #  Set : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ||Value| |
> ``` lang=cpp, name=Nada
> function Set( : Key,  : Value) : Boolean
> ``` 


---  
 #  SetOrError : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ||Value| |
> ``` lang=cpp, name=Nada
> function SetOrError( : Key,  : Value)
> ``` 


---  
 #  SetOrIgnore : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ||Value| |
> ``` lang=cpp, name=Nada
> function SetOrIgnore( : Key,  : Value) : Boolean
> ``` 


---  
 #  SetOrOverwrite : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ||Key| |
> ||Value| |
> ``` lang=cpp, name=Nada
> function SetOrOverwrite( : Key,  : Value) : Boolean
> ``` 


---  
 

 
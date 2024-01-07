 `Engine`

(NOTE) Object cache is use to store objects at runtime.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ClearStore](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objectstore.md#clearstore-void)|[ EntryCount](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objectstore.md#entrycount-zilch-engine-d)| | |
|[ Erase](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objectstore.md#erase-void)| | | |
|[ GetDirectoryPath](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objectstore.md#getdirectorypath-zilch-en)| | | |
|[ GetEntryAt](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objectstore.md#getentryat-zilch-engine-d)| | | |
|[ IsEntryStored](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objectstore.md#isentrystored-zilch-engin)| | | |
|[ IsStored](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objectstore.md#isstored-zilch-engine-doc)| | | |
|[ Restore](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objectstore.md#restore-zilch-engine-docu)| | | |
|[ RestoreOrArchetype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objectstore.md#restoreorarchetype-zero)| | | |
|[ Store](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objectstore.md#store-zilch-engine-docume)| | | |


 #  Properties


---  
 #  EntryCount : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Get number of entries in the ObjectStore.
> ``` lang=cpp, name=Nada
> var EntryCount : Integer


---  
 #  Methods


---  
 #  ClearStore : Void

> Clear the store.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ClearStore()
> ``` 


---  
 #  Erase : Void

> Attempts to remove an object from the store.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function Erase(name : String)
> ``` 


---  
 #  GetDirectoryPath : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> Returns the directory path to the object store.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function GetDirectoryPath() : String
> ``` 


---  
 #  GetEntryAt : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> Get the ObjectStore entry at the specified index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function GetEntryAt(index : Integer) : String
> ``` 


---  
 #  IsEntryStored : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Is there an entry record for the object in the store?
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function IsEntryStored(name : String) : Boolean
> ``` 


---  
 #  IsStored : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ||[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function IsStored( : String) : Boolean
> ``` 


---  
 #  Restore : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Restore an object to the space.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |space|[space](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md)| |
> ``` lang=cpp, name=Nada
> function Restore(name : String, space : Space) : Cog
> ``` 


---  
 #  RestoreOrArchetype : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Restore an object if it is not stored use the archetype to create it.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |archetype|[archetype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/archetype.md)| |
> |space|[space](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md)| |
> ``` lang=cpp, name=Nada
> function RestoreOrArchetype(name : String, archetype : Archetype, space : Space) : Cog
> ``` 


---  
 #  Store : [StoreResult](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#storeresult)

> Store an object.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |object|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Nada
> function Store(name : String, object : Cog) : StoreResult
> ``` 


---  
 

 
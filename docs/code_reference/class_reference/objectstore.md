 `Engine`

(NOTE) Object cache is use to store objects at runtime.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ClearStore](objectstore.md#clearstore-void)|[EntryCount](objectstore.md#entrycount-zilch-engine-d)| | |
|[Erase](objectstore.md#erase-void)| | | |
|[GetDirectoryPath](objectstore.md#getdirectorypath-zilch-en)| | | |
|[GetEntryAt](objectstore.md#getentryat-zilch-engine-d)| | | |
|[IsEntryStored](objectstore.md#isentrystored-zilch-engin)| | | |
|[IsStored](objectstore.md#isstored-zilch-engine-doc)| | | |
|[Restore](objectstore.md#restore-zilch-engine-docu)| | | |
|[RestoreOrArchetype](objectstore.md#restoreorarchetype-zero)| | | |
|[Store](objectstore.md#store-zilch-engine-docume)| | | |


 #  Properties


---  
 #  EntryCount : [integer](../nada_base_types/integer.md)

 `read-only`

> Get number of entries in the ObjectStore.
> ```TS:Nada
> var EntryCount : Integer


---  
 #  Methods


---  
 #  ClearStore : Void

> Clear the store.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ClearStore()
> ``` 


---  
 #  Erase : Void

> Attempts to remove an object from the store.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function Erase(name : String)
> ``` 


---  
 #  GetDirectoryPath : [string](../nada_base_types/string.md)

> Returns the directory path to the object store.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function GetDirectoryPath() : String
> ``` 


---  
 #  GetEntryAt : [string](../nada_base_types/string.md)

> Get the ObjectStore entry at the specified index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function GetEntryAt(index : Integer) : String
> ``` 


---  
 #  IsEntryStored : [boolean](../nada_base_types/boolean.md)

> Is there an entry record for the object in the store?
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function IsEntryStored(name : String) : Boolean
> ``` 


---  
 #  IsStored : [boolean](../nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ||[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function IsStored( : String) : Boolean
> ``` 


---  
 #  Restore : [cog](cog.md)

> Restore an object to the space.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> |space|[space](space.md)| |
> ```TS:Nada
> function Restore(name : String, space : Space) : Cog
> ``` 


---  
 #  RestoreOrArchetype : [cog](cog.md)

> Restore an object if it is not stored use the archetype to create it.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> |archetype|[archetype](archetype.md)| |
> |space|[space](space.md)| |
> ```TS:Nada
> function RestoreOrArchetype(name : String, archetype : Archetype, space : Space) : Cog
> ``` 


---  
 #  Store : [StoreResult](../enum_reference.md#storeresult)

> Store an object.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> |object|[cog](cog.md)| |
> ```TS:Nada
> function Store(name : String, object : Cog) : StoreResult
> ``` 


---  
 

 
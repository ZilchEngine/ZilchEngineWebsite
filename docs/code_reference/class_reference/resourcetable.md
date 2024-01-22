 `Resource` `Engine`



(NOTE) A table of resources (or strings) that can be indexed, searched by name, or sampled randomly. The table can be randomly sampled to return an entry into the table.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[AddOrError](resourcetable.md#addorerror-void)|[All](resourcetable.md#all-zilch-engine-document)|[dataresource](dataresource.md)| |
|[AddOrIgnore](resourcetable.md#addorignore-zilch-engine)|[Count](resourcetable.md#count-zilch-engine-docume)| | |
|[AddOrOverwrite](resourcetable.md#addoroverwrite-zilch-engi)|[MaxWeight](resourcetable.md#maxweight-zilch-engine-do)| | |
|[Clear](resourcetable.md#clear-void)|[ResourceType](resourcetable.md#resourcetype-zilch-engine)| | |
|[Contains](resourcetable.md#contains-zilch-engine-doc)| | | |
|[CreateRuntime](resourcetable.md#createruntime-zilch-engin)| | | |
|[ForceRebuild](resourcetable.md#forcerebuild-void)| | | |
|[Get](resourcetable.md#get-zilch-engine-document)| | | |
|[GetOrDefault](resourcetable.md#getordefault-zilch-engine)| | | |
|[GetOrError](resourcetable.md#getorerror-zilch-engine-d)| | | |
|[GetOrNull](resourcetable.md#getornull-zilch-engine-do)| | | |
|[RemoveAt](resourcetable.md#removeat-void)| | | |
|[RemoveOrError](resourcetable.md#removeorerror-void)| | | |
|[RemoveOrIgnore](resourcetable.md#removeorignore-zilch-engi)| | | |
|[RuntimeClone](resourcetable.md#runtimeclone-zilch-engine)| | | |
|[Sample](resourcetable.md#sample-zilch-engine-docum)| | | |
|[SampleIndex](resourcetable.md#sampleindex-zilch-engine)| | | |
|[Set](resourcetable.md#set-void)| | | |


 #  Properties


---  
 #  All : [resourcetableentryrange](resourcetableentryrange.md)

 `read-only`

> Range to iterate over all entries.
> ```TS:Nada
> var All : ResourceTableEntryRange


---  
 #  Count : [integer](../nada_base_types/integer.md)

 `read-only`

> How many items are stored in the table.
> ```TS:Nada
> var Count : Integer


---  
 #  MaxWeight : [real](../nada_base_types/real.md)

> The maximum probability weight value that can be stored in the table. Setting this will clamp all weight values.
> ```TS:Nada
> var MaxWeight : Real


---  
 #  ResourceType : [string](../nada_base_types/string.md)

> The kind of resource contained in this table. This is either a resource type or "String".
> ```TS:Nada
> var ResourceType : String


---  
 #  Methods


---  
 #  AddOrError : Void

> Add the given entry. If another entry with the same name exists then an error is thrown.
> |Name|Type|Description|
> |---|---|---|
> |entry|[resourcetableentry](resourcetableentry.md)| |
> ```TS:Nada
> function AddOrError(entry : ResourceTableEntry)
> ``` 


---  
 #  AddOrIgnore : [boolean](../nada_base_types/boolean.md)

> Add the given entry. If another entry with the same name exists then no operation is performed.
> |Name|Type|Description|
> |---|---|---|
> |entry|[resourcetableentry](resourcetableentry.md)| |
> ```TS:Nada
> function AddOrIgnore(entry : ResourceTableEntry) : Boolean
> ``` 


---  
 #  AddOrOverwrite : [boolean](../nada_base_types/boolean.md)

> Add the given entry. If another entry with the same name exists then it is overwritten.
> |Name|Type|Description|
> |---|---|---|
> |entry|[resourcetableentry](resourcetableentry.md)| |
> ```TS:Nada
> function AddOrOverwrite(entry : ResourceTableEntry) : Boolean
> ``` 


---  
 #  Clear : Void

> Clear all items in the table.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Clear()
> ``` 


---  
 #  Contains : [boolean](../nada_base_types/boolean.md)

> Returns if the given key is contained.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function Contains(key : String) : Boolean
> ``` 


---  
 #  CreateRuntime : [resourcetable](resourcetable.md)

 `static`

> Creates a ResourceTable for run-time modifications.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function CreateRuntime() : ResourceTable
> ``` 


---  
 #  ForceRebuild : Void

> Force rebuild the weighted probability table.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ForceRebuild()
> ``` 


---  
 #  Get : [resourcetableentry](resourcetableentry.md)

> Access an item at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function Get(index : Integer) : ResourceTableEntry
> ``` 


---  
 #  Get : [resourcetableentry](resourcetableentry.md)

> Hash-Set interface. Gets the item with the same name as the entry.
> |Name|Type|Description|
> |---|---|---|
> |entry|[resourcetableentry](resourcetableentry.md)| |
> ```TS:Nada
> function Get(entry : ResourceTableEntry) : ResourceTableEntry
> ``` 


---  
 #  Get : [resourcetableentry](resourcetableentry.md)

> Hash-Map interface. Gets via the provided key.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function Get(key : String) : ResourceTableEntry
> ``` 


---  
 #  GetOrDefault : [resourcetableentry](resourcetableentry.md)

> Returns the entry associated with the given key. If no entry matches the key then the provided default is returned.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](../nada_base_types/string.md)| |
> |defaultValue|[resourcetableentry](resourcetableentry.md)| |
> ```TS:Nada
> function GetOrDefault(key : String, defaultValue : ResourceTableEntry) : ResourceTableEntry
> ``` 


---  
 #  GetOrError : [resourcetableentry](resourcetableentry.md)

> Returns the entry associated with the given key. If no entry matches the key then an exception is thrown.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function GetOrError(key : String) : ResourceTableEntry
> ``` 


---  
 #  GetOrNull : [resourcetableentry](resourcetableentry.md)

> Returns the entry associated with the given key. If no entry matches then null is returned.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function GetOrNull(key : String) : ResourceTableEntry
> ``` 


---  
 #  RemoveAt : Void

> Removes the item at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function RemoveAt(index : Integer)
> ``` 


---  
 #  RemoveOrError : Void

> Removes the entry associated with the given key. If no entry matches an exception is thrown.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function RemoveOrError(key : String)
> ``` 


---  
 #  RemoveOrIgnore : [boolean](../nada_base_types/boolean.md)

> Removes the entry associated with the given key. If no entry matches then no operation is performed.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function RemoveOrIgnore(key : String) : Boolean
> ``` 


---  
 #  RuntimeClone : [resourcetable](resourcetable.md)

> Creates a clone of this table for run-time modifications.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function RuntimeClone() : ResourceTable
> ``` 


---  
 #  Sample : [resourcetableentry](resourcetableentry.md)

> Samples the table to return a random entry. Takes two (different) random floats from [0,1) in order to sample. Returns an empty string if the table is empty.
> |Name|Type|Description|
> |---|---|---|
> |random1|[real](../nada_base_types/real.md)| |
> |random2|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function Sample(random1 : Real, random2 : Real) : ResourceTableEntry
> ``` 


---  
 #  SampleIndex : [integer](../nada_base_types/integer.md)

> Samples the table to return a random index into the table. Takes two (different) random floats from [0,1) in order to sample.
> |Name|Type|Description|
> |---|---|---|
> |random1|[real](../nada_base_types/real.md)| |
> |random2|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function SampleIndex(random1 : Real, random2 : Real) : Integer
> ``` 


---  
 #  Set : Void

> Access an item at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> |entry|[resourcetableentry](resourcetableentry.md)| |
> ```TS:Nada
> function Set(index : Integer, entry : ResourceTableEntry)
> ``` 


---  
 #  Set : Void

> Hash-Set interface. Sets the item with the same name as the entry.
> |Name|Type|Description|
> |---|---|---|
> |entry|[resourcetableentry](resourcetableentry.md)| |
> ```TS:Nada
> function Set(entry : ResourceTableEntry)
> ``` 


---  
 #  Set : Void

> Hash-Map interface. Sets via the provided key.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](../nada_base_types/string.md)| |
> |entry|[resourcetableentry](resourcetableentry.md)| |
> ```TS:Nada
> function Set(key : String, entry : ResourceTableEntry)
> ``` 


---  
 

 
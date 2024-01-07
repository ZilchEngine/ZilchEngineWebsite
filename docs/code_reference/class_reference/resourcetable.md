 `Resource` `Engine`



(NOTE) A table of resources (or strings) that can be indexed, searched by name, or sampled randomly. The table can be randomly sampled to return an entry into the table.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddOrError](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetable.md#addorerror-void)|[ All](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetable.md#all-zilch-engine-document)|[dataresource](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/dataresource.md)| |
|[ AddOrIgnore](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetable.md#addorignore-zilch-engine)|[ Count](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetable.md#count-zilch-engine-docume)| | |
|[ AddOrOverwrite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetable.md#addoroverwrite-zilch-engi)|[ MaxWeight](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetable.md#maxweight-zilch-engine-do)| | |
|[ Clear](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetable.md#clear-void)|[ ResourceType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetable.md#resourcetype-zilch-engine)| | |
|[ Contains](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetable.md#contains-zilch-engine-doc)| | | |
|[ CreateRuntime](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetable.md#createruntime-zilch-engin)| | | |
|[ ForceRebuild](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetable.md#forcerebuild-void)| | | |
|[ Get](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetable.md#get-zilch-engine-document)| | | |
|[ GetOrDefault](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetable.md#getordefault-zilch-engine)| | | |
|[ GetOrError](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetable.md#getorerror-zilch-engine-d)| | | |
|[ GetOrNull](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetable.md#getornull-zilch-engine-do)| | | |
|[ RemoveAt](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetable.md#removeat-void)| | | |
|[ RemoveOrError](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetable.md#removeorerror-void)| | | |
|[ RemoveOrIgnore](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetable.md#removeorignore-zilch-engi)| | | |
|[ RuntimeClone](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetable.md#runtimeclone-zilch-engine)| | | |
|[ Sample](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetable.md#sample-zilch-engine-docum)| | | |
|[ SampleIndex](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetable.md#sampleindex-zilch-engine)| | | |
|[ Set](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetable.md#set-void)| | | |


 #  Properties


---  
 #  All : [resourcetableentryrange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetableentryrange.md)

 `read-only`

> Range to iterate over all entries.
> ``` lang=cpp, name=Nada
> var All : ResourceTableEntryRange


---  
 #  Count : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> How many items are stored in the table.
> ``` lang=cpp, name=Nada
> var Count : Integer


---  
 #  MaxWeight : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The maximum probability weight value that can be stored in the table. Setting this will clamp all weight values.
> ``` lang=cpp, name=Nada
> var MaxWeight : Real


---  
 #  ResourceType : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> The kind of resource contained in this table. This is either a resource type or "String".
> ``` lang=cpp, name=Nada
> var ResourceType : String


---  
 #  Methods


---  
 #  AddOrError : Void

> Add the given entry. If another entry with the same name exists then an error is thrown.
> |Name|Type|Description|
> |---|---|---|
> |entry|[resourcetableentry](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetableentry.md)| |
> ``` lang=cpp, name=Nada
> function AddOrError(entry : ResourceTableEntry)
> ``` 


---  
 #  AddOrIgnore : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Add the given entry. If another entry with the same name exists then no operation is performed.
> |Name|Type|Description|
> |---|---|---|
> |entry|[resourcetableentry](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetableentry.md)| |
> ``` lang=cpp, name=Nada
> function AddOrIgnore(entry : ResourceTableEntry) : Boolean
> ``` 


---  
 #  AddOrOverwrite : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Add the given entry. If another entry with the same name exists then it is overwritten.
> |Name|Type|Description|
> |---|---|---|
> |entry|[resourcetableentry](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetableentry.md)| |
> ``` lang=cpp, name=Nada
> function AddOrOverwrite(entry : ResourceTableEntry) : Boolean
> ``` 


---  
 #  Clear : Void

> Clear all items in the table.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Clear()
> ``` 


---  
 #  Contains : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Returns if the given key is contained.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function Contains(key : String) : Boolean
> ``` 


---  
 #  CreateRuntime : [resourcetable](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetable.md)

 `static`

> Creates a ResourceTable for run-time modifications.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function CreateRuntime() : ResourceTable
> ``` 


---  
 #  ForceRebuild : Void

> Force rebuild the weighted probability table.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ForceRebuild()
> ``` 


---  
 #  Get : [resourcetableentry](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetableentry.md)

> Access an item at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Get(index : Integer) : ResourceTableEntry
> ``` 


---  
 #  Get : [resourcetableentry](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetableentry.md)

> Hash-Set interface. Gets the item with the same name as the entry.
> |Name|Type|Description|
> |---|---|---|
> |entry|[resourcetableentry](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetableentry.md)| |
> ``` lang=cpp, name=Nada
> function Get(entry : ResourceTableEntry) : ResourceTableEntry
> ``` 


---  
 #  Get : [resourcetableentry](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetableentry.md)

> Hash-Map interface. Gets via the provided key.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function Get(key : String) : ResourceTableEntry
> ``` 


---  
 #  GetOrDefault : [resourcetableentry](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetableentry.md)

> Returns the entry associated with the given key. If no entry matches the key then the provided default is returned.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |defaultValue|[resourcetableentry](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetableentry.md)| |
> ``` lang=cpp, name=Nada
> function GetOrDefault(key : String, defaultValue : ResourceTableEntry) : ResourceTableEntry
> ``` 


---  
 #  GetOrError : [resourcetableentry](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetableentry.md)

> Returns the entry associated with the given key. If no entry matches the key then an exception is thrown.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function GetOrError(key : String) : ResourceTableEntry
> ``` 


---  
 #  GetOrNull : [resourcetableentry](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetableentry.md)

> Returns the entry associated with the given key. If no entry matches then null is returned.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function GetOrNull(key : String) : ResourceTableEntry
> ``` 


---  
 #  RemoveAt : Void

> Removes the item at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function RemoveAt(index : Integer)
> ``` 


---  
 #  RemoveOrError : Void

> Removes the entry associated with the given key. If no entry matches an exception is thrown.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function RemoveOrError(key : String)
> ``` 


---  
 #  RemoveOrIgnore : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Removes the entry associated with the given key. If no entry matches then no operation is performed.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function RemoveOrIgnore(key : String) : Boolean
> ``` 


---  
 #  RuntimeClone : [resourcetable](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetable.md)

> Creates a clone of this table for run-time modifications.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function RuntimeClone() : ResourceTable
> ``` 


---  
 #  Sample : [resourcetableentry](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetableentry.md)

> Samples the table to return a random entry. Takes two (different) random floats from [0,1) in order to sample. Returns an empty string if the table is empty.
> |Name|Type|Description|
> |---|---|---|
> |random1|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |random2|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function Sample(random1 : Real, random2 : Real) : ResourceTableEntry
> ``` 


---  
 #  SampleIndex : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> Samples the table to return a random index into the table. Takes two (different) random floats from [0,1) in order to sample.
> |Name|Type|Description|
> |---|---|---|
> |random1|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |random2|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function SampleIndex(random1 : Real, random2 : Real) : Integer
> ``` 


---  
 #  Set : Void

> Access an item at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |entry|[resourcetableentry](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetableentry.md)| |
> ``` lang=cpp, name=Nada
> function Set(index : Integer, entry : ResourceTableEntry)
> ``` 


---  
 #  Set : Void

> Hash-Set interface. Sets the item with the same name as the entry.
> |Name|Type|Description|
> |---|---|---|
> |entry|[resourcetableentry](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetableentry.md)| |
> ``` lang=cpp, name=Nada
> function Set(entry : ResourceTableEntry)
> ``` 


---  
 #  Set : Void

> Hash-Map interface. Sets via the provided key.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |entry|[resourcetableentry](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetableentry.md)| |
> ``` lang=cpp, name=Nada
> function Set(key : String, entry : ResourceTableEntry)
> ``` 


---  
 

 
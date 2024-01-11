 `Engine`

(NOTE) An entry from a resource table. The resource type of this entry must match the resource type of the table to add/set. If the value is set via string then the type will be implicitly set to string, otherwise the type must be set via the Resource property.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Clone](resourcetableentry.md#clone-zilch-engine-docume)|[ Name](resourcetableentry.md#name-zilch-engine-documen)| | |
|[ Constructor](resourcetableentry.md#resourcetableentry-void)|[ Resource](resourcetableentry.md#resource-resource)| | |
| |[ ResourceType](resourcetableentry.md#resourcetype-zilch-engine)| | |
| |[ Value](resourcetableentry.md#value-zilch-engine-docume)| | |
| |[ Weight](resourcetableentry.md#weight-zilch-engine-docum)| | |


 #  Properties


---  
 #  Name : [string](../nada_base_types/string.md)

> 
> ``` lang=cpp, name=Nada
> var Name : String


---  
 #  Resource : Resource

> The resource value of this entry. Returns null if the underlying type is not a resource. Changes this entry's type to the given resource's type on Set.
> ``` lang=cpp, name=Nada
> var Resource : Resource


---  
 #  ResourceType : [string](../nada_base_types/string.md)

> 
> ``` lang=cpp, name=Nada
> var ResourceType : String


---  
 #  Value : [string](../nada_base_types/string.md)

> The string value of this entry. Changes this entry's type to String on Set.
> ``` lang=cpp, name=Nada
> var Value : String


---  
 #  Weight : [real](../nada_base_types/real.md)

> The weight value used to determine how likely this item is to be sampled. Note: Weights must be positive. Negative weights will be clamped to 0.
> ``` lang=cpp, name=Nada
> var Weight : Real


---  
 #  Methods


---  
 #  Clone : [resourcetableentry](resourcetableentry.md)

> Creates a new entry with the same values.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Clone() : ResourceTableEntry
> ``` 


---  
 #  ResourceTableEntry : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ResourceTableEntry()
> ``` 


---  
 #  ResourceTableEntry : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ||[resourcetableentry](resourcetableentry.md)| |
> ``` lang=cpp, name=Nada
> function ResourceTableEntry( : ResourceTableEntry)
> ``` 


---  
 

 
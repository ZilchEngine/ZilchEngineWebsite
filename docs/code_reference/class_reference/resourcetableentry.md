 `Engine`

(NOTE) An entry from a resource table. The resource type of this entry must match the resource type of the table to add/set. If the value is set via string then the type will be implicitly set to string, otherwise the type must be set via the Resource property.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Clone](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetableentry.md#clone-zilch-engine-docume)|[ Name](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetableentry.md#name-zilch-engine-documen)| | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetableentry.md#resourcetableentry-void)|[ Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetableentry.md#resource-resource)| | |
| |[ ResourceType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetableentry.md#resourcetype-zilch-engine)| | |
| |[ Value](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetableentry.md#value-zilch-engine-docume)| | |
| |[ Weight](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetableentry.md#weight-zilch-engine-docum)| | |


 #  Properties


---  
 #  Name : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> 
> ``` lang=cpp, name=Nada
> var Name : String


---  
 #  Resource : Resource

> The resource value of this entry. Returns null if the underlying type is not a resource. Changes this entry's type to the given resource's type on Set.
> ``` lang=cpp, name=Nada
> var Resource : Resource


---  
 #  ResourceType : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> 
> ``` lang=cpp, name=Nada
> var ResourceType : String


---  
 #  Value : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> The string value of this entry. Changes this entry's type to String on Set.
> ``` lang=cpp, name=Nada
> var Value : String


---  
 #  Weight : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The weight value used to determine how likely this item is to be sampled. Note: Weights must be positive. Negative weights will be clamped to 0.
> ``` lang=cpp, name=Nada
> var Weight : Real


---  
 #  Methods


---  
 #  Clone : [resourcetableentry](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetableentry.md)

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
> ||[resourcetableentry](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcetableentry.md)| |
> ``` lang=cpp, name=Nada
> function ResourceTableEntry( : ResourceTableEntry)
> ``` 


---  
 

 
 `Resource` `Engine`



(NOTE) An archetype is a resource containing the serialized data definition of an object. The archetype stores a binary cache of the serialization data and the source file for debugging and for archetype updating.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ StoredType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/archetype.md#storedtype-zilch-engine-d)|Resource| |


 #  Properties


---  
 #  StoredType : [boundtype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boundtype.md)

> An Archetype can be a Cog, Space, or GameSession. It's okay for this to be a raw BoundType* because native types will never be destructed.
> ``` lang=cpp, name=Nada
> var StoredType : BoundType


---  
 #  Methods


---  
 

 
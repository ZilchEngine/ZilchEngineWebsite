 `Resource` `Graphics`



(NOTE) A composition of shader fragments that defines a shader program that is used when rendering Graphicals.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ RuntimeClone](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/material.md#runtimeclone-zilch-engine)|[ CompositionLabel](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/material.md#compositionlabel-zilch-en)|[dataresource](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/dataresource.md)| |
| |[ ReferencedByList](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/material.md#referencedbylist-zilch-en)| | |
| |[ RenderGroups](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/material.md#rendergroups-zilch-engine)| | |


 #  Properties


---  
 #  CompositionLabel : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var CompositionLabel : Integer


---  
 #  ReferencedByList : [rendergrouplist](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rendergrouplist.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var ReferencedByList : RenderGroupList


---  
 #  RenderGroups : [rendergrouplist](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rendergrouplist.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var RenderGroups : RenderGroupList


---  
 #  Methods


---  
 #  RuntimeClone : [material](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/material.md)

> Creates an anonymous copy that can be independently modified, destroyed when all references are gone.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function RuntimeClone() : Material
> ``` 


---  
 

 
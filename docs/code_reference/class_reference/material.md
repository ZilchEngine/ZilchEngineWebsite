 `Resource` `Graphics`



(NOTE) A composition of shader fragments that defines a shader program that is used when rendering Graphicals.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ RuntimeClone](material.md#runtimeclone-zilch-engine)|[ CompositionLabel](material.md#compositionlabel-zilch-en)|[dataresource](dataresource.md)| |
| |[ ReferencedByList](material.md#referencedbylist-zilch-en)| | |
| |[ RenderGroups](material.md#rendergroups-zilch-engine)| | |


 #  Properties


---  
 #  CompositionLabel : [integer](../nada_base_types/integer.md)

 `read-only`

> 
> ```TS:Nada
> var CompositionLabel : Integer


---  
 #  ReferencedByList : [rendergrouplist](rendergrouplist.md)

 `read-only`

> 
> ```TS:Nada
> var ReferencedByList : RenderGroupList


---  
 #  RenderGroups : [rendergrouplist](rendergrouplist.md)

 `read-only`

> 
> ```TS:Nada
> var RenderGroups : RenderGroupList


---  
 #  Methods


---  
 #  RuntimeClone : [material](material.md)

> Creates an anonymous copy that can be independently modified, destroyed when all references are gone.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function RuntimeClone() : Material
> ``` 


---  
 

 
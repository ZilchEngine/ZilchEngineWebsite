 `Resource` `Graphics`



(NOTE) How Materials are categorized, determines which graphicals are drawn in a render pass.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ IsSubRenderGroup](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rendergroup.md#issubrendergroup-zilch-en)|[ ChildRenderGroups](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rendergroup.md#childrendergroups-zilch-e)|[dataresource](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/dataresource.md)| |
|[ IsSubRenderGroupOf](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rendergroup.md#issubrendergroupof-zero)|[ GraphicalSortMethod](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rendergroup.md#graphicalsortmethod-zero)| | |
| |[ Materials](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rendergroup.md#materials-zilch-engine-do)| | |
| |[ ParentRenderGroup](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rendergroup.md#parentrendergroup-zilch-e)| | |
| |[ ReferencedByList](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rendergroup.md#referencedbylist-zilch-en)| | |


 #  Properties


---  
 #  ChildRenderGroups : [childrendergrouplist](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/childrendergrouplist.md)

 `read-only`

> For assigning child RenderGroups, making this a parent group of everything in the list.
> ``` lang=cpp, name=Nada
> var ChildRenderGroups : ChildRenderGroupList


---  
 #  GraphicalSortMethod : [GraphicalSortMethod](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#graphicalsortmethod)

> Determines the order that graphicals will be drawn when processed as this RenderGroup.
> ``` lang=cpp, name=Nada
> var GraphicalSortMethod : GraphicalSortMethod


---  
 #  Materials : [materiallist](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/materiallist.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Materials : MaterialList


---  
 #  ParentRenderGroup : [rendergroup](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rendergroup.md)

> RenderGroup that this is a sub group of. Also a sub group of all of its parents.
> ``` lang=cpp, name=Nada
> var ParentRenderGroup : RenderGroup


---  
 #  ReferencedByList : [materiallist](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/materiallist.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var ReferencedByList : MaterialList


---  
 #  Methods


---  
 #  IsSubRenderGroup : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Returns whether or not the given RenderGroup is a sub group of this.
> |Name|Type|Description|
> |---|---|---|
> |renderGroup|[rendergroup](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rendergroup.md)| |
> ``` lang=cpp, name=Nada
> function IsSubRenderGroup(renderGroup : RenderGroup) : Boolean
> ``` 


---  
 #  IsSubRenderGroupOf : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Returns whether or not this is a sub group of the given RenderGroup.
> |Name|Type|Description|
> |---|---|---|
> |renderGroup|[rendergroup](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rendergroup.md)| |
> ``` lang=cpp, name=Nada
> function IsSubRenderGroupOf(renderGroup : RenderGroup) : Boolean
> ``` 


---  
 

 
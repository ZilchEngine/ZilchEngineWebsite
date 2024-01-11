 `Resource` `Graphics`



(NOTE) How Materials are categorized, determines which graphicals are drawn in a render pass.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ IsSubRenderGroup](rendergroup.md#issubrendergroup-zilch-en)|[ ChildRenderGroups](rendergroup.md#childrendergroups-zilch-e)|[dataresource](dataresource.md)| |
|[ IsSubRenderGroupOf](rendergroup.md#issubrendergroupof-zero)|[ GraphicalSortMethod](rendergroup.md#graphicalsortmethod-zero)| | |
| |[ Materials](rendergroup.md#materials-zilch-engine-do)| | |
| |[ ParentRenderGroup](rendergroup.md#parentrendergroup-zilch-e)| | |
| |[ ReferencedByList](rendergroup.md#referencedbylist-zilch-en)| | |


 #  Properties


---  
 #  ChildRenderGroups : [childrendergrouplist](childrendergrouplist.md)

 `read-only`

> For assigning child RenderGroups, making this a parent group of everything in the list.
> ```TS:Nada
> var ChildRenderGroups : ChildRenderGroupList


---  
 #  GraphicalSortMethod : [GraphicalSortMethod](../enum_reference.md#graphicalsortmethod)

> Determines the order that graphicals will be drawn when processed as this RenderGroup.
> ```TS:Nada
> var GraphicalSortMethod : GraphicalSortMethod


---  
 #  Materials : [materiallist](materiallist.md)

 `read-only`

> 
> ```TS:Nada
> var Materials : MaterialList


---  
 #  ParentRenderGroup : [rendergroup](rendergroup.md)

> RenderGroup that this is a sub group of. Also a sub group of all of its parents.
> ```TS:Nada
> var ParentRenderGroup : RenderGroup


---  
 #  ReferencedByList : [materiallist](materiallist.md)

 `read-only`

> 
> ```TS:Nada
> var ReferencedByList : MaterialList


---  
 #  Methods


---  
 #  IsSubRenderGroup : [boolean](../nada_base_types/boolean.md)

> Returns whether or not the given RenderGroup is a sub group of this.
> |Name|Type|Description|
> |---|---|---|
> |renderGroup|[rendergroup](rendergroup.md)| |
> ```TS:Nada
> function IsSubRenderGroup(renderGroup : RenderGroup) : Boolean
> ``` 


---  
 #  IsSubRenderGroupOf : [boolean](../nada_base_types/boolean.md)

> Returns whether or not this is a sub group of the given RenderGroup.
> |Name|Type|Description|
> |---|---|---|
> |renderGroup|[rendergroup](rendergroup.md)| |
> ```TS:Nada
> function IsSubRenderGroupOf(renderGroup : RenderGroup) : Boolean
> ``` 


---  
 

 
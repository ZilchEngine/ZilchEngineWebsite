 `Component` `UiWidget`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetChildren](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidgetcomponenthierarchy.md#getchildren-zilch-engine)|[ ChildCount](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidgetcomponenthierarchy.md#childcount-zilch-engine-d)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)|[uiwidget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidget.md)|
|[ IsAncestorOf](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidgetcomponenthierarchy.md#isancestorof-zilch-engine)|[ LastDeepestChild](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidgetcomponenthierarchy.md#lastdeepestchild-zilch-en)| | |
|[ IsDescendantOf](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidgetcomponenthierarchy.md#isdescendantof-zilch-engi)|[ LastDirectChild](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidgetcomponenthierarchy.md#lastdirectchild-zilch-eng)| | |
| |[ NextInHierarchyOrder](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidgetcomponenthierarchy.md#nextinhierarchyorder-zer)| | |
| |[ NextSibling](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidgetcomponenthierarchy.md#nextsibling-zilch-engine)| | |
| |[ Parent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidgetcomponenthierarchy.md#parent-zilch-engine-docum)| | |
| |[ PreviousInHierarchyOrder](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidgetcomponenthierarchy.md#previousinhierarchyorder)| | |
| |[ PreviousSibling](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidgetcomponenthierarchy.md#previoussibling-zilch-eng)| | |
| |[ Root](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidgetcomponenthierarchy.md#root-zilch-engine-documen)| | |


 #  Properties


---  
 #  ChildCount : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var ChildCount : Integer


---  
 #  LastDeepestChild : [uiwidget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidget.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var LastDeepestChild : UiWidget


---  
 #  LastDirectChild : [uiwidget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidget.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var LastDirectChild : UiWidget


---  
 #  NextInHierarchyOrder : [uiwidget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidget.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var NextInHierarchyOrder : UiWidget


---  
 #  NextSibling : [uiwidget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidget.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var NextSibling : UiWidget


---  
 #  Parent : [uiwidget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidget.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Parent : UiWidget


---  
 #  PreviousInHierarchyOrder : [uiwidget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidget.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var PreviousInHierarchyOrder : UiWidget


---  
 #  PreviousSibling : [uiwidget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidget.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var PreviousSibling : UiWidget


---  
 #  Root : [uiwidget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidget.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Root : UiWidget


---  
 #  Methods


---  
 #  GetChildren : [uiwidgetrange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidgetrange.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function GetChildren() : UiWidgetRange
> ``` 


---  
 #  IsAncestorOf : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ||[uiwidget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidget.md)| |
> ``` lang=cpp, name=Nada
> function IsAncestorOf( : UiWidget) : Boolean
> ``` 


---  
 #  IsDescendantOf : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ||[uiwidget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidget.md)| |
> ``` lang=cpp, name=Nada
> function IsDescendantOf( : UiWidget) : Boolean
> ``` 


---  
 

 
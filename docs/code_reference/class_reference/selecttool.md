 `Component` `Editor`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ RayCast](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/selecttool.md#raycast-zilch-engine-docu)|[ ArchetypeSelect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/selecttool.md#archetypeselect-zilch-eng)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)| |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/selecttool.md#selecttool-void)|[ Raycaster](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/selecttool.md#raycaster-zilch-engine-do)| | |
|[ SmartSelect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/selecttool.md#smartselect-zilch-engine)|[ RootSelect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/selecttool.md#rootselect-zilch-engine-d)| | |
| |[ SmartGroupSelect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/selecttool.md#smartgroupselect-zilch-en)| | |


 #  Properties


---  
 #  ArchetypeSelect : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Selects the root archetype of the tree, subsequent clicks will select the nearest archetype followed by any direct children following that.
> ``` lang=cpp, name=Nada
> var ArchetypeSelect : Boolean


---  
 #  Raycaster : [raycaster](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/raycaster.md)

> 
> ``` lang=cpp, name=Nada
> var Raycaster : Raycaster


---  
 #  RootSelect : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Selects the root of a hierarchy first, subsequent clicks will select children objects.
> ``` lang=cpp, name=Nada
> var RootSelect : Boolean


---  
 #  SmartGroupSelect : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> If a parent of a hierarchy is already selected drag select will only select all the children of the currently selected parent.
> ``` lang=cpp, name=Nada
> var SmartGroupSelect : Boolean


---  
 #  Methods


---  
 #  RayCast : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |viewport|[viewport](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/viewport.md)| |
> |mousePosition|[real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)| |
> ``` lang=cpp, name=Nada
> function RayCast(viewport : Viewport, mousePosition : Real2) : Cog
> ``` 


---  
 #  SelectTool : Void

 `constructor`

> Constructor.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function SelectTool()
> ``` 


---  
 #  SmartSelect : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |selection|[metaselection](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/metaselection.md)| |
> |toSelect|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |rootSelect|[boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)| |
> |archetypeSelect|[boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)| |
> ``` lang=cpp, name=Nada
> function SmartSelect(selection : MetaSelection, toSelect : Cog, rootSelect : Boolean, archetypeSelect : Boolean) : Cog
> ``` 


---  
 

 
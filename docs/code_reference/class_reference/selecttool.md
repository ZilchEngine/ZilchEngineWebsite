 `Component` `Editor`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ RayCast](selecttool.md#raycast-zilch-engine-docu)|[ ArchetypeSelect](selecttool.md#archetypeselect-zilch-eng)|[component](component.md)| |
|[ Constructor](selecttool.md#selecttool-void)|[ Raycaster](selecttool.md#raycaster-zilch-engine-do)| | |
|[ SmartSelect](selecttool.md#smartselect-zilch-engine)|[ RootSelect](selecttool.md#rootselect-zilch-engine-d)| | |
| |[ SmartGroupSelect](selecttool.md#smartgroupselect-zilch-en)| | |


 #  Properties


---  
 #  ArchetypeSelect : [boolean](../nada_base_types/boolean.md)

> Selects the root archetype of the tree, subsequent clicks will select the nearest archetype followed by any direct children following that.
> ```TS:Nada
> var ArchetypeSelect : Boolean


---  
 #  Raycaster : [raycaster](raycaster.md)

> 
> ```TS:Nada
> var Raycaster : Raycaster


---  
 #  RootSelect : [boolean](../nada_base_types/boolean.md)

> Selects the root of a hierarchy first, subsequent clicks will select children objects.
> ```TS:Nada
> var RootSelect : Boolean


---  
 #  SmartGroupSelect : [boolean](../nada_base_types/boolean.md)

> If a parent of a hierarchy is already selected drag select will only select all the children of the currently selected parent.
> ```TS:Nada
> var SmartGroupSelect : Boolean


---  
 #  Methods


---  
 #  RayCast : [cog](cog.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |viewport|[viewport](viewport.md)| |
> |mousePosition|[real2](../nada_base_types/real2.md)| |
> ```TS:Nada
> function RayCast(viewport : Viewport, mousePosition : Real2) : Cog
> ``` 


---  
 #  SelectTool : Void

 `constructor`

> Constructor.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function SelectTool()
> ``` 


---  
 #  SmartSelect : [cog](cog.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |selection|[metaselection](metaselection.md)| |
> |toSelect|[cog](cog.md)| |
> |rootSelect|[boolean](../nada_base_types/boolean.md)| |
> |archetypeSelect|[boolean](../nada_base_types/boolean.md)| |
> ```TS:Nada
> function SmartSelect(selection : MetaSelection, toSelect : Cog, rootSelect : Boolean, archetypeSelect : Boolean) : Cog
> ``` 


---  
 

 
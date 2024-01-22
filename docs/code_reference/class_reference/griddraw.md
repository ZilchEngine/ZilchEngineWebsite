 `Component` `Editor`



(NOTE) A component used for drawing a grid.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](griddraw.md#griddraw-void)|[Active](griddraw.md#active-zilch-engine-docum)|[component](component.md)| |
| |[AlwaysDrawInEditor](griddraw.md#alwaysdrawineditor-zero)| | |
| |[Axis](griddraw.md#axis-zilch-engine-documen)| | |
| |[CellSize](griddraw.md#cellsize-zilch-engine-doc)| | |
| |[DrawAxisOrigins](griddraw.md#drawaxisorigins-zilch-eng)| | |
| |[DrawInGame](griddraw.md#drawingame-zilch-engine-d)| | |
| |[FollowEditorCamera](griddraw.md#followeditorcamera-zero)| | |
| |[GridColor](griddraw.md#gridcolor-zilch-engine-do)| | |
| |[GridHighlight](griddraw.md#gridhighlight-zilch-engin)| | |
| |[HalfCellOffset](griddraw.md#halfcelloffset-zilch-engi)| | |
| |[HighlightInterval](griddraw.md#highlightinterval-zilch-e)| | |
| |[Lines](griddraw.md#lines-zilch-engine-docume)| | |


 #  Properties


---  
 #  Active : [boolean](../nada_base_types/boolean.md)

> 
> ```TS:Nada
> var Active : Boolean


---  
 #  AlwaysDrawInEditor : [boolean](../nada_base_types/boolean.md)

> Always draw the grid in editor (not just when it's selected)
> ```TS:Nada
> var AlwaysDrawInEditor : Boolean


---  
 #  Axis : [AxisDirection](../enum_reference.md#axisdirection)

> 
> ```TS:Nada
> var Axis : AxisDirection


---  
 #  CellSize : [real](../nada_base_types/real.md)

> The deltas in the grid (how far apart we draw grid lines)
> ```TS:Nada
> var CellSize : Real


---  
 #  DrawAxisOrigins : [boolean](../nada_base_types/boolean.md)

> Changes the line color to.
> ```TS:Nada
> var DrawAxisOrigins : Boolean


---  
 #  DrawInGame : [boolean](../nada_base_types/boolean.md)

> Draw the grid in the game.
> ```TS:Nada
> var DrawInGame : Boolean


---  
 #  FollowEditorCamera : [boolean](../nada_base_types/boolean.md)

> Move with the editor camera?
> ```TS:Nada
> var FollowEditorCamera : Boolean


---  
 #  GridColor : [real4](../nada_base_types/real4.md)

> Color of grid lines.
> ```TS:Nada
> var GridColor : Real4


---  
 #  GridHighlight : [real4](../nada_base_types/real4.md)

> 
> ```TS:Nada
> var GridHighlight : Real4


---  
 #  HalfCellOffset : [boolean](../nada_base_types/boolean.md)

> Is the grid offset by half a unit?
> ```TS:Nada
> var HalfCellOffset : Boolean


---  
 #  HighlightInterval : [integer](../nada_base_types/integer.md)

> How often should cells be activated.
> ```TS:Nada
> var HighlightInterval : Integer


---  
 #  Lines : [integer](../nada_base_types/integer.md)

> The number of lines to draw.
> ```TS:Nada
> var Lines : Integer


---  
 #  Methods


---  
 #  GridDraw : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function GridDraw()
> ``` 


---  
 

 
 `Component` `Editor`



(NOTE) A component used for drawing a grid.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/griddraw.md#griddraw-void)|[ Active](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/griddraw.md#active-zilch-engine-docum)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)| |
| |[ AlwaysDrawInEditor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/griddraw.md#alwaysdrawineditor-zero)| | |
| |[ Axis](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/griddraw.md#axis-zilch-engine-documen)| | |
| |[ CellSize](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/griddraw.md#cellsize-zilch-engine-doc)| | |
| |[ DrawAxisOrigins](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/griddraw.md#drawaxisorigins-zilch-eng)| | |
| |[ DrawInGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/griddraw.md#drawingame-zilch-engine-d)| | |
| |[ FollowEditorCamera](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/griddraw.md#followeditorcamera-zero)| | |
| |[ GridColor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/griddraw.md#gridcolor-zilch-engine-do)| | |
| |[ GridHighlight](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/griddraw.md#gridhighlight-zilch-engin)| | |
| |[ HalfCellOffset](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/griddraw.md#halfcelloffset-zilch-engi)| | |
| |[ HighlightInterval](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/griddraw.md#highlightinterval-zilch-e)| | |
| |[ Lines](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/griddraw.md#lines-zilch-engine-docume)| | |


 #  Properties


---  
 #  Active : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var Active : Boolean


---  
 #  AlwaysDrawInEditor : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Always draw the grid in editor (not just when it's selected)
> ``` lang=cpp, name=Nada
> var AlwaysDrawInEditor : Boolean


---  
 #  Axis : [AxisDirection](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#axisdirection)

> 
> ``` lang=cpp, name=Nada
> var Axis : AxisDirection


---  
 #  CellSize : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The deltas in the grid (how far apart we draw grid lines)
> ``` lang=cpp, name=Nada
> var CellSize : Real


---  
 #  DrawAxisOrigins : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Changes the line color to.
> ``` lang=cpp, name=Nada
> var DrawAxisOrigins : Boolean


---  
 #  DrawInGame : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Draw the grid in the game.
> ``` lang=cpp, name=Nada
> var DrawInGame : Boolean


---  
 #  FollowEditorCamera : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Move with the editor camera?
> ``` lang=cpp, name=Nada
> var FollowEditorCamera : Boolean


---  
 #  GridColor : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

> Color of grid lines.
> ``` lang=cpp, name=Nada
> var GridColor : Real4


---  
 #  GridHighlight : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

> 
> ``` lang=cpp, name=Nada
> var GridHighlight : Real4


---  
 #  HalfCellOffset : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Is the grid offset by half a unit?
> ``` lang=cpp, name=Nada
> var HalfCellOffset : Boolean


---  
 #  HighlightInterval : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> How often should cells be activated.
> ``` lang=cpp, name=Nada
> var HighlightInterval : Integer


---  
 #  Lines : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> The number of lines to draw.
> ``` lang=cpp, name=Nada
> var Lines : Integer


---  
 #  Methods


---  
 #  GridDraw : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function GridDraw()
> ``` 


---  
 

 
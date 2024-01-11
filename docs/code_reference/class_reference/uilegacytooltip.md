 `Editor`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddText](uilegacytooltip.md#addtext-void)|[ BackgroundColor](uilegacytooltip.md#backgroundcolor-zilch-eng)| | |
|[ ClearText](uilegacytooltip.md#cleartext-void)|[ BorderColor](uilegacytooltip.md#bordercolor-zilch-engine)| | |
|[ SetColorScheme](uilegacytooltip.md#setcolorscheme-void)|[ Padding](uilegacytooltip.md#padding-zilch-engine-docu)| | |
|[ SetPlacement](uilegacytooltip.md#setplacement-void)| | | |
|[ SetPriority](uilegacytooltip.md#setpriority-void)| | | |
|[ Constructor](uilegacytooltip.md#uilegacytooltip-void)| | | |


 #  Properties


---  
 #  BackgroundColor : [real4](../nada_base_types/real4.md)

> 
> ```TS:Nada
> var BackgroundColor : Real4


---  
 #  BorderColor : [real4](../nada_base_types/real4.md)

> 
> ```TS:Nada
> var BorderColor : Real4


---  
 #  Padding : [thickness](thickness.md)

> 
> ```TS:Nada
> var Padding : Thickness


---  
 #  Methods


---  
 #  AddText : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[string](../nada_base_types/string.md)| |
> |p1|[real4](../nada_base_types/real4.md)| |
> ```TS:Nada
> function AddText(p0 : String, p1 : Real4)
> ``` 


---  
 #  ClearText : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ClearText()
> ``` 


---  
 #  SetColorScheme : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[ToolTipColorScheme](../enum_reference.md#tooltipcolorscheme)| |
> ```TS:Nada
> function SetColorScheme(p0 : ToolTipColorScheme)
> ``` 


---  
 #  SetPlacement : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[cameraviewport](cameraviewport.md)| |
> |p1|[rectangle](rectangle.md)| |
> ```TS:Nada
> function SetPlacement(p0 : CameraViewport, p1 : Rectangle)
> ``` 


---  
 #  SetPriority : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[IndicatorSide](../enum_reference.md#indicatorside)| |
> |p1|[IndicatorSide](../enum_reference.md#indicatorside)| |
> |p2|[IndicatorSide](../enum_reference.md#indicatorside)| |
> |p3|[IndicatorSide](../enum_reference.md#indicatorside)| |
> ```TS:Nada
> function SetPriority(p0 : IndicatorSide, p1 : IndicatorSide, p2 : IndicatorSide, p3 : IndicatorSide)
> ``` 


---  
 #  UiLegacyToolTip : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function UiLegacyToolTip()
> ``` 


---  
 #  UiLegacyToolTip : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[uilegacytooltip](uilegacytooltip.md)| |
> ```TS:Nada
> function UiLegacyToolTip(p0 : UiLegacyToolTip)
> ``` 


---  
 

 
 `Editor`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uilegacytooltip.md#addtext-void)|[ BackgroundColor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uilegacytooltip.md#backgroundcolor-zilch-eng)| | |
|[ ClearText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uilegacytooltip.md#cleartext-void)|[ BorderColor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uilegacytooltip.md#bordercolor-zilch-engine)| | |
|[ SetColorScheme](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uilegacytooltip.md#setcolorscheme-void)|[ Padding](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uilegacytooltip.md#padding-zilch-engine-docu)| | |
|[ SetPlacement](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uilegacytooltip.md#setplacement-void)| | | |
|[ SetPriority](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uilegacytooltip.md#setpriority-void)| | | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uilegacytooltip.md#uilegacytooltip-void)| | | |


 #  Properties


---  
 #  BackgroundColor : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

> 
> ``` lang=cpp, name=Nada
> var BackgroundColor : Real4


---  
 #  BorderColor : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

> 
> ``` lang=cpp, name=Nada
> var BorderColor : Real4


---  
 #  Padding : [thickness](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/thickness.md)

> 
> ``` lang=cpp, name=Nada
> var Padding : Thickness


---  
 #  Methods


---  
 #  AddText : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |p1|[real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)| |
> ``` lang=cpp, name=Nada
> function AddText(p0 : String, p1 : Real4)
> ``` 


---  
 #  ClearText : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ClearText()
> ``` 


---  
 #  SetColorScheme : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[ToolTipColorScheme](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#tooltipcolorscheme)| |
> ``` lang=cpp, name=Nada
> function SetColorScheme(p0 : ToolTipColorScheme)
> ``` 


---  
 #  SetPlacement : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[cameraviewport](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cameraviewport.md)| |
> |p1|[rectangle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rectangle.md)| |
> ``` lang=cpp, name=Nada
> function SetPlacement(p0 : CameraViewport, p1 : Rectangle)
> ``` 


---  
 #  SetPriority : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[IndicatorSide](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#indicatorside)| |
> |p1|[IndicatorSide](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#indicatorside)| |
> |p2|[IndicatorSide](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#indicatorside)| |
> |p3|[IndicatorSide](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#indicatorside)| |
> ``` lang=cpp, name=Nada
> function SetPriority(p0 : IndicatorSide, p1 : IndicatorSide, p2 : IndicatorSide, p3 : IndicatorSide)
> ``` 


---  
 #  UiLegacyToolTip : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function UiLegacyToolTip()
> ``` 


---  
 #  UiLegacyToolTip : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[uilegacytooltip](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uilegacytooltip.md)| |
> ``` lang=cpp, name=Nada
> function UiLegacyToolTip(p0 : UiLegacyToolTip)
> ``` 


---  
 

 
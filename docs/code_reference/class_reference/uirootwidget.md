 `Component` `UiWidget`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Render](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uirootwidget.md#render-void)|[ DebugMouseInteraction](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uirootwidget.md#debugmouseinteraction-ze)|[uiwidget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidget.md)| |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uirootwidget.md#uirootwidget-void)|[ DebugSelected](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uirootwidget.md#debugselected-zilch-engin)| | |
|[ Update](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uirootwidget.md#update-void)|[ DepthSeparation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uirootwidget.md#depthseparation-zilch-eng)| | |
| |[ DoubleClickTime](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uirootwidget.md#doubleclicktime-zilch-eng)| | |
| |[ FocusWidget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uirootwidget.md#focuswidget-zilch-engine)| | |
| |[ MouseDownWidget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uirootwidget.md#mousedownwidget-zilch-eng)| | |
| |[ MouseHoldTime](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uirootwidget.md#mouseholdtime-zilch-engin)| | |
| |[ MouseHoverTime](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uirootwidget.md#mousehovertime-zilch-engi)| | |
| |[ MouseOverWidget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uirootwidget.md#mouseoverwidget-zilch-eng)| | |


 #  Properties


---  
 #  DebugMouseInteraction : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Whether or not to print out debug information to the console about what the mouse is currently doing.
> ``` lang=cpp, name=Nada
> var DebugMouseInteraction : Boolean


---  
 #  DebugSelected : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> 
> ``` lang=cpp, name=Nada
> var DebugSelected : Cog


---  
 #  DepthSeparation : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Used for debugging.
> ``` lang=cpp, name=Nada
> var DepthSeparation : Real


---  
 #  DoubleClickTime : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The amount of time between clicks to send the 'DoubleClick' event.
> ``` lang=cpp, name=Nada
> var DoubleClickTime : Real


---  
 #  FocusWidget : [uiwidget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidget.md)

> The widget that currently has focus.
> ``` lang=cpp, name=Nada
> var FocusWidget : UiWidget


---  
 #  MouseDownWidget : [uiwidget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidget.md)

 `read-only`

> The widget that the mouse was pressed down on.
> ``` lang=cpp, name=Nada
> var MouseDownWidget : UiWidget


---  
 #  MouseHoldTime : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Only send the 'MouseHold' event when the mouse has been holding on a single widget for this amount of time.
> ``` lang=cpp, name=Nada
> var MouseHoldTime : Real


---  
 #  MouseHoverTime : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Only send the MouseHover event when the mouse has been over a single widget for this amount of time.
> ``` lang=cpp, name=Nada
> var MouseHoverTime : Real


---  
 #  MouseOverWidget : [uiwidget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uiwidget.md)

 `read-only`

> The widget that the mouse is currently over.
> ``` lang=cpp, name=Nada
> var MouseOverWidget : UiWidget


---  
 #  Methods


---  
 #  Render : Void

> Renders the Ui to the given color render target. The depth render target must have stencil.
> |Name|Type|Description|
> |---|---|---|
> |e|[rendertasksevent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rendertasksevent.md)| |
> |color|[rendertarget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rendertarget.md)| |
> |depth|[rendertarget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rendertarget.md)| |
> |renderPass|[materialblock](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/materialblock.md)| |
> ``` lang=cpp, name=Nada
> function Render(e : RenderTasksEvent, color : RenderTarget, depth : RenderTarget, renderPass : MaterialBlock)
> ``` 


---  
 #  UiRootWidget : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function UiRootWidget()
> ``` 


---  
 #  Update : Void

> Updates all widgets and layouts that need to be updated. This should be called right before rendering.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Update()
> ``` 


---  
 

 
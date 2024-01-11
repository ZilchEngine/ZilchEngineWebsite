 `Component` `UiWidget`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Render](uirootwidget.md#render-void)|[ DebugMouseInteraction](uirootwidget.md#debugmouseinteraction-ze)|[uiwidget](uiwidget.md)| |
|[ Constructor](uirootwidget.md#uirootwidget-void)|[ DebugSelected](uirootwidget.md#debugselected-zilch-engin)| | |
|[ Update](uirootwidget.md#update-void)|[ DepthSeparation](uirootwidget.md#depthseparation-zilch-eng)| | |
| |[ DoubleClickTime](uirootwidget.md#doubleclicktime-zilch-eng)| | |
| |[ FocusWidget](uirootwidget.md#focuswidget-zilch-engine)| | |
| |[ MouseDownWidget](uirootwidget.md#mousedownwidget-zilch-eng)| | |
| |[ MouseHoldTime](uirootwidget.md#mouseholdtime-zilch-engin)| | |
| |[ MouseHoverTime](uirootwidget.md#mousehovertime-zilch-engi)| | |
| |[ MouseOverWidget](uirootwidget.md#mouseoverwidget-zilch-eng)| | |


 #  Properties


---  
 #  DebugMouseInteraction : [boolean](../nada_base_types/boolean.md)

> Whether or not to print out debug information to the console about what the mouse is currently doing.
> ```TS:Nada
> var DebugMouseInteraction : Boolean


---  
 #  DebugSelected : [cog](cog.md)

> 
> ```TS:Nada
> var DebugSelected : Cog


---  
 #  DepthSeparation : [real](../nada_base_types/real.md)

> Used for debugging.
> ```TS:Nada
> var DepthSeparation : Real


---  
 #  DoubleClickTime : [real](../nada_base_types/real.md)

> The amount of time between clicks to send the 'DoubleClick' event.
> ```TS:Nada
> var DoubleClickTime : Real


---  
 #  FocusWidget : [uiwidget](uiwidget.md)

> The widget that currently has focus.
> ```TS:Nada
> var FocusWidget : UiWidget


---  
 #  MouseDownWidget : [uiwidget](uiwidget.md)

 `read-only`

> The widget that the mouse was pressed down on.
> ```TS:Nada
> var MouseDownWidget : UiWidget


---  
 #  MouseHoldTime : [real](../nada_base_types/real.md)

> Only send the 'MouseHold' event when the mouse has been holding on a single widget for this amount of time.
> ```TS:Nada
> var MouseHoldTime : Real


---  
 #  MouseHoverTime : [real](../nada_base_types/real.md)

> Only send the MouseHover event when the mouse has been over a single widget for this amount of time.
> ```TS:Nada
> var MouseHoverTime : Real


---  
 #  MouseOverWidget : [uiwidget](uiwidget.md)

 `read-only`

> The widget that the mouse is currently over.
> ```TS:Nada
> var MouseOverWidget : UiWidget


---  
 #  Methods


---  
 #  Render : Void

> Renders the Ui to the given color render target. The depth render target must have stencil.
> |Name|Type|Description|
> |---|---|---|
> |e|[rendertasksevent](rendertasksevent.md)| |
> |color|[rendertarget](rendertarget.md)| |
> |depth|[rendertarget](rendertarget.md)| |
> |renderPass|[materialblock](materialblock.md)| |
> ```TS:Nada
> function Render(e : RenderTasksEvent, color : RenderTarget, depth : RenderTarget, renderPass : MaterialBlock)
> ``` 


---  
 #  UiRootWidget : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function UiRootWidget()
> ``` 


---  
 #  Update : Void

> Updates all widgets and layouts that need to be updated. This should be called right before rendering.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Update()
> ``` 


---  
 

 
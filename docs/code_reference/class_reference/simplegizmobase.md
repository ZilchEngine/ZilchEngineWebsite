 `Component` `Editor`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](simplegizmobase.md#simplegizmobase-void)|[ Color](simplegizmobase.md#color-zilch-engine-docume)|[component](component.md)|[arrowgizmo](arrowgizmo.md)|
| |[ DrawOnTop](simplegizmobase.md#drawontop-zilch-engine-do)| |[ringgizmo](ringgizmo.md)|
| |[ HoverColor](simplegizmobase.md#hovercolor-zilch-engine-d)| |[squaregizmo](squaregizmo.md)|
| |[ MouseInput](simplegizmobase.md#mouseinput-zilch-engine-d)| | |
| |[ PickingPriority](simplegizmobase.md#pickingpriority-zilch-eng)| | |
| |[ UseParentAsViewScaleOrigin](simplegizmobase.md#useparentasviewscaleorig)| | |
| |[ ViewScaled](simplegizmobase.md#viewscaled-zilch-engine-d)| | |


 #  Properties


---  
 #  Color : [real4](../nada_base_types/real4.md)

> Display colors.
> ``` lang=cpp, name=Nada
> var Color : Real4


---  
 #  DrawOnTop : [boolean](../nada_base_types/boolean.md)

> Whether or not to draw on top of all objects regardless of depth.
> ``` lang=cpp, name=Nada
> var DrawOnTop : Boolean


---  
 #  HoverColor : [real4](../nada_base_types/real4.md)

> 
> ``` lang=cpp, name=Nada
> var HoverColor : Real4


---  
 #  MouseInput : [boolean](../nada_base_types/boolean.md)

> Whether or not this Gizmo should receive mouse input.
> ``` lang=cpp, name=Nada
> var MouseInput : Boolean


---  
 #  PickingPriority : [integer](../nada_base_types/integer.md)

> Used to manually determine which Gizmo gets selected when the mouse is over multiple Gizmos. Higher priority will get picked first.
> ``` lang=cpp, name=Nada
> var PickingPriority : Integer


---  
 #  UseParentAsViewScaleOrigin : [boolean](../nada_base_types/boolean.md)

> If enabled, the gizmo will scale around it's parent.
> ``` lang=cpp, name=Nada
> var UseParentAsViewScaleOrigin : Boolean


---  
 #  ViewScaled : [boolean](../nada_base_types/boolean.md)

> If enabled, the size of the gizmo will stay the same regardless of how far away the camera is.
> ``` lang=cpp, name=Nada
> var ViewScaled : Boolean


---  
 #  Methods


---  
 #  SimpleGizmoBase : Void

 `constructor`

> Constructor.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function SimpleGizmoBase()
> ``` 


---  
 

 
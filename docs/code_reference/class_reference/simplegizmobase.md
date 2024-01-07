 `Component` `Editor`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simplegizmobase.md#simplegizmobase-void)|[ Color](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simplegizmobase.md#color-zilch-engine-docume)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)|[arrowgizmo](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/arrowgizmo.md)|
| |[ DrawOnTop](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simplegizmobase.md#drawontop-zilch-engine-do)| |[ringgizmo](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ringgizmo.md)|
| |[ HoverColor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simplegizmobase.md#hovercolor-zilch-engine-d)| |[squaregizmo](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/squaregizmo.md)|
| |[ MouseInput](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simplegizmobase.md#mouseinput-zilch-engine-d)| | |
| |[ PickingPriority](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simplegizmobase.md#pickingpriority-zilch-eng)| | |
| |[ UseParentAsViewScaleOrigin](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simplegizmobase.md#useparentasviewscaleorig)| | |
| |[ ViewScaled](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simplegizmobase.md#viewscaled-zilch-engine-d)| | |


 #  Properties


---  
 #  Color : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

> Display colors.
> ``` lang=cpp, name=Nada
> var Color : Real4


---  
 #  DrawOnTop : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Whether or not to draw on top of all objects regardless of depth.
> ``` lang=cpp, name=Nada
> var DrawOnTop : Boolean


---  
 #  HoverColor : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

> 
> ``` lang=cpp, name=Nada
> var HoverColor : Real4


---  
 #  MouseInput : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Whether or not this Gizmo should receive mouse input.
> ``` lang=cpp, name=Nada
> var MouseInput : Boolean


---  
 #  PickingPriority : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> Used to manually determine which Gizmo gets selected when the mouse is over multiple Gizmos. Higher priority will get picked first.
> ``` lang=cpp, name=Nada
> var PickingPriority : Integer


---  
 #  UseParentAsViewScaleOrigin : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> If enabled, the gizmo will scale around it's parent.
> ``` lang=cpp, name=Nada
> var UseParentAsViewScaleOrigin : Boolean


---  
 #  ViewScaled : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

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
 

 
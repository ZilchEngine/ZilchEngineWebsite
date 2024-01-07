 `Event` `Widget`



(NOTE) Mouse events for actions concerning the mouse.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ IsButtonUp](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mouseevent.md#isbuttonup-zilch-engine-d)|[ AltPressed](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mouseevent.md#altpressed-zilch-engine-d)|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)|[mousedragevent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mousedragevent.md)|
| |[ Button](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mouseevent.md#button-zilch-engine-docum)| |[mousefiledropevent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mousefiledropevent.md)|
| |[ ButtonDown](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mouseevent.md#buttondown-zilch-engine-d)| |[viewportmouseevent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/viewportmouseevent.md)|
| |[ CtrlPressed](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mouseevent.md#ctrlpressed-zilch-engine)| | |
| |[ HandledEvent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mouseevent.md#handledevent-zilch-engine)| | |
| |[ Mouse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mouseevent.md#mouse-zilch-engine-docume)| | |
| |[ Movement](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mouseevent.md#movement-zilch-engine-doc)| | |
| |[ Position](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mouseevent.md#position-zilch-engine-doc)| | |
| |[ Scroll](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mouseevent.md#scroll-zilch-engine-docum)| | |
| |[ ShiftPressed](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mouseevent.md#shiftpressed-zilch-engine)| | |


 #  Properties


---  
 #  AltPressed : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var AltPressed : Boolean


---  
 #  Button : [MouseButtons](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#mousebuttons)

> 
> ``` lang=cpp, name=Nada
> var Button : MouseButtons


---  
 #  ButtonDown : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> State of all the mouse buttons.
> ``` lang=cpp, name=Nada
> var ButtonDown : Boolean


---  
 #  CtrlPressed : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var CtrlPressed : Boolean


---  
 #  HandledEvent : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var HandledEvent : Boolean


---  
 #  Mouse : [mouse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mouse.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Mouse : Mouse


---  
 #  Movement : [real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)

> 
> ``` lang=cpp, name=Nada
> var Movement : Real2


---  
 #  Position : [real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)

> 
> ``` lang=cpp, name=Nada
> var Position : Real2


---  
 #  Scroll : [real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)

> 
> ``` lang=cpp, name=Nada
> var Scroll : Real2


---  
 #  ShiftPressed : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var ShiftPressed : Boolean


---  
 #  Methods


---  
 #  IsButtonUp : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |button|[MouseButtons](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#mousebuttons)| |
> ``` lang=cpp, name=Nada
> function IsButtonUp(button : MouseButtons) : Boolean
> ``` 


---  
 

 
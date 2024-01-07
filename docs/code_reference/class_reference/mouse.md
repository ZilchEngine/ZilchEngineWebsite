 `Engine`

(NOTE) Mouse object for Display System.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ IsButtonDown](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mouse.md#isbuttondown-zilch-engine)|[ ClientPosition](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mouse.md#clientposition-zilch-engi)|[eventobject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/eventobject.md)| |
|[ ToggleTrapped](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mouse.md#toggletrapped-void)|[ Cursor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mouse.md#cursor-zilch-engine-docum)| | |
| |[ CursorMovement](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mouse.md#cursormovement-zilch-engi)| | |
| |[ RawMovement](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mouse.md#rawmovement-zilch-engine)| | |
| |[ Trapped](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mouse.md#trapped-zilch-engine-docu)| | |


 #  Properties


---  
 #  ClientPosition : [real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)

 `read-only`

> The position of the mouse cursor relative to the application's top-left corner in pixels.
> ``` lang=cpp, name=Nada
> var ClientPosition : Real2


---  
 #  Cursor : [Cursor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#cursor)

> Set the cursor of the mouse.
> ``` lang=cpp, name=Nada
> var Cursor : Cursor


---  
 #  CursorMovement : [real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)

 `read-only`

> The movement of the mouse in pixels.
> ``` lang=cpp, name=Nada
> var CursorMovement : Real2


---  
 #  RawMovement : [real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)

> High precision raw movement of the mouse.
> ``` lang=cpp, name=Nada
> var RawMovement : Real2


---  
 #  Trapped : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Trap the mouse preventing it from moving.
> ``` lang=cpp, name=Nada
> var Trapped : Boolean


---  
 #  Methods


---  
 #  IsButtonDown : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Is a mouse button currently down?
> |Name|Type|Description|
> |---|---|---|
> |button|[MouseButtons](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#mousebuttons)| |
> ``` lang=cpp, name=Nada
> function IsButtonDown(button : MouseButtons) : Boolean
> ``` 


---  
 #  ToggleTrapped : Void

> Toggles if the mouse is currently trapped.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ToggleTrapped()
> ``` 


---  
 

 
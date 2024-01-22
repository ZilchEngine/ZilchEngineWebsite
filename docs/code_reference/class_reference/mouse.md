 `Engine`

(NOTE) Mouse object for Display System.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[IsButtonDown](mouse.md#isbuttondown-zilch-engine)|[ClientPosition](mouse.md#clientposition-zilch-engi)|[eventobject](eventobject.md)| |
|[ToggleTrapped](mouse.md#toggletrapped-void)|[Cursor](mouse.md#cursor-zilch-engine-docum)| | |
| |[CursorMovement](mouse.md#cursormovement-zilch-engi)| | |
| |[RawMovement](mouse.md#rawmovement-zilch-engine)| | |
| |[Trapped](mouse.md#trapped-zilch-engine-docu)| | |


 #  Properties


---  
 #  ClientPosition : [real2](../nada_base_types/real2.md)

 `read-only`

> The position of the mouse cursor relative to the application's top-left corner in pixels.
> ```TS:Nada
> var ClientPosition : Real2


---  
 #  Cursor : [Cursor](../enum_reference.md#cursor)

> Set the cursor of the mouse.
> ```TS:Nada
> var Cursor : Cursor


---  
 #  CursorMovement : [real2](../nada_base_types/real2.md)

 `read-only`

> The movement of the mouse in pixels.
> ```TS:Nada
> var CursorMovement : Real2


---  
 #  RawMovement : [real2](../nada_base_types/real2.md)

> High precision raw movement of the mouse.
> ```TS:Nada
> var RawMovement : Real2


---  
 #  Trapped : [boolean](../nada_base_types/boolean.md)

> Trap the mouse preventing it from moving.
> ```TS:Nada
> var Trapped : Boolean


---  
 #  Methods


---  
 #  IsButtonDown : [boolean](../nada_base_types/boolean.md)

> Is a mouse button currently down?
> |Name|Type|Description|
> |---|---|---|
> |button|[MouseButtons](../enum_reference.md#mousebuttons)| |
> ```TS:Nada
> function IsButtonDown(button : MouseButtons) : Boolean
> ``` 


---  
 #  ToggleTrapped : Void

> Toggles if the mouse is currently trapped.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ToggleTrapped()
> ``` 


---  
 

 
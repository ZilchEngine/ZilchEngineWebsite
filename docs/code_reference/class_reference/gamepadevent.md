 `Event` `Engine`



(NOTE) Gamepad events are send when a game pad button state is changed.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[Button](gamepadevent.md#button-zilch-engine-docum)|[event](event.md)| |
| |[FlickDirection](gamepadevent.md#flickdirection-zilch-engi)| | |
| |[FlickedStick](gamepadevent.md#flickedstick-zilch-engine)| | |
| |[Gamepad](gamepadevent.md#gamepad-zilch-engine-docu)| | |


 #  Properties


---  
 #  Button : [integer](../nada_base_types/integer.md)

> Button that was just pressed down or released up.
> ```TS:Nada
> var Button : Integer


---  
 #  FlickDirection : [real2](../nada_base_types/real2.md)

> The direction of the stick that was flicked (normalized)
> ```TS:Nada
> var FlickDirection : Real2


---  
 #  FlickedStick : [FlickedStick](../enum_reference.md#flickedstick)

> When responding to the 'GamepadStickFlicked' event, this will be set to the stick that was flicked.
> ```TS:Nada
> var FlickedStick : FlickedStick


---  
 #  Gamepad : [gamepad](gamepad.md)

> Gamepad that generated this event.
> ```TS:Nada
> var Gamepad : Gamepad


---  
 #  Methods


---  
 

 
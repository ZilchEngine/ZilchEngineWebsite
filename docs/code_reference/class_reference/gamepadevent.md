 `Event` `Engine`



(NOTE) Gamepad events are send when a game pad button state is changed.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ Button](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepadevent.md#button-zilch-engine-docum)|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
| |[ FlickDirection](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepadevent.md#flickdirection-zilch-engi)| | |
| |[ FlickedStick](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepadevent.md#flickedstick-zilch-engine)| | |
| |[ Gamepad](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepadevent.md#gamepad-zilch-engine-docu)| | |


 #  Properties


---  
 #  Button : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> Button that was just pressed down or released up.
> ``` lang=cpp, name=Nada
> var Button : Integer


---  
 #  FlickDirection : [real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)

> The direction of the stick that was flicked (normalized)
> ``` lang=cpp, name=Nada
> var FlickDirection : Real2


---  
 #  FlickedStick : [FlickedStick](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#flickedstick)

> When responding to the 'GamepadStickFlicked' event, this will be set to the stick that was flicked.
> ``` lang=cpp, name=Nada
> var FlickedStick : FlickedStick


---  
 #  Gamepad : [gamepad](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepad.md)

> Gamepad that generated this event.
> ``` lang=cpp, name=Nada
> var Gamepad : Gamepad


---  
 #  Methods


---  
 

 
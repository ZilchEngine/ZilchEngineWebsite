 `Engine`

(NOTE) Gamepads is a collection of gamepads.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetGamePad](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepads.md#getgamepad-zilch-engine-d)|[ MaxGamepadCount](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepads.md#maxgamepadcount-zilch-eng)|[eventobject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/eventobject.md)| |
|[ PauseVibration](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepads.md#pausevibration-void)| | | |
|[ ResumeVibration](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepads.md#resumevibration-void)| | | |


 #  Properties


---  
 #  MaxGamepadCount : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Gets the maximum number of supported gamepads.
> ``` lang=cpp, name=Nada
> var MaxGamepadCount : Integer


---  
 #  Methods


---  
 #  GetGamePad : [gamepad](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepad.md)

> Get the gamepad for a given index from [0, GamepadCount].
> |Name|Type|Description|
> |---|---|---|
> |gamepadIndex|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function GetGamePad(gamepadIndex : Integer) : Gamepad
> ``` 


---  
 #  PauseVibration : Void

> Pause Vibration on all gamepads.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function PauseVibration()
> ``` 


---  
 #  ResumeVibration : Void

> Resume vibration on all gamepads.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ResumeVibration()
> ``` 


---  
 

 
 `Engine`

(NOTE) Gamepads is a collection of gamepads.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetGamePad](gamepads.md#getgamepad-zilch-engine-d)|[ MaxGamepadCount](gamepads.md#maxgamepadcount-zilch-eng)|[eventobject](eventobject.md)| |
|[ PauseVibration](gamepads.md#pausevibration-void)| | | |
|[ ResumeVibration](gamepads.md#resumevibration-void)| | | |


 #  Properties


---  
 #  MaxGamepadCount : [integer](../nada_base_types/integer.md)

 `read-only`

> Gets the maximum number of supported gamepads.
> ```TS:Nada
> var MaxGamepadCount : Integer


---  
 #  Methods


---  
 #  GetGamePad : [gamepad](gamepad.md)

> Get the gamepad for a given index from [0, GamepadCount].
> |Name|Type|Description|
> |---|---|---|
> |gamepadIndex|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function GetGamePad(gamepadIndex : Integer) : Gamepad
> ``` 


---  
 #  PauseVibration : Void

> Pause Vibration on all gamepads.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function PauseVibration()
> ``` 


---  
 #  ResumeVibration : Void

> Resume vibration on all gamepads.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ResumeVibration()
> ``` 


---  
 

 
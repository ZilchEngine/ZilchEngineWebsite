 `Engine`

(NOTE) Game pad is a object for getting game pad input.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ IsButtonHeld](gamepad.md#isbuttonheld-zilch-engine)|[ GamepadIndex](gamepad.md#gamepadindex-zilch-engine)|[eventobject](eventobject.md)| |
|[ IsButtonPressed](gamepad.md#isbuttonpressed-zilch-eng)|[ IsActive](gamepad.md#isactive-zilch-engine-doc)| | |
|[ IsButtonReleased](gamepad.md#isbuttonreleased-zilch-en)|[ LeftStick](gamepad.md#leftstick-zilch-engine-do)| | |
|[ TimeButtonHeld](gamepad.md#timebuttonheld-zilch-engi)|[ LeftStickDelta](gamepad.md#leftstickdelta-zilch-engi)| | |
|[ Vibrate](gamepad.md#vibrate-void)|[ LeftTrigger](gamepad.md#lefttrigger-zilch-engine)| | |
| |[ RightStick](gamepad.md#rightstick-zilch-engine-d)| | |
| |[ RightStickDelta](gamepad.md#rightstickdelta-zilch-eng)| | |
| |[ RightTrigger](gamepad.md#righttrigger-zilch-engine)| | |


 #  Properties


---  
 #  GamepadIndex : [integer](../nada_base_types/integer.md)

> Index of this gamepad.
> ```TS:Nada
> var GamepadIndex : Integer


---  
 #  IsActive : [boolean](../nada_base_types/boolean.md)

> Is this controller turned on and plugged in.
> ```TS:Nada
> var IsActive : Boolean


---  
 #  LeftStick : [real2](../nada_base_types/real2.md)

> Current offset [-1,1] from the center of the left stick.
> ```TS:Nada
> var LeftStick : Real2


---  
 #  LeftStickDelta : [real2](../nada_base_types/real2.md)

> Change in the left stick this frame.
> ```TS:Nada
> var LeftStickDelta : Real2


---  
 #  LeftTrigger : [real](../nada_base_types/real.md)

> Value of how much the Left Trigger is down. Range [0,1].
> ```TS:Nada
> var LeftTrigger : Real


---  
 #  RightStick : [real2](../nada_base_types/real2.md)

> Current offset [-1,1] from the center of the right stick.
> ```TS:Nada
> var RightStick : Real2


---  
 #  RightStickDelta : [real2](../nada_base_types/real2.md)

> Change in the right stick this frame.
> ```TS:Nada
> var RightStickDelta : Real2


---  
 #  RightTrigger : [real](../nada_base_types/real.md)

> Value of how much the Right Trigger is down. Range [0,1].
> ```TS:Nada
> var RightTrigger : Real


---  
 #  Methods


---  
 #  IsButtonHeld : [boolean](../nada_base_types/boolean.md)

> Is the button currently being held down.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function IsButtonHeld(index : Integer) : Boolean
> ``` 


---  
 #  IsButtonPressed : [boolean](../nada_base_types/boolean.md)

> Has the button just been pressed this frame.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function IsButtonPressed(index : Integer) : Boolean
> ``` 


---  
 #  IsButtonReleased : [boolean](../nada_base_types/boolean.md)

> Is the button just been released.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function IsButtonReleased(index : Integer) : Boolean
> ``` 


---  
 #  TimeButtonHeld : [real](../nada_base_types/real.md)

> How long has this button been held down.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function TimeButtonHeld(index : Integer) : Real
> ``` 


---  
 #  Vibrate : Void

> Vibrate this controller for a given time. Speed is a value between zero and one.
> |Name|Type|Description|
> |---|---|---|
> |time|[real](../nada_base_types/real.md)| |
> |LeftSpeed|[real](../nada_base_types/real.md)| |
> |RightSpeed|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function Vibrate(time : Real, LeftSpeed : Real, RightSpeed : Real)
> ``` 


---  
 

 
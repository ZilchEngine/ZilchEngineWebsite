 `Engine`

(NOTE) Game pad is a object for getting game pad input.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ IsButtonHeld](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepad.md#isbuttonheld-zilch-engine)|[ GamepadIndex](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepad.md#gamepadindex-zilch-engine)|[eventobject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/eventobject.md)| |
|[ IsButtonPressed](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepad.md#isbuttonpressed-zilch-eng)|[ IsActive](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepad.md#isactive-zilch-engine-doc)| | |
|[ IsButtonReleased](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepad.md#isbuttonreleased-zilch-en)|[ LeftStick](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepad.md#leftstick-zilch-engine-do)| | |
|[ TimeButtonHeld](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepad.md#timebuttonheld-zilch-engi)|[ LeftStickDelta](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepad.md#leftstickdelta-zilch-engi)| | |
|[ Vibrate](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepad.md#vibrate-void)|[ LeftTrigger](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepad.md#lefttrigger-zilch-engine)| | |
| |[ RightStick](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepad.md#rightstick-zilch-engine-d)| | |
| |[ RightStickDelta](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepad.md#rightstickdelta-zilch-eng)| | |
| |[ RightTrigger](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepad.md#righttrigger-zilch-engine)| | |


 #  Properties


---  
 #  GamepadIndex : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> Index of this gamepad.
> ``` lang=cpp, name=Nada
> var GamepadIndex : Integer


---  
 #  IsActive : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Is this controller turned on and plugged in.
> ``` lang=cpp, name=Nada
> var IsActive : Boolean


---  
 #  LeftStick : [real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)

> Current offset [-1,1] from the center of the left stick.
> ``` lang=cpp, name=Nada
> var LeftStick : Real2


---  
 #  LeftStickDelta : [real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)

> Change in the left stick this frame.
> ``` lang=cpp, name=Nada
> var LeftStickDelta : Real2


---  
 #  LeftTrigger : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Value of how much the Left Trigger is down. Range [0,1].
> ``` lang=cpp, name=Nada
> var LeftTrigger : Real


---  
 #  RightStick : [real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)

> Current offset [-1,1] from the center of the right stick.
> ``` lang=cpp, name=Nada
> var RightStick : Real2


---  
 #  RightStickDelta : [real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)

> Change in the right stick this frame.
> ``` lang=cpp, name=Nada
> var RightStickDelta : Real2


---  
 #  RightTrigger : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Value of how much the Right Trigger is down. Range [0,1].
> ``` lang=cpp, name=Nada
> var RightTrigger : Real


---  
 #  Methods


---  
 #  IsButtonHeld : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Is the button currently being held down.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function IsButtonHeld(index : Integer) : Boolean
> ``` 


---  
 #  IsButtonPressed : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Has the button just been pressed this frame.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function IsButtonPressed(index : Integer) : Boolean
> ``` 


---  
 #  IsButtonReleased : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Is the button just been released.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function IsButtonReleased(index : Integer) : Boolean
> ``` 


---  
 #  TimeButtonHeld : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> How long has this button been held down.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function TimeButtonHeld(index : Integer) : Real
> ``` 


---  
 #  Vibrate : Void

> Vibrate this controller for a given time. Speed is a value between zero and one.
> |Name|Type|Description|
> |---|---|---|
> |time|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |LeftSpeed|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |RightSpeed|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function Vibrate(time : Real, LeftSpeed : Real, RightSpeed : Real)
> ``` 


---  
 

 
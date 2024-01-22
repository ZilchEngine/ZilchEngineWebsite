 `Engine`

(NOTE) A Joystick is associated with a hardware joystick, and provides the ability to query axes and buttons.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Calibrating](joystick.md#calibrating-zilch-engine)|[AxisCount](joystick.md#axiscount-zilch-engine-do)|[eventobject](eventobject.md)| |
|[EndCalibration](joystick.md#endcalibration-void)|[ButtonCount](joystick.md#buttoncount-zilch-engine)| | |
|[GetAxisIndex](joystick.md#getaxisindex-zilch-engine)|[DisabledValue](joystick.md#disabledvalue-zilch-engin)| | |
|[GetAxisName](joystick.md#getaxisname-zilch-engine)|[IsActive](joystick.md#isactive-zilch-engine-doc)| | |
|[GetAxisValue](joystick.md#getaxisvalue-zilch-engine)|[Name](joystick.md#name-zilch-engine-documen)| | |
|[GetAxisValueByName](joystick.md#getaxisvaluebyname-zero)| | | |
|[GetButtonValue](joystick.md#getbuttonvalue-zilch-engi)| | | |
|[LoadInputMapping](joystick.md#loadinputmapping-void)| | | |
|[SaveInputMapping](joystick.md#saveinputmapping-void)| | | |
|[StartCalibration](joystick.md#startcalibration-void)| | | |


 #  Properties


---  
 #  AxisCount : [integer](../nada_base_types/integer.md)

 `read-only`

> 
> ```TS:Nada
> var AxisCount : Integer


---  
 #  ButtonCount : [integer](../nada_base_types/integer.md)

 `read-only`

> Get the number of buttons or axes.
> ```TS:Nada
> var ButtonCount : Integer


---  
 #  DisabledValue : [real](../nada_base_types/real.md)

 `read-only` `static`

> A value that means a joystick axis is invalid. For example when a HAT-switch is not pressed down, it will return this value.
> ```TS:Nada
> var DisabledValue : Real


---  
 #  IsActive : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Gets whether or not the joystick is active.
> ```TS:Nada
> var IsActive : Boolean


---  
 #  Name : [string](../nada_base_types/string.md)

 `read-only`

> Get the name of the Joystick.
> ```TS:Nada
> var Name : String


---  
 #  Methods


---  
 #  Calibrating : [boolean](../nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Calibrating() : Boolean
> ``` 


---  
 #  EndCalibration : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function EndCalibration()
> ``` 


---  
 #  GetAxisIndex : [integer](../nada_base_types/integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function GetAxisIndex(name : String) : Integer
> ``` 


---  
 #  GetAxisName : [string](../nada_base_types/string.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function GetAxisName(index : Integer) : String
> ``` 


---  
 #  GetAxisValue : [real](../nada_base_types/real.md)

> Queries an axes and returns a value between [-1, 1]. The valid range of axes is between 0 and 'GetMaxAxes'. If the axis is not valid, then the value returned is 0. If the axis is disabled, then the value returned is Joystick.DisabledValue.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function GetAxisValue(index : Integer) : Real
> ``` 


---  
 #  GetAxisValueByName : [real](../nada_base_types/real.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function GetAxisValueByName(name : String) : Real
> ``` 


---  
 #  GetButtonValue : [boolean](../nada_base_types/boolean.md)

> Queries a button and returns true if it is down, false if it is up The valid range of buttons is between 0 and 'GetMaxButtons' If the button is not valid, then the value returned is false.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function GetButtonValue(index : Integer) : Boolean
> ``` 


---  
 #  LoadInputMapping : Void

> Load an input mapping.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function LoadInputMapping(name : String)
> ``` 


---  
 #  SaveInputMapping : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function SaveInputMapping(name : String)
> ``` 


---  
 #  StartCalibration : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function StartCalibration()
> ``` 


---  
 

 
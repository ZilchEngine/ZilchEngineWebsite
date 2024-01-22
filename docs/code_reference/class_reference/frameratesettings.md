 `Component` `Engine`



(NOTE) Settings for how the frame rate of the engine should be controlled.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](frameratesettings.md#frameratesettings-void)|[FrameRate](frameratesettings.md#framerate-zilch-engine-do)|[component](component.md)| |
| |[LimitFrameRate](frameratesettings.md#limitframerate-zilch-engi)| | |
| |[VerticalSync](frameratesettings.md#verticalsync-zilch-engine)| | |


 #  Properties


---  
 #  FrameRate : [integer](../nada_base_types/integer.md)

> How many frames per second the engine should be limited at.
> ```TS:Nada
> var FrameRate : Integer


---  
 #  LimitFrameRate : [boolean](../nada_base_types/boolean.md)

> If the engine should limit the frame rate.
> ```TS:Nada
> var LimitFrameRate : Boolean


---  
 #  VerticalSync : [boolean](../nada_base_types/boolean.md)

> If the frame rate should sync with the monitor's refresh rate, superseded by LimitFrameRate.
> ```TS:Nada
> var VerticalSync : Boolean


---  
 #  Methods


---  
 #  FrameRateSettings : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function FrameRateSettings()
> ``` 


---  
 

 
 `Component` `Engine`



(NOTE) Time space component controls time for a Space.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Step](timespace.md#step-void)|[ Dt](timespace.md#dt-zilch-engine-documenta)|[component](component.md)| |
|[ Constructor](timespace.md#timespace-void)|[ DtOrZero](timespace.md#dtorzilch-zilch-engine-doc)| | |
|[ TogglePause](timespace.md#togglepause-void)|[ Frame](timespace.md#frame-zilch-engine-docume)| | |
| |[ GloballyPaused](timespace.md#globallypaused-zilch-engi)| | |
| |[ MaxDt](timespace.md#maxdt-zilch-engine-docume)| | |
| |[ MinDt](timespace.md#mindt-zilch-engine-docume)| | |
| |[ Paused](timespace.md#paused-zilch-engine-docum)| | |
| |[ RealDt](timespace.md#realdt-zilch-engine-docum)| | |
| |[ RealTimePassed](timespace.md#realtimepassed-zilch-engi)| | |
| |[ StepCount](timespace.md#stepcount-zilch-engine-do)| | |
| |[ TimeMode](timespace.md#timemode-zilch-engine-doc)| | |
| |[ TimePassed](timespace.md#timepassed-zilch-engine-d)| | |
| |[ TimeScale](timespace.md#timescale-zilch-engine-do)| | |


 #  Properties


---  
 #  Dt : [real](../nada_base_types/real.md)

 `read-only`

> 
> ```TS:Nada
> var Dt : Real


---  
 #  DtOrZero : [real](../nada_base_types/real.md)

 `read-only`

> 
> ```TS:Nada
> var DtOrZero : Real


---  
 #  Frame : [integer](../nada_base_types/integer.md)

> The current frame we are on (starts at 0 and counts up for every frame that is run) This value counts up regardless of if the space is paused.
> ```TS:Nada
> var Frame : Integer


---  
 #  GloballyPaused : [boolean](../nada_base_types/boolean.md)

 `read-only`

> 
> ```TS:Nada
> var GloballyPaused : Boolean


---  
 #  MaxDt : [real](../nada_base_types/real.md)

> The maximum amount of time we send when running in 'ActualFrametime' mode If this value is set too high and the user does anything to pause their system or the game (example grabbing the window) then a large frame time will be sent out and physics objects will jump very far (causing tunneling and random bounces)
> ```TS:Nada
> var MaxDt : Real


---  
 #  MinDt : [real](../nada_base_types/real.md)

> The minimum amount of time we send when running in 'ActualFrametime' mode Ideally this is set to a very small non-zero value to prevent any division by zero errors.
> ```TS:Nada
> var MinDt : Real


---  
 #  Paused : [boolean](../nada_base_types/boolean.md)

> If the time space is paused then we cease sending out logic update events When paused, the Dt will remain at whatever it was (it will NOT be set to 0)
> ```TS:Nada
> var Paused : Boolean


---  
 #  RealDt : [real](../nada_base_types/real.md)

 `read-only`

> 
> ```TS:Nada
> var RealDt : Real


---  
 #  RealTimePassed : [real](../nada_base_types/real.md)

> 
> ```TS:Nada
> var RealTimePassed : Real


---  
 #  StepCount : [integer](../nada_base_types/integer.md)

> Causes the engine to update multiple times before rendering a frame.
> ```TS:Nada
> var StepCount : Integer


---  
 #  TimeMode : [TimeMode](../enum_reference.md#timemode)

> When set to fixed framerate the Dt/frame time will never change (it will send whatever the project frame-rate-limiter is set to) This means it is important to run with a frame-rate limiter of some kind otherwise the game will appear to run much faster/slower Note: For determinism, you should always run in FixedFrametime mode When set to actual framerate we will send out the real time that the engine is encountering (clamped by MinDt / MaxDt)
> ```TS:Nada
> var TimeMode : TimeMode


---  
 #  TimePassed : [real](../nada_base_types/real.md)

> 
> ```TS:Nada
> var TimePassed : Real


---  
 #  TimeScale : [real](../nada_base_types/real.md)

> Scale the speed of time for interesting effects like bullet time or fast paced gameplay. TimeScale is clamped to be positive.
> ```TS:Nada
> var TimeScale : Real


---  
 #  Methods


---  
 #  Step : Void

> Allows the engine to be advance one frame forward. Useful for debugging one frame at a time.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Step()
> ``` 


---  
 #  TimeSpace : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function TimeSpace()
> ``` 


---  
 #  TogglePause : Void

> Toggles the state of paused.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function TogglePause()
> ``` 


---  
 

 
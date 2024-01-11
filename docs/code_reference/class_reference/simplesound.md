 `Component` `Sound`



(NOTE) Plays a specified SoundCue, either when created or when the Play method is called.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Play](simplesound.md#play-zilch-engine-documen)|[ Cue](simplesound.md#cue-zilch-engine-document)|[component](component.md)| |
|[ Constructor](simplesound.md#simplesound-void)|[ IsPlaying](simplesound.md#isplaying-zilch-engine-do)| | |
|[ Stop](simplesound.md#stop-void)|[ Paused](simplesound.md#paused-zilch-engine-docum)| | |
| |[ Positional](simplesound.md#positional-zilch-engine-d)| | |
| |[ StartPlaying](simplesound.md#startplaying-zilch-engine)| | |


 #  Properties


---  
 #  Cue : [soundcue](soundcue.md)

> 
> ```TS:Nada
> var Cue : SoundCue


---  
 #  IsPlaying : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Will be true if the SoundCue is currently being played.
> ```TS:Nada
> var IsPlaying : Boolean


---  
 #  Paused : [boolean](../nada_base_types/boolean.md)

> Setting this Property to true will pause a currently playing SoundCue. Setting it to false will resume playback.
> ```TS:Nada
> var Paused : Boolean


---  
 #  Positional : [boolean](../nada_base_types/boolean.md)

> If this property is true the SoundCue will be played positionally (heard at a specific location by SoundListeners) through the SoundEmitter component on the same object. If false, the SoundCue will be played through the SoundSpace, and will NOT be affected by any SoundEmitter settings.
> ```TS:Nada
> var Positional : Boolean


---  
 #  StartPlaying : [boolean](../nada_base_types/boolean.md)

> If this property is true the SoundCue will begin playing as soon as the object is created.
> ```TS:Nada
> var StartPlaying : Boolean


---  
 #  Methods


---  
 #  Play : [soundinstance](soundinstance.md)

> Begins playing the SoundCue chosen in the Cue property and returns the resulting SoundInstance. If already playing it will be stopped and re-started.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Play() : SoundInstance
> ``` 


---  
 #  SimpleSound : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function SimpleSound()
> ``` 


---  
 #  Stop : Void

> Stops a currently playing SoundInstance if it exists.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Stop()
> ``` 


---  
 

 
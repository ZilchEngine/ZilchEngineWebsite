 `Component` `Sound`



(NOTE) Plays a specified SoundCue, either when created or when the Play method is called.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Play](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simplesound.md#play-zilch-engine-documen)|[ Cue](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simplesound.md#cue-zilch-engine-document)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)| |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simplesound.md#simplesound-void)|[ IsPlaying](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simplesound.md#isplaying-zilch-engine-do)| | |
|[ Stop](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simplesound.md#stop-void)|[ Paused](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simplesound.md#paused-zilch-engine-docum)| | |
| |[ Positional](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simplesound.md#positional-zilch-engine-d)| | |
| |[ StartPlaying](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/simplesound.md#startplaying-zilch-engine)| | |


 #  Properties


---  
 #  Cue : [soundcue](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundcue.md)

> 
> ``` lang=cpp, name=Nada
> var Cue : SoundCue


---  
 #  IsPlaying : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> Will be true if the SoundCue is currently being played.
> ``` lang=cpp, name=Nada
> var IsPlaying : Boolean


---  
 #  Paused : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Setting this Property to true will pause a currently playing SoundCue. Setting it to false will resume playback.
> ``` lang=cpp, name=Nada
> var Paused : Boolean


---  
 #  Positional : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> If this property is true the SoundCue will be played positionally (heard at a specific location by SoundListeners) through the SoundEmitter component on the same object. If false, the SoundCue will be played through the SoundSpace, and will NOT be affected by any SoundEmitter settings.
> ``` lang=cpp, name=Nada
> var Positional : Boolean


---  
 #  StartPlaying : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> If this property is true the SoundCue will begin playing as soon as the object is created.
> ``` lang=cpp, name=Nada
> var StartPlaying : Boolean


---  
 #  Methods


---  
 #  Play : [soundinstance](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundinstance.md)

> Begins playing the SoundCue chosen in the Cue property and returns the resulting SoundInstance. If already playing it will be stopped and re-started.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Play() : SoundInstance
> ``` 


---  
 #  SimpleSound : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function SimpleSound()
> ``` 


---  
 #  Stop : Void

> Stops a currently playing SoundInstance if it exists.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Stop()
> ``` 


---  
 

 
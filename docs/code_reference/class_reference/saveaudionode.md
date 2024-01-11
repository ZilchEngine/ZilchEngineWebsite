 `Sound`

(NOTE) Saves audio from its input SoundNodes and then plays it. All audio from inputs is passed to outputs.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ClearSavedAudio](saveaudionode.md#clearsavedaudio-void)|[ SaveAudio](saveaudionode.md#saveaudio-zilch-engine-do)|[soundnode](soundnode.md)| |
|[ PlaySavedAudio](saveaudionode.md#playsavedaudio-void)| | | |
|[ StopPlaying](saveaudionode.md#stopplaying-void)| | | |


 #  Properties


---  
 #  SaveAudio : [boolean](../nada_base_types/boolean.md)

> When true, audio from input SoundNodes will be saved. Setting this to true will remove any existing saved audio before saving more.
> ``` lang=cpp, name=Nada
> var SaveAudio : Boolean


---  
 #  Methods


---  
 #  ClearSavedAudio : Void

> Removes all currently saved audio.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ClearSavedAudio()
> ``` 


---  
 #  PlaySavedAudio : Void

> Plays the saved audio.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function PlaySavedAudio()
> ``` 


---  
 #  StopPlaying : Void

> Stops playing the saved audio.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function StopPlaying()
> ``` 


---  
 

 
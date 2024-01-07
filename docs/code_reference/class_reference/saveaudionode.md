 `Sound`

(NOTE) Saves audio from its input SoundNodes and then plays it. All audio from inputs is passed to outputs.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ClearSavedAudio](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/saveaudionode.md#clearsavedaudio-void)|[ SaveAudio](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/saveaudionode.md#saveaudio-zilch-engine-do)|[soundnode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundnode.md)| |
|[ PlaySavedAudio](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/saveaudionode.md#playsavedaudio-void)| | | |
|[ StopPlaying](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/saveaudionode.md#stopplaying-void)| | | |


 #  Properties


---  
 #  SaveAudio : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

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
 

 
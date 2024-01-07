 `Component` `Sound`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/audiosettings.md#audiosettings-void)|[ LatencySetting](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/audiosettings.md#latencysetting-zilch-engi)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)| |
| |[ MinVolumeThreshold](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/audiosettings.md#minvolumethreshold-zero)| | |
| |[ MixType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/audiosettings.md#mixtype-zilch-engine-docu)| | |
| |[ MuteAllAudio](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/audiosettings.md#muteallaudio-zilch-engine)| | |
| |[ SystemVolume](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/audiosettings.md#systemvolume-zilch-engine)| | |


 #  Properties


---  
 #  LatencySetting : [AudioLatency](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#audiolatency)

> Using the high latency setting can fix some audio problems (such as clicks and static) but can lead to a slight delay in the audio.
> ``` lang=cpp, name=Nada
> var LatencySetting : AudioLatency


---  
 #  MinVolumeThreshold : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Sets the volume threshold at which sounds will be virtualized (they will continue tracking their position and all data but will not process audio). This is a floating point volume number, not decibels.
> ``` lang=cpp, name=Nada
> var MinVolumeThreshold : Real


---  
 #  MixType : [AudioMixTypes](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#audiomixtypes)

> Sets the number of channels the audio system uses when creating audio. See the enum descriptions. If your selection is different from the output device, it will be automatically translated to match the number of channels needed for output.
> ``` lang=cpp, name=Nada
> var MixType : AudioMixTypes


---  
 #  MuteAllAudio : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> When true, audio will be processed normally but will be silent.
> ``` lang=cpp, name=Nada
> var MuteAllAudio : Boolean


---  
 #  SystemVolume : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> An overall volume modifier that is applied to all audio produced by Zilch.
> ``` lang=cpp, name=Nada
> var SystemVolume : Real


---  
 #  Methods


---  
 #  AudioSettings : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function AudioSettings()
> ``` 


---  
 

 
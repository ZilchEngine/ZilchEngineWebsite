 `Component` `Sound`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](audiosettings.md#audiosettings-void)|[LatencySetting](audiosettings.md#latencysetting-zilch-engi)|[component](component.md)| |
| |[MinVolumeThreshold](audiosettings.md#minvolumethreshold-zero)| | |
| |[MixType](audiosettings.md#mixtype-zilch-engine-docu)| | |
| |[MuteAllAudio](audiosettings.md#muteallaudio-zilch-engine)| | |
| |[SystemVolume](audiosettings.md#systemvolume-zilch-engine)| | |


 #  Properties


---  
 #  LatencySetting : [AudioLatency](../enum_reference.md#audiolatency)

> Using the high latency setting can fix some audio problems (such as clicks and static) but can lead to a slight delay in the audio.
> ```TS:Nada
> var LatencySetting : AudioLatency


---  
 #  MinVolumeThreshold : [real](../nada_base_types/real.md)

> Sets the volume threshold at which sounds will be virtualized (they will continue tracking their position and all data but will not process audio). This is a floating point volume number, not decibels.
> ```TS:Nada
> var MinVolumeThreshold : Real


---  
 #  MixType : [AudioMixTypes](../enum_reference.md#audiomixtypes)

> Sets the number of channels the audio system uses when creating audio. See the enum descriptions. If your selection is different from the output device, it will be automatically translated to match the number of channels needed for output.
> ```TS:Nada
> var MixType : AudioMixTypes


---  
 #  MuteAllAudio : [boolean](../nada_base_types/boolean.md)

> When true, audio will be processed normally but will be silent.
> ```TS:Nada
> var MuteAllAudio : Boolean


---  
 #  SystemVolume : [real](../nada_base_types/real.md)

> An overall volume modifier that is applied to all audio produced by Zilch.
> ```TS:Nada
> var SystemVolume : Real


---  
 #  Methods


---  
 #  AudioSettings : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function AudioSettings()
> ``` 


---  
 

 
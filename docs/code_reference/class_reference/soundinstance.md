 `Sound`

(NOTE) The object associated with a currently playing sound.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[InterpolateDecibels](soundinstance.md#interpolatedecibels-void)|[CustomEventTime](soundinstance.md#customeventtime-zilch-eng)|[referencecountedeventobject](referencecountedeventobject.md)| |
|[InterpolatePitch](soundinstance.md#interpolatepitch-void)|[Decibels](soundinstance.md#decibels-zilch-engine-doc)| | |
|[InterpolateSemitones](soundinstance.md#interpolatesemitones-voi)|[EndTime](soundinstance.md#endtime-zilch-engine-docu)| | |
|[InterpolateVolume](soundinstance.md#interpolatevolume-void)|[FileLength](soundinstance.md#filelength-zilch-engine-d)| | |
|[Stop](soundinstance.md#stop-void)|[IsPlaying](soundinstance.md#isplaying-zilch-engine-do)| | |
| |[LoopEndTime](soundinstance.md#loopendtime-zilch-engine)| | |
| |[Looping](soundinstance.md#looping-zilch-engine-docu)| | |
| |[LoopStartTime](soundinstance.md#loopstarttime-zilch-engin)| | |
| |[Paused](soundinstance.md#paused-zilch-engine-docum)| | |
| |[Pitch](soundinstance.md#pitch-zilch-engine-docume)| | |
| |[Semitones](soundinstance.md#semitones-zilch-engine-do)| | |
| |[SoundName](soundinstance.md#soundname-zilch-engine-do)| | |
| |[SoundNode](soundinstance.md#soundnode-zilch-engine-do)| | |
| |[Time](soundinstance.md#time-zilch-engine-documen)| | |
| |[Volume](soundinstance.md#volume-zilch-engine-docum)| | |


 #  Properties


---  
 #  CustomEventTime : [real](../nada_base_types/real.md)

> The time (in seconds from the beginning of the file) to get a MusicCustomTime event.
> ```TS:Nada
> var CustomEventTime : Real


---  
 #  Decibels : [real](../nada_base_types/real.md)

> The volume adjustment (in decibels) of the SoundInstance, initially set by the SoundCue's Decibels property. A value of 0 does nothing, 6 will double the sound's volume, -6 will halve it. The Decibels property is linked to the Volume property (changing one will change the other).
> ```TS:Nada
> var Decibels : Real


---  
 #  EndTime : [real](../nada_base_types/real.md)

> The time in seconds from the beginning of the file that the instance will stop.
> ```TS:Nada
> var EndTime : Real


---  
 #  FileLength : [real](../nada_base_types/real.md)

 `read-only`

> The length of the entire audio file, in seconds.
> ```TS:Nada
> var FileLength : Real


---  
 #  IsPlaying : [boolean](../nada_base_types/boolean.md)

 `read-only`

> This Property will be true while the SoundInstance is playing, then will become false when its sound has stopped.
> ```TS:Nada
> var IsPlaying : Boolean


---  
 #  LoopEndTime : [real](../nada_base_types/real.md)

> The time in seconds from the beginning of the file that the instance will stop and jump back when looping.
> ```TS:Nada
> var LoopEndTime : Real


---  
 #  Looping : [boolean](../nada_base_types/boolean.md)

> When this Property is true the SoundInstance will loop indefinitely. If changed to false while a SoundInstance is looping the SoundInstance will continue playing to its EndTime and then stop.
> ```TS:Nada
> var Looping : Boolean


---  
 #  LoopStartTime : [real](../nada_base_types/real.md)

> The time in seconds from the beginning of the file that the instance will jump back to when it loops.
> ```TS:Nada
> var LoopStartTime : Real


---  
 #  Paused : [boolean](../nada_base_types/boolean.md)

> Setting this Property to true will pause a currently playing SoundInstance. Setting it to false will resume playback.
> ```TS:Nada
> var Paused : Boolean


---  
 #  Pitch : [real](../nada_base_types/real.md)

> The pitch adjustment of the SoundInstance, initially set by the SoundCue's Pitch property. A value of 0 will do nothing, 1 will raise the pitch by an octave and speed up the sound,.
> ```TS:Nada
> var Pitch : Real


---  
 #  Semitones : [real](../nada_base_types/real.md)

> The pitch adjustment, in semitones (or half-steps), of the SoundInstance, initially set by the SoundCue's Semitones property. A value of 0 will do nothing, 12 will raise the pitch by an octave and speed up the sound, and -12 will lower the sound by an octave and slow it down. The Semitones property is linked to the Pitch property (changing one will change the other).
> ```TS:Nada
> var Semitones : Real


---  
 #  SoundName : [string](../nada_base_types/string.md)

 `read-only`

> The name of the Sound being played by this SoundInstance.
> ```TS:Nada
> var SoundName : String


---  
 #  SoundNode : [soundnode](soundnode.md)

 `read-only`

> The SoundNode associated with this SoundInstance.
> ```TS:Nada
> var SoundNode : SoundNode


---  
 #  Time : [real](../nada_base_types/real.md)

> This property tells you to the current playback position, in seconds from the beginning of the file, and allows you to tell the instance to change its playback position to a different time. Be aware that the time will not be precisely accurate. If the Sound resource used to play the SoundInstance has Streamed selected, you cannot set the playback position.
> ```TS:Nada
> var Time : Real


---  
 #  Volume : [real](../nada_base_types/real.md)

> The volume adjustment of the SoundInstance, initially set by the SoundCue's Volume property. A value of 1 does nothing, 2 will double the sound's volume, 0.5 will halve it. The Volume property is linked to the Decibels property (changing one will change the other).
> ```TS:Nada
> var Volume : Real


---  
 #  Methods


---  
 #  InterpolateDecibels : Void

> Interpolates the SoundInstance's Decibels property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |decibels|[real](../nada_base_types/real.md)| |
> |interpolationTime|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function InterpolateDecibels(decibels : Real, interpolationTime : Real)
> ``` 


---  
 #  InterpolatePitch : Void

> Interpolates the SoundInstance's Pitch property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |pitch|[real](../nada_base_types/real.md)| |
> |interpolationTime|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function InterpolatePitch(pitch : Real, interpolationTime : Real)
> ``` 


---  
 #  InterpolateSemitones : Void

> Interpolates the SoundInstance's Semitones property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |pitchSemitones|[real](../nada_base_types/real.md)| |
> |interpolationTime|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function InterpolateSemitones(pitchSemitones : Real, interpolationTime : Real)
> ``` 


---  
 #  InterpolateVolume : Void

> Interpolates the SoundInstance's Volume property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |volume|[real](../nada_base_types/real.md)| |
> |interpolationTime|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function InterpolateVolume(volume : Real, interpolationTime : Real)
> ``` 


---  
 #  Stop : Void

> Stops the playback of this SoundInstance. It cannot be re-started.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Stop()
> ``` 


---  
 

 
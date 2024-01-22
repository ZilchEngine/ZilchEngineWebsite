 `Sound`

(NOTE) Stores Sounds and associated properties to be used by a SoundCue.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Preview](soundentry.md#preview-void)|[CrossFadeLoopTail](soundentry.md#crossfadelooptail-zilch-e)|Object| |
|[StopPreview](soundentry.md#stoppreview-void)|[EndTime](soundentry.md#endtime-zilch-engine-docu)| | |
| |[LoopEndTime](soundentry.md#loopendtime-zilch-engine)| | |
| |[LoopStartTime](soundentry.md#loopstarttime-zilch-engin)| | |
| |[LoopTailLength](soundentry.md#looptaillength-zilch-engi)| | |
| |[Sound](soundentry.md#sound-zilch-engine-docume)| | |
| |[StartTime](soundentry.md#starttime-zilch-engine-do)| | |
| |[Weight](soundentry.md#weight-zilch-engine-docum)| | |


 #  Properties


---  
 #  CrossFadeLoopTail : [boolean](../nada_base_types/boolean.md)

> If false, the loop tail will be added to the audio and will fade out over the specified time. If true, the audio will be cross-faded, so the beginning of the loop will fade in as the tail fades out.
> ```TS:Nada
> var CrossFadeLoopTail : Boolean


---  
 #  EndTime : [real](../nada_base_types/real.md)

> The time (in seconds) at which the Sound will stop playing. Defaults to the length of the audio file. Cannot be smaller than the StartTime.
> ```TS:Nada
> var EndTime : Real


---  
 #  LoopEndTime : [real](../nada_base_types/real.md)

> The time (in seconds) from the beginning of the audio file at which a looping SoundInstance jumps back to the LoopStartTime. If it stops looping while playing it will continue to the EndTime and then stop. Cannot be smaller than the LoopStartTime.
> ```TS:Nada
> var LoopEndTime : Real


---  
 #  LoopStartTime : [real](../nada_base_types/real.md)

> The time (in seconds) from the beginning of the audio file that a looping SoundInstance will jump back to after it reaches the LoopEndTime. The Sound will still start at the StartTime when it is played, but after it begins looping it will start at the LoopStartTime. Cannot be larger than the LoopEndTime.
> ```TS:Nada
> var LoopStartTime : Real


---  
 #  LoopTailLength : [real](../nada_base_types/real.md)

> The length (in seconds) of the tail, from the LoopEndTime, which will continue to play after the Sound jumps back to the LoopStartTime. The loop tail will fade out smoothly.
> ```TS:Nada
> var LoopTailLength : Real


---  
 #  Sound : [sound](sound.md)

> The Sound resource that will be played by this SoundEntry.
> ```TS:Nada
> var Sound : Sound


---  
 #  StartTime : [real](../nada_base_types/real.md)

> The time (in seconds) at which the Sound will start playing. A value of 0 will start the Sound at the beginning of the audio file. Cannot be larger than the EndTime.
> ```TS:Nada
> var StartTime : Real


---  
 #  Weight : [real](../nada_base_types/real.md)

> The weighted randomization value for this particular SoundEntry to be chosen to play. The values of all SoundEntries are considered: two SoundEntries with weights of 1 and 1 will each play 50 percent of the time, as will weights of 10 and 10.
> ```TS:Nada
> var Weight : Real


---  
 #  Methods


---  
 #  Preview : Void

> Preview this sound with no SoundCue settings.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Preview()
> ``` 


---  
 #  StopPreview : Void

> Stop previewing this sound.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function StopPreview()
> ``` 


---  
 

 
 `Component` `Sound`



(NOTE) Sound functionality associated with a Space.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[InterpolateDecibels](soundspace.md#interpolatedecibels-void)|[Decibels](soundspace.md#decibels-zilch-engine-doc)|[component](component.md)| |
|[InterpolatePitch](soundspace.md#interpolatepitch-void)|[InputNode](soundspace.md#inputnode-zilch-engine-do)| | |
|[InterpolateSemitones](soundspace.md#interpolatesemitones-voi)|[MuteAudio](soundspace.md#muteaudio-zilch-engine-do)| | |
|[InterpolateVolume](soundspace.md#interpolatevolume-void)|[OutputNode](soundspace.md#outputnode-zilch-engine-d)| | |
|[PlayCue](soundspace.md#playcue-zilch-engine-docu)|[Paused](soundspace.md#paused-zilch-engine-docum)| | |
|[PlayCuePaused](soundspace.md#playcuepaused-zilch-engin)|[PauseWithTimeSpace](soundspace.md#pausewithtimespace-zero)| | |
|[Constructor](soundspace.md#soundspace-void)|[Pitch](soundspace.md#pitch-zilch-engine-docume)| | |
| |[PitchWithTimeSpace](soundspace.md#pitchwithtimespace-zero)| | |
| |[Semitones](soundspace.md#semitones-zilch-engine-do)| | |
| |[SoundNodeInput](soundspace.md#soundnodeinput-zilch-engi)| | |
| |[SoundNodeOutput](soundspace.md#soundnodeoutput-zilch-eng)| | |
| |[Volume](soundspace.md#volume-zilch-engine-docum)| | |


 #  Properties


---  
 #  Decibels : [real](../nada_base_types/real.md)

> The volume adjustment, in decibels, applied to all sounds in the space. A value of 0 does nothing, 6 will double the sound's volume, -6 will halve it.
> ```TS:Nada
> var Decibels : Real


---  
 #  InputNode : [soundnode](soundnode.md)

 `read-only`

> DEPRECATED The SoundNodeInput property should be used instead.
> ```TS:Nada
> var InputNode : SoundNode


---  
 #  MuteAudio : [boolean](../nada_base_types/boolean.md)

> Silences all audio output from this space but processes audio normally.
> ```TS:Nada
> var MuteAudio : Boolean


---  
 #  OutputNode : [soundnode](soundnode.md)

 `read-only`

> DEPRECATED The SoundNodeOutput property should be used instead.
> ```TS:Nada
> var OutputNode : SoundNode


---  
 #  Paused : [boolean](../nada_base_types/boolean.md)

> Setting this Property to true will pause all audio in the space. Setting it to false will resume all audio.
> ```TS:Nada
> var Paused : Boolean


---  
 #  PauseWithTimeSpace : [boolean](../nada_base_types/boolean.md)

> If true, the audio of the space will pause when the space is paused.
> ```TS:Nada
> var PauseWithTimeSpace : Boolean


---  
 #  Pitch : [real](../nada_base_types/real.md)

> The pitch adjustment applied to all sounds in the space. A value of 0 will do nothing, 1 will raise the pitch by an octave and speed up the sound, -1 will lower the sound by an octave and slow it down.
> ```TS:Nada
> var Pitch : Real


---  
 #  PitchWithTimeSpace : [boolean](../nada_base_types/boolean.md)

> If true, the audio in the SoundSpace will be pitched according to the TimeScale of the Space(if time slows down the audio will slow down and lower in pitch, if it speeds up the audio will speed up and raise in pitch).
> ```TS:Nada
> var PitchWithTimeSpace : Boolean


---  
 #  Semitones : [real](../nada_base_types/real.md)

> The pitch adjustment, in semitones (or half-steps), applied to all sounds in the space. A value of 0 will do nothing, 12 will raise the pitch by an octave and speed up the sound,.
> ```TS:Nada
> var Semitones : Real


---  
 #  SoundNodeInput : [soundnode](soundnode.md)

 `read-only`

> The SoundNode which is the ultimate output of all sounds in this space.
> ```TS:Nada
> var SoundNodeInput : SoundNode


---  
 #  SoundNodeOutput : [soundnode](soundnode.md)

 `read-only`

> The SoundNode which can be used to attach other nodes which should process all audio in the SoundSpace.
> ```TS:Nada
> var SoundNodeOutput : SoundNode


---  
 #  Volume : [real](../nada_base_types/real.md)

> The volume adjustment applied to all sounds in the space. A value of 1 does nothing, 2 will double the volume, 0.5 will halve it.
> ```TS:Nada
> var Volume : Real


---  
 #  Methods


---  
 #  InterpolateDecibels : Void

> Interpolates the SoundSpace's Decibels property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |decibels|[real](../nada_base_types/real.md)| |
> |interpolationTime|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function InterpolateDecibels(decibels : Real, interpolationTime : Real)
> ``` 


---  
 #  InterpolatePitch : Void

> Interpolates the SoundSpace's Pitch property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |pitch|[real](../nada_base_types/real.md)| |
> |time|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function InterpolatePitch(pitch : Real, time : Real)
> ``` 


---  
 #  InterpolateSemitones : Void

> Interpolates the SoundSpace's Semitones property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |pitch|[real](../nada_base_types/real.md)| |
> |time|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function InterpolateSemitones(pitch : Real, time : Real)
> ``` 


---  
 #  InterpolateVolume : Void

> Interpolates the SoundSpace's Volume property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |value|[real](../nada_base_types/real.md)| |
> |interpolationTime|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function InterpolateVolume(value : Real, interpolationTime : Real)
> ``` 


---  
 #  PlayCue : [soundinstance](soundinstance.md)

> Plays the passed-in SoundCue non-positionally and returns the resulting SoundInstance.
> |Name|Type|Description|
> |---|---|---|
> |cue|[soundcue](soundcue.md)| |
> ```TS:Nada
> function PlayCue(cue : SoundCue) : SoundInstance
> ``` 


---  
 #  PlayCuePaused : [soundinstance](soundinstance.md)

> Plays the passed-in SoundCue non-positionally and returns the resulting SoundInstance, which starts off paused.
> |Name|Type|Description|
> |---|---|---|
> |cue|[soundcue](soundcue.md)| |
> ```TS:Nada
> function PlayCuePaused(cue : SoundCue) : SoundInstance
> ``` 


---  
 #  SoundSpace : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function SoundSpace()
> ``` 


---  
 

 
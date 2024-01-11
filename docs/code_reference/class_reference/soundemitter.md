 `Component` `Sound`



(NOTE) Allows 3D positioning of sounds relative to SoundListeners.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ InterpolateDecibels](soundemitter.md#interpolatedecibels-void)|[ Attenuator](soundemitter.md#attenuator-zilch-engine-d)|[component](component.md)| |
|[ InterpolatePitch](soundemitter.md#interpolatepitch-void)|[ Decibels](soundemitter.md#decibels-zilch-engine-doc)| | |
|[ InterpolateSemitones](soundemitter.md#interpolatesemitones-voi)|[ Directional](soundemitter.md#directional-zilch-engine)| | |
|[ InterpolateVolume](soundemitter.md#interpolatevolume-void)|[ EmitAngle](soundemitter.md#emitangle-zilch-engine-do)| | |
|[ PlayCue](soundemitter.md#playcue-zilch-engine-docu)|[ InputNode](soundemitter.md#inputnode-zilch-engine-do)| | |
|[ PlayCuePaused](soundemitter.md#playcuepaused-zilch-engin)|[ IsPlaying](soundemitter.md#isplaying-zilch-engine-do)| | |
|[ Constructor](soundemitter.md#soundemitter-void)|[ OutputNode](soundemitter.md#outputnode-zilch-engine-d)| | |
| |[ Paused](soundemitter.md#paused-zilch-engine-docum)| | |
| |[ Pitch](soundemitter.md#pitch-zilch-engine-docume)| | |
| |[ RearVolume](soundemitter.md#rearvolume-zilch-engine-d)| | |
| |[ Semitones](soundemitter.md#semitones-zilch-engine-do)| | |
| |[ SoundNodeInput](soundemitter.md#soundnodeinput-zilch-engi)| | |
| |[ SoundNodeOutput](soundemitter.md#soundnodeoutput-zilch-eng)| | |
| |[ Volume](soundemitter.md#volume-zilch-engine-docum)| | |


 #  Properties


---  
 #  Attenuator : [soundattenuator](soundattenuator.md)

> If a SoundAttenuator resource other than DefaultNoAttenuation is selected it will be applied to SoundCues without their own SoundAttenuator resource. If a SoundCue has attenuation settings those will always be used. If neither has settings, the sound will not be attenuated.
> ``` lang=cpp, name=Nada
> var Attenuator : SoundAttenuator


---  
 #  Decibels : [real](../nada_base_types/real.md)

> The volume adjustment, in decibels, applied to all sounds played through this SoundEmitter. A value of 0 does nothing, 6 will double the volume, -6 will halve it. The Decibels property is linked to the Volume property (changing one will change the other).
> ``` lang=cpp, name=Nada
> var Decibels : Real


---  
 #  Directional : [boolean](../nada_base_types/boolean.md)

> When true, the audio output of the SoundEmitter will be limited by the EmitAngle, so that sound in front of the object will be louder than sound behind it. Within the EmitAngle the sound will be at full volume. The volume interpolates logarithmically until it reaches the RearVolume value directly behind the object.
> ``` lang=cpp, name=Nada
> var Directional : Boolean


---  
 #  EmitAngle : [real](../nada_base_types/real.md)

> The angle of full volume sound for a directional SoundEmitter, from 1 to 360. An angle of 90, for example, will be centered at the object's front, extending 45 degrees to the left and right.
> ``` lang=cpp, name=Nada
> var EmitAngle : Real


---  
 #  InputNode : [soundnode](soundnode.md)

 `read-only`

> DEPRECATED The SoundNodeInput property should be used instead.
> ``` lang=cpp, name=Nada
> var InputNode : SoundNode


---  
 #  IsPlaying : [boolean](../nada_base_types/boolean.md)

 `read-only`

> This property will be true if there are SoundInstances currently associated with this SoundEmitter, even if they are paused or otherwise not audible.
> ``` lang=cpp, name=Nada
> var IsPlaying : Boolean


---  
 #  OutputNode : [soundnode](soundnode.md)

 `read-only`

> DEPRECATED The SoundNodeOutput property should be used instead.
> ``` lang=cpp, name=Nada
> var OutputNode : SoundNode


---  
 #  Paused : [boolean](../nada_base_types/boolean.md)

> Setting this property to true pauses all sounds currently playing through the SoundEmitter. Setting it to false will resume playback.
> ``` lang=cpp, name=Nada
> var Paused : Boolean


---  
 #  Pitch : [real](../nada_base_types/real.md)

> This property affects both the pitch and speed of all sounds played through this SoundEmitter. A value of 0 will do nothing, 1 will raise the pitch by an octave and speed up the sound, -1 will lower the sound by an octave and slow it down. The Pitch property is linked to the Semitones property (changing one will change the other).
> ``` lang=cpp, name=Nada
> var Pitch : Real


---  
 #  RearVolume : [real](../nada_base_types/real.md)

> The volume of sound heard directly behind a directional SoundEmitter. It will only reach this value in a small area, since volume is interpolated from the edge of the EmitAngle. To make the volume as quiet as possible behind the object, use a small EmitAngle.
> ``` lang=cpp, name=Nada
> var RearVolume : Real


---  
 #  Semitones : [real](../nada_base_types/real.md)

> This property, specified in semitones (or half-steps), affects both the pitch and speed of all sounds played through this SoundEmitter.. A value of 0 will do nothing, 12 will raise the pitch by an octave and speed up the sound, -12 will lower the sound by an octave and slow it down. The Semitones property is linked to the Pitch property (changing one will change the other).
> ``` lang=cpp, name=Nada
> var Semitones : Real


---  
 #  SoundNodeInput : [soundnode](soundnode.md)

 `read-only`

> The SoundNode to use for attaching other nodes to the input of the SoundEmitter.
> ``` lang=cpp, name=Nada
> var SoundNodeInput : SoundNode


---  
 #  SoundNodeOutput : [soundnode](soundnode.md)

 `read-only`

> The SoundNode to use for attaching other nodes to the output of the SoundEmitter.
> ``` lang=cpp, name=Nada
> var SoundNodeOutput : SoundNode


---  
 #  Volume : [real](../nada_base_types/real.md)

> The volume adjustment applied to all sounds played through this SoundEmitter. A value of 1 does nothing, 2 will double the volume, 0.5 will halve it. The Volume property is linked to the Decibels property (changing one will change the other).
> ``` lang=cpp, name=Nada
> var Volume : Real


---  
 #  Methods


---  
 #  InterpolateDecibels : Void

> Interpolates the Decibels property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |decibels|[real](../nada_base_types/real.md)| |
> |interpolationTime|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function InterpolateDecibels(decibels : Real, interpolationTime : Real)
> ``` 


---  
 #  InterpolatePitch : Void

> Interpolates the Pitch property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |pitch|[real](../nada_base_types/real.md)| |
> |interpolationTime|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function InterpolatePitch(pitch : Real, interpolationTime : Real)
> ``` 


---  
 #  InterpolateSemitones : Void

> Interpolates the Semitones property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |pitch|[real](../nada_base_types/real.md)| |
> |interpolationTime|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function InterpolateSemitones(pitch : Real, interpolationTime : Real)
> ``` 


---  
 #  InterpolateVolume : Void

> Interpolates the Volume property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |volume|[real](../nada_base_types/real.md)| |
> |interpolationTime|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function InterpolateVolume(volume : Real, interpolationTime : Real)
> ``` 


---  
 #  PlayCue : [soundinstance](soundinstance.md)

> Plays the SoundCue passed into the function and returns the resulting SoundInstance.
> |Name|Type|Description|
> |---|---|---|
> |cue|[soundcue](soundcue.md)| |
> ``` lang=cpp, name=Nada
> function PlayCue(cue : SoundCue) : SoundInstance
> ``` 


---  
 #  PlayCuePaused : [soundinstance](soundinstance.md)

> Plays the SoundCue passed into the function and returns the resulting SoundInstance, which starts off paused.
> |Name|Type|Description|
> |---|---|---|
> |cue|[soundcue](soundcue.md)| |
> ``` lang=cpp, name=Nada
> function PlayCuePaused(cue : SoundCue) : SoundInstance
> ``` 


---  
 #  SoundEmitter : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function SoundEmitter()
> ``` 


---  
 

 
 `Resource` `Sound`



(NOTE) Controls settings on all tagged SoundInstances.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[EQSetAllBands](soundtag.md#eqsetallbands-void)|[CompressorAttack](soundtag.md#compressorattack-zilch-en)|[dataresource](dataresource.md)| |
|[InterpolateDecibels](soundtag.md#interpolatedecibels-void)|[CompressorKneeWidth](soundtag.md#compressorkneewidth-zero)| | |
|[InterpolateVolume](soundtag.md#interpolatevolume-void)|[CompressorRatio](soundtag.md#compressorratio-zilch-eng)| | |
|[StopSounds](soundtag.md#stopsounds-void)|[CompressorRelease](soundtag.md#compressorrelease-zilch-e)| | |
|[TagSound](soundtag.md#tagsound-void)|[CompressorThreshold](soundtag.md#compressorthreshold-zero)| | |
|[UnTagSound](soundtag.md#untagsound-void)|[Decibels](soundtag.md#decibels-zilch-engine-doc)| | |
| |[EQBand1Gain](soundtag.md#eqband1gain-zilch-engine)| | |
| |[EQBand2Gain](soundtag.md#eqband2gain-zilch-engine)| | |
| |[EQBand3Gain](soundtag.md#eqband3gain-zilch-engine)| | |
| |[EQHighPassGain](soundtag.md#eqhighpassgain-zilch-engi)| | |
| |[EQLowPassGain](soundtag.md#eqlowpassgain-zilch-engin)| | |
| |[InstanceCount](soundtag.md#instancecount-zilch-engin)| | |
| |[InstanceLimit](soundtag.md#instancelimit-zilch-engin)| | |
| |[Instances](soundtag.md#instances-zilch-engine-do)| | |
| |[Paused](soundtag.md#paused-zilch-engine-docum)| | |
| |[TagForDucking](soundtag.md#tagforducking-zilch-engin)| | |
| |[UseCompressor](soundtag.md#usecompressor-zilch-engin)| | |
| |[UseEqualizer](soundtag.md#useequalizer-zilch-engine)| | |
| |[Volume](soundtag.md#volume-zilch-engine-docum)| | |


 #  Properties


---  
 #  CompressorAttack : [real](../nada_base_types/real.md)

> The time, in milliseconds, for the filter to ramp to full effect after the input reaches the threshold.
> ```TS:Nada
> var CompressorAttack : Real


---  
 #  CompressorKneeWidth : [real](../nada_base_types/real.md)

> The knee width of the filter, in decibels.
> ```TS:Nada
> var CompressorKneeWidth : Real


---  
 #  CompressorRatio : [real](../nada_base_types/real.md)

> The ratio of the compression applied by the filter.
> ```TS:Nada
> var CompressorRatio : Real


---  
 #  CompressorRelease : [real](../nada_base_types/real.md)

> The time, in milliseconds, for the filter to ramp from full effect to off after the input drops below the threshold.
> ```TS:Nada
> var CompressorRelease : Real


---  
 #  CompressorThreshold : [real](../nada_base_types/real.md)

> The threshold, in decibels, at which the volume is affected by the filter.
> ```TS:Nada
> var CompressorThreshold : Real


---  
 #  Decibels : [real](../nada_base_types/real.md)

> The volume adjustment, in decibels, applied to all tagged instances.
> ```TS:Nada
> var Decibels : Real


---  
 #  EQBand1Gain : [real](../nada_base_types/real.md)

> The volume adjustment applied to frequencies within the band centered at 150 Hz. Positive values will boost these frequencies while negative values will reduce them.
> ```TS:Nada
> var EQBand1Gain : Real


---  
 #  EQBand2Gain : [real](../nada_base_types/real.md)

> The volume adjustment applied to frequencies within the band centered at 600 Hz. Positive values will boost these frequencies while negative values will reduce them.
> ```TS:Nada
> var EQBand2Gain : Real


---  
 #  EQBand3Gain : [real](../nada_base_types/real.md)

> The volume adjustment applied to frequencies within the band centered at 2500 Hz. Positive values will boost these frequencies while negative values will reduce them.
> ```TS:Nada
> var EQBand3Gain : Real


---  
 #  EQHighPassGain : [real](../nada_base_types/real.md)

> The volume adjustment applied to frequencies above 5000 Hz. Positive values will boost these frequencies while negative values will reduce them.
> ```TS:Nada
> var EQHighPassGain : Real


---  
 #  EQLowPassGain : [real](../nada_base_types/real.md)

> The volume adjustment applied to frequencies below 80 Hz. Positive values will boost these frequencies while negative values will reduce them.
> ```TS:Nada
> var EQLowPassGain : Real


---  
 #  InstanceCount : [integer](../nada_base_types/integer.md)

 `read-only`

> The number of SoundInstances currently associated with this SoundTag.
> ```TS:Nada
> var InstanceCount : Integer


---  
 #  InstanceLimit : [real](../nada_base_types/real.md)

> If this value is greater than zero, SoundCues with this SoundTag will only play if the number of tagged SoundInstances is less than this number.
> ```TS:Nada
> var InstanceLimit : Real


---  
 #  Instances : [soundinstancerange](soundinstancerange.md)

 `read-only`

> This allows you to get all currently tagged SoundInstances. Using a foreach loop, you can access any SoundInstance functionality on each of the tagged instances.
> ```TS:Nada
> var Instances : SoundInstanceRange


---  
 #  Paused : [boolean](../nada_base_types/boolean.md)

> Setting this property to true will pause all tagged instances. Setting it to false will resume playback.
> ```TS:Nada
> var Paused : Boolean


---  
 #  TagForDucking : [soundtag](soundtag.md)

> If this property is not null, the selected SoundTag will be used to trigger this SoundTag's compressor.
> ```TS:Nada
> var TagForDucking : SoundTag


---  
 #  UseCompressor : [boolean](../nada_base_types/boolean.md)

> If true, the SoundTag's compressor settings will be applied to the tagged SoundInstances.
> ```TS:Nada
> var UseCompressor : Boolean


---  
 #  UseEqualizer : [boolean](../nada_base_types/boolean.md)

> If true, the SoundTag's equalizer settings will be applied to the tagged SoundInstances.
> ```TS:Nada
> var UseEqualizer : Boolean


---  
 #  Volume : [real](../nada_base_types/real.md)

> The volume adjustment applied to all tagged instances.
> ```TS:Nada
> var Volume : Real


---  
 #  Methods


---  
 #  EQSetAllBands : Void

> Sets all equalizer band gain values at once. The parameters are in order from the lowest band to the highest. The last parameter is the number of seconds to interpolate the values over.
> |Name|Type|Description|
> |---|---|---|
> |lowPass|[real](../nada_base_types/real.md)| |
> |band1|[real](../nada_base_types/real.md)| |
> |band2|[real](../nada_base_types/real.md)| |
> |band3|[real](../nada_base_types/real.md)| |
> |highPass|[real](../nada_base_types/real.md)| |
> |timeToInterpolate|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function EQSetAllBands(lowPass : Real, band1 : Real, band2 : Real, band3 : Real, highPass : Real, timeToInterpolate : Real)
> ``` 


---  
 #  InterpolateDecibels : Void

> Interpolates the SoundTag's Decibels property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |decibels|[real](../nada_base_types/real.md)| |
> |interpolationTime|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function InterpolateDecibels(decibels : Real, interpolationTime : Real)
> ``` 


---  
 #  InterpolateVolume : Void

> Interpolates the SoundTag's Volume property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |value|[real](../nada_base_types/real.md)| |
> |interpolationTime|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function InterpolateVolume(value : Real, interpolationTime : Real)
> ``` 


---  
 #  StopSounds : Void

> Stops all currently tagged SoundInstances.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function StopSounds()
> ``` 


---  
 #  TagSound : Void

> Adds a new SoundInstance to this SoundTag.
> |Name|Type|Description|
> |---|---|---|
> |instance|[soundinstance](soundinstance.md)| |
> ```TS:Nada
> function TagSound(instance : SoundInstance)
> ``` 


---  
 #  UnTagSound : Void

> Removes a SoundInstance from this SoundTag.
> |Name|Type|Description|
> |---|---|---|
> |instance|[soundinstance](soundinstance.md)| |
> ```TS:Nada
> function UnTagSound(instance : SoundInstance)
> ``` 


---  
 

 
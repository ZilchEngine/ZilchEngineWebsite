 `Resource` `Sound`



(NOTE) Controls settings on all tagged SoundInstances.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ EQSetAllBands](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundtag.md#eqsetallbands-void)|[ CompressorAttack](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundtag.md#compressorattack-zilch-en)|[dataresource](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/dataresource.md)| |
|[ InterpolateDecibels](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundtag.md#interpolatedecibels-void)|[ CompressorKneeWidth](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundtag.md#compressorkneewidth-zero)| | |
|[ InterpolateVolume](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundtag.md#interpolatevolume-void)|[ CompressorRatio](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundtag.md#compressorratio-zilch-eng)| | |
|[ StopSounds](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundtag.md#stopsounds-void)|[ CompressorRelease](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundtag.md#compressorrelease-zilch-e)| | |
|[ TagSound](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundtag.md#tagsound-void)|[ CompressorThreshold](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundtag.md#compressorthreshold-zero)| | |
|[ UnTagSound](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundtag.md#untagsound-void)|[ Decibels](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundtag.md#decibels-zilch-engine-doc)| | |
| |[ EQBand1Gain](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundtag.md#eqband1gain-zilch-engine)| | |
| |[ EQBand2Gain](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundtag.md#eqband2gain-zilch-engine)| | |
| |[ EQBand3Gain](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundtag.md#eqband3gain-zilch-engine)| | |
| |[ EQHighPassGain](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundtag.md#eqhighpassgain-zilch-engi)| | |
| |[ EQLowPassGain](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundtag.md#eqlowpassgain-zilch-engin)| | |
| |[ InstanceCount](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundtag.md#instancecount-zilch-engin)| | |
| |[ InstanceLimit](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundtag.md#instancelimit-zilch-engin)| | |
| |[ Instances](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundtag.md#instances-zilch-engine-do)| | |
| |[ Paused](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundtag.md#paused-zilch-engine-docum)| | |
| |[ TagForDucking](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundtag.md#tagforducking-zilch-engin)| | |
| |[ UseCompressor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundtag.md#usecompressor-zilch-engin)| | |
| |[ UseEqualizer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundtag.md#useequalizer-zilch-engine)| | |
| |[ Volume](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundtag.md#volume-zilch-engine-docum)| | |


 #  Properties


---  
 #  CompressorAttack : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The time, in milliseconds, for the filter to ramp to full effect after the input reaches the threshold.
> ``` lang=cpp, name=Nada
> var CompressorAttack : Real


---  
 #  CompressorKneeWidth : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The knee width of the filter, in decibels.
> ``` lang=cpp, name=Nada
> var CompressorKneeWidth : Real


---  
 #  CompressorRatio : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The ratio of the compression applied by the filter.
> ``` lang=cpp, name=Nada
> var CompressorRatio : Real


---  
 #  CompressorRelease : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The time, in milliseconds, for the filter to ramp from full effect to off after the input drops below the threshold.
> ``` lang=cpp, name=Nada
> var CompressorRelease : Real


---  
 #  CompressorThreshold : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The threshold, in decibels, at which the volume is affected by the filter.
> ``` lang=cpp, name=Nada
> var CompressorThreshold : Real


---  
 #  Decibels : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The volume adjustment, in decibels, applied to all tagged instances.
> ``` lang=cpp, name=Nada
> var Decibels : Real


---  
 #  EQBand1Gain : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The volume adjustment applied to frequencies within the band centered at 150 Hz. Positive values will boost these frequencies while negative values will reduce them.
> ``` lang=cpp, name=Nada
> var EQBand1Gain : Real


---  
 #  EQBand2Gain : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The volume adjustment applied to frequencies within the band centered at 600 Hz. Positive values will boost these frequencies while negative values will reduce them.
> ``` lang=cpp, name=Nada
> var EQBand2Gain : Real


---  
 #  EQBand3Gain : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The volume adjustment applied to frequencies within the band centered at 2500 Hz. Positive values will boost these frequencies while negative values will reduce them.
> ``` lang=cpp, name=Nada
> var EQBand3Gain : Real


---  
 #  EQHighPassGain : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The volume adjustment applied to frequencies above 5000 Hz. Positive values will boost these frequencies while negative values will reduce them.
> ``` lang=cpp, name=Nada
> var EQHighPassGain : Real


---  
 #  EQLowPassGain : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The volume adjustment applied to frequencies below 80 Hz. Positive values will boost these frequencies while negative values will reduce them.
> ``` lang=cpp, name=Nada
> var EQLowPassGain : Real


---  
 #  InstanceCount : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> The number of SoundInstances currently associated with this SoundTag.
> ``` lang=cpp, name=Nada
> var InstanceCount : Integer


---  
 #  InstanceLimit : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> If this value is greater than zero, SoundCues with this SoundTag will only play if the number of tagged SoundInstances is less than this number.
> ``` lang=cpp, name=Nada
> var InstanceLimit : Real


---  
 #  Instances : [soundinstancerange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundinstancerange.md)

 `read-only`

> This allows you to get all currently tagged SoundInstances. Using a foreach loop, you can access any SoundInstance functionality on each of the tagged instances.
> ``` lang=cpp, name=Nada
> var Instances : SoundInstanceRange


---  
 #  Paused : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Setting this property to true will pause all tagged instances. Setting it to false will resume playback.
> ``` lang=cpp, name=Nada
> var Paused : Boolean


---  
 #  TagForDucking : [soundtag](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundtag.md)

> If this property is not null, the selected SoundTag will be used to trigger this SoundTag's compressor.
> ``` lang=cpp, name=Nada
> var TagForDucking : SoundTag


---  
 #  UseCompressor : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> If true, the SoundTag's compressor settings will be applied to the tagged SoundInstances.
> ``` lang=cpp, name=Nada
> var UseCompressor : Boolean


---  
 #  UseEqualizer : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> If true, the SoundTag's equalizer settings will be applied to the tagged SoundInstances.
> ``` lang=cpp, name=Nada
> var UseEqualizer : Boolean


---  
 #  Volume : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The volume adjustment applied to all tagged instances.
> ``` lang=cpp, name=Nada
> var Volume : Real


---  
 #  Methods


---  
 #  EQSetAllBands : Void

> Sets all equalizer band gain values at once. The parameters are in order from the lowest band to the highest. The last parameter is the number of seconds to interpolate the values over.
> |Name|Type|Description|
> |---|---|---|
> |lowPass|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |band1|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |band2|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |band3|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |highPass|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |timeToInterpolate|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function EQSetAllBands(lowPass : Real, band1 : Real, band2 : Real, band3 : Real, highPass : Real, timeToInterpolate : Real)
> ``` 


---  
 #  InterpolateDecibels : Void

> Interpolates the SoundTag's Decibels property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |decibels|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |interpolationTime|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function InterpolateDecibels(decibels : Real, interpolationTime : Real)
> ``` 


---  
 #  InterpolateVolume : Void

> Interpolates the SoundTag's Volume property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |value|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |interpolationTime|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function InterpolateVolume(value : Real, interpolationTime : Real)
> ``` 


---  
 #  StopSounds : Void

> Stops all currently tagged SoundInstances.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function StopSounds()
> ``` 


---  
 #  TagSound : Void

> Adds a new SoundInstance to this SoundTag.
> |Name|Type|Description|
> |---|---|---|
> |instance|[soundinstance](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundinstance.md)| |
> ``` lang=cpp, name=Nada
> function TagSound(instance : SoundInstance)
> ``` 


---  
 #  UnTagSound : Void

> Removes a SoundInstance from this SoundTag.
> |Name|Type|Description|
> |---|---|---|
> |instance|[soundinstance](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundinstance.md)| |
> ``` lang=cpp, name=Nada
> function UnTagSound(instance : SoundInstance)
> ``` 


---  
 

 
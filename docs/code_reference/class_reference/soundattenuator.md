 `Resource` `Sound`



(NOTE) Decreases a positional sound's volume as the SoundEmitter gets further away from a SoundListener.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ FalloffCurve](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundattenuator.md#falloffcurve-zilch-engine)|[dataresource](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/dataresource.md)| |
| |[ FalloffCurveType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundattenuator.md#falloffcurvetype-zilch-en)| | |
| |[ LowPassCutoffFreq](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundattenuator.md#lowpasscutofffreq-zilch-e)| | |
| |[ LowPassStartDistance](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundattenuator.md#lowpassstartdistance-zer)| | |
| |[ MinAttenuatedVolume](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundattenuator.md#minattenuatedvolume-zero)| | |
| |[ StartDistance](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundattenuator.md#startdistance-zilch-engin)| | |
| |[ StopDistance](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundattenuator.md#stopdistance-zilch-engine)| | |
| |[ UseLowPassFilter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundattenuator.md#uselowpassfilter-zilch-en)| | |


 #  Properties


---  
 #  FalloffCurve : [samplecurve](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/samplecurve.md)

> The SampleCurve resource to use as the attenuation's falloff curve. It will be normalized and stretched to fit between the StartDistance and StopDistance values.
> ``` lang=cpp, name=Nada
> var FalloffCurve : SampleCurve


---  
 #  FalloffCurveType : [FalloffCurveType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#falloffcurvetype)

> The type of curve used to reduce the sound's volume over distance. The default is a logarithmic curve which mimics the real world.
> ``` lang=cpp, name=Nada
> var FalloffCurveType : FalloffCurveType


---  
 #  LowPassCutoffFreq : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The lowest cutoff frequency of the low pass filter, reached at the StopDistance. The cutoff frequency will be interpolated logarithmically from 15000.00 (a value with very little effect on the sound) to the LowPassCutoffFreq between the LowPassStartDistance and the StopDistance.
> ``` lang=cpp, name=Nada
> var LowPassCutoffFreq : Real


---  
 #  LowPassStartDistance : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The distance at which the low pass filter begins to take effect.
> ``` lang=cpp, name=Nada
> var LowPassStartDistance : Real


---  
 #  MinAttenuatedVolume : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The lowest volume that the attenuation will reach. If set above 0, the sound will continue to be heard at all distances.
> ``` lang=cpp, name=Nada
> var MinAttenuatedVolume : Real


---  
 #  StartDistance : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The distance from a SoundListener at which the sound's volume begins attenuating. At shorter distances the volume will not be changed. Cannot be larger than the StopDistance.
> ``` lang=cpp, name=Nada
> var StartDistance : Real


---  
 #  StopDistance : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The distance at which the attenuation reaches the minimum volume. No volume changes will happen past this distance. Cannot be smaller than the StartDistance.
> ``` lang=cpp, name=Nada
> var StopDistance : Real


---  
 #  UseLowPassFilter : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> If true, a low pass filter will be applied to the sound after reaching a specified distance, mimicking the way sound is muffled with distance in real life. The filter begins at the LowPassStartDistance and interpolates its cutoff frequency logarithmically until the StopDistance. The filter will not change past the StopDistance.
> ``` lang=cpp, name=Nada
> var UseLowPassFilter : Boolean


---  
 #  Methods


---  
 

 
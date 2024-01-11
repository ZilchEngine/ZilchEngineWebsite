 `Resource` `Sound`



(NOTE) Decreases a positional sound's volume as the SoundEmitter gets further away from a SoundListener.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ FalloffCurve](soundattenuator.md#falloffcurve-zilch-engine)|[dataresource](dataresource.md)| |
| |[ FalloffCurveType](soundattenuator.md#falloffcurvetype-zilch-en)| | |
| |[ LowPassCutoffFreq](soundattenuator.md#lowpasscutofffreq-zilch-e)| | |
| |[ LowPassStartDistance](soundattenuator.md#lowpassstartdistance-zer)| | |
| |[ MinAttenuatedVolume](soundattenuator.md#minattenuatedvolume-zero)| | |
| |[ StartDistance](soundattenuator.md#startdistance-zilch-engin)| | |
| |[ StopDistance](soundattenuator.md#stopdistance-zilch-engine)| | |
| |[ UseLowPassFilter](soundattenuator.md#uselowpassfilter-zilch-en)| | |


 #  Properties


---  
 #  FalloffCurve : [samplecurve](samplecurve.md)

> The SampleCurve resource to use as the attenuation's falloff curve. It will be normalized and stretched to fit between the StartDistance and StopDistance values.
> ```TS:Nada
> var FalloffCurve : SampleCurve


---  
 #  FalloffCurveType : [FalloffCurveType](../enum_reference.md#falloffcurvetype)

> The type of curve used to reduce the sound's volume over distance. The default is a logarithmic curve which mimics the real world.
> ```TS:Nada
> var FalloffCurveType : FalloffCurveType


---  
 #  LowPassCutoffFreq : [real](../nada_base_types/real.md)

> The lowest cutoff frequency of the low pass filter, reached at the StopDistance. The cutoff frequency will be interpolated logarithmically from 15000.00 (a value with very little effect on the sound) to the LowPassCutoffFreq between the LowPassStartDistance and the StopDistance.
> ```TS:Nada
> var LowPassCutoffFreq : Real


---  
 #  LowPassStartDistance : [real](../nada_base_types/real.md)

> The distance at which the low pass filter begins to take effect.
> ```TS:Nada
> var LowPassStartDistance : Real


---  
 #  MinAttenuatedVolume : [real](../nada_base_types/real.md)

> The lowest volume that the attenuation will reach. If set above 0, the sound will continue to be heard at all distances.
> ```TS:Nada
> var MinAttenuatedVolume : Real


---  
 #  StartDistance : [real](../nada_base_types/real.md)

> The distance from a SoundListener at which the sound's volume begins attenuating. At shorter distances the volume will not be changed. Cannot be larger than the StopDistance.
> ```TS:Nada
> var StartDistance : Real


---  
 #  StopDistance : [real](../nada_base_types/real.md)

> The distance at which the attenuation reaches the minimum volume. No volume changes will happen past this distance. Cannot be smaller than the StartDistance.
> ```TS:Nada
> var StopDistance : Real


---  
 #  UseLowPassFilter : [boolean](../nada_base_types/boolean.md)

> If true, a low pass filter will be applied to the sound after reaching a specified distance, mimicking the way sound is muffled with distance in real life. The filter begins at the LowPassStartDistance and interpolates its cutoff frequency logarithmically until the StopDistance. The filter will not change past the StopDistance.
> ```TS:Nada
> var UseLowPassFilter : Boolean


---  
 #  Methods


---  
 

 
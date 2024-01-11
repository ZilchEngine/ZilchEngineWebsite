 `Sound`

(NOTE) Plays audio using the specified type of generated wave.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ InterpolateDecibels](generatedwavenode.md#interpolatedecibels-void)|[ Decibels](generatedwavenode.md#decibels-zilch-engine-doc)|[soundnode](soundnode.md)| |
|[ InterpolateVolume](generatedwavenode.md#interpolatevolume-void)|[ SquareWavePulseValue](generatedwavenode.md#squarewavepulsevalue-zer)| | |
|[ InterpolateWaveFrequency](generatedwavenode.md#interpolatewavefrequency)|[ Volume](generatedwavenode.md#volume-zilch-engine-docum)| | |
|[ Play](generatedwavenode.md#play-void)|[ WaveFrequency](generatedwavenode.md#wavefrequency-zilch-engin)| | |
|[ Stop](generatedwavenode.md#stop-void)|[ WaveType](generatedwavenode.md#wavetype-zilch-engine-doc)| | |


 #  Properties


---  
 #  Decibels : [real](../nada_base_types/real.md)

> The volume adjustment, in decibels, that will be applied to the sound when it plays. A value of 0 does not affect the sound; 6 will double the sound's volume, -6 will halve it, and -100 is effectively the same as a Volume of 0.
> ```TS:Nada
> var Decibels : Real


---  
 #  SquareWavePulseValue : [real](../nada_base_types/real.md)

> The percentage of the square wave (from 0 to 1.0) which should be up. This will have no effect if a different wave type is chosen.
> ```TS:Nada
> var SquareWavePulseValue : Real


---  
 #  Volume : [real](../nada_base_types/real.md)

> The volume adjustment that will be applied to the sound when it plays. A value of 1 does not affect the sound; 2 will double the sound's volume, 0.5 will halve it, and 0 will make the sound inaudible.
> ```TS:Nada
> var Volume : Real


---  
 #  WaveFrequency : [real](../nada_base_types/real.md)

> The frequency of the generated sound wave. This value will have no effect if the Noise type is chosen.
> ```TS:Nada
> var WaveFrequency : Real


---  
 #  WaveType : [SynthWaveType](../enum_reference.md#synthwavetype)

> The type of sound wave used to generate the audio. Possible types are Sine, Square, Saw, Triangle, and Noise (randomly generated white noise).
> ```TS:Nada
> var WaveType : SynthWaveType


---  
 #  Methods


---  
 #  InterpolateDecibels : Void

> Interpolates the Decibels property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |decibels|[real](../nada_base_types/real.md)| |
> |interpolationTime|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function InterpolateDecibels(decibels : Real, interpolationTime : Real)
> ``` 


---  
 #  InterpolateVolume : Void

> Interpolates the Volume property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |volume|[real](../nada_base_types/real.md)| |
> |interpolationTime|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function InterpolateVolume(volume : Real, interpolationTime : Real)
> ``` 


---  
 #  InterpolateWaveFrequency : Void

> Interpolates the WaveFrequency property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter. This method will have no effect if the Noise type is chosen.
> |Name|Type|Description|
> |---|---|---|
> |frequency|[real](../nada_base_types/real.md)| |
> |time|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function InterpolateWaveFrequency(frequency : Real, time : Real)
> ``` 


---  
 #  Play : Void

> Starts playing the generated audio.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Play()
> ``` 


---  
 #  Stop : Void

> Stops playing the generated audio.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Stop()
> ``` 


---  
 

 
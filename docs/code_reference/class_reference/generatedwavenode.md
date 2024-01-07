 `Sound`

(NOTE) Plays audio using the specified type of generated wave.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ InterpolateDecibels](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/generatedwavenode.md#interpolatedecibels-void)|[ Decibels](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/generatedwavenode.md#decibels-zilch-engine-doc)|[soundnode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundnode.md)| |
|[ InterpolateVolume](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/generatedwavenode.md#interpolatevolume-void)|[ SquareWavePulseValue](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/generatedwavenode.md#squarewavepulsevalue-zer)| | |
|[ InterpolateWaveFrequency](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/generatedwavenode.md#interpolatewavefrequency)|[ Volume](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/generatedwavenode.md#volume-zilch-engine-docum)| | |
|[ Play](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/generatedwavenode.md#play-void)|[ WaveFrequency](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/generatedwavenode.md#wavefrequency-zilch-engin)| | |
|[ Stop](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/generatedwavenode.md#stop-void)|[ WaveType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/generatedwavenode.md#wavetype-zilch-engine-doc)| | |


 #  Properties


---  
 #  Decibels : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The volume adjustment, in decibels, that will be applied to the sound when it plays. A value of 0 does not affect the sound; 6 will double the sound's volume, -6 will halve it, and -100 is effectively the same as a Volume of 0.
> ``` lang=cpp, name=Nada
> var Decibels : Real


---  
 #  SquareWavePulseValue : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The percentage of the square wave (from 0 to 1.0) which should be up. This will have no effect if a different wave type is chosen.
> ``` lang=cpp, name=Nada
> var SquareWavePulseValue : Real


---  
 #  Volume : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The volume adjustment that will be applied to the sound when it plays. A value of 1 does not affect the sound; 2 will double the sound's volume, 0.5 will halve it, and 0 will make the sound inaudible.
> ``` lang=cpp, name=Nada
> var Volume : Real


---  
 #  WaveFrequency : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The frequency of the generated sound wave. This value will have no effect if the Noise type is chosen.
> ``` lang=cpp, name=Nada
> var WaveFrequency : Real


---  
 #  WaveType : [SynthWaveType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#synthwavetype)

> The type of sound wave used to generate the audio. Possible types are Sine, Square, Saw, Triangle, and Noise (randomly generated white noise).
> ``` lang=cpp, name=Nada
> var WaveType : SynthWaveType


---  
 #  Methods


---  
 #  InterpolateDecibels : Void

> Interpolates the Decibels property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |decibels|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |interpolationTime|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function InterpolateDecibels(decibels : Real, interpolationTime : Real)
> ``` 


---  
 #  InterpolateVolume : Void

> Interpolates the Volume property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |volume|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |interpolationTime|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function InterpolateVolume(volume : Real, interpolationTime : Real)
> ``` 


---  
 #  InterpolateWaveFrequency : Void

> Interpolates the WaveFrequency property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter. This method will have no effect if the Noise type is chosen.
> |Name|Type|Description|
> |---|---|---|
> |frequency|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |time|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function InterpolateWaveFrequency(frequency : Real, time : Real)
> ``` 


---  
 #  Play : Void

> Starts playing the generated audio.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Play()
> ``` 


---  
 #  Stop : Void

> Stops playing the generated audio.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Stop()
> ``` 


---  
 

 
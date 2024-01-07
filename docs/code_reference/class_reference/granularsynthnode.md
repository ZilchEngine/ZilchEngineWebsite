 `Sound`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Play](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/granularsynthnode.md#play-void)|[ BufferScanRate](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/granularsynthnode.md#bufferscanrate-zilch-engi)|[soundnode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundnode.md)| |
|[ SetSound](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/granularsynthnode.md#setsound-void)|[ GrainDelay](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/granularsynthnode.md#graindelay-zilch-engine-d)| | |
|[ Stop](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/granularsynthnode.md#stop-void)|[ GrainDelayVariance](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/granularsynthnode.md#graindelayvariance-zero)| | |
| |[ GrainLength](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/granularsynthnode.md#grainlength-zilch-engine)| | |
| |[ GrainLengthVariance](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/granularsynthnode.md#grainlengthvariance-zero)| | |
| |[ GrainPanningValue](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/granularsynthnode.md#grainpanningvalue-zilch-e)| | |
| |[ GrainPanningVariance](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/granularsynthnode.md#grainpanningvariance-zer)| | |
| |[ GrainResampleRate](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/granularsynthnode.md#grainresamplerate-zilch-e)| | |
| |[ GrainResampleRateVariance](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/granularsynthnode.md#grainresampleratevarianc)| | |
| |[ GrainVolume](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/granularsynthnode.md#grainvolume-zilch-engine)| | |
| |[ GrainVolumeVariance](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/granularsynthnode.md#grainvolumevariance-zero)| | |
| |[ RandomLocationValue](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/granularsynthnode.md#randomlocationvalue-zero)| | |
| |[ WindowAttack](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/granularsynthnode.md#windowattack-zilch-engine)| | |
| |[ WindowRelease](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/granularsynthnode.md#windowrelease-zilch-engin)| | |
| |[ WindowType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/granularsynthnode.md#windowtype-zilch-engine-d)| | |


 #  Properties


---  
 #  BufferScanRate : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The rate at which the synthesizer scans the buffer as it creates grains. A value of 1.0 will move through the audio data at the same rate as it would normally be played, 0.5 will move at half speed, and -1.0 will move at normal speed backward. A value of 0.0 will make the synthesizer repeat the same audio continuously.
> ``` lang=cpp, name=Nada
> var BufferScanRate : Real


---  
 #  GrainDelay : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> The number of milliseconds to wait before playing another grain.
> ``` lang=cpp, name=Nada
> var GrainDelay : Integer


---  
 #  GrainDelayVariance : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> The variance for randomizing the grain delay, in milliseconds.
> ``` lang=cpp, name=Nada
> var GrainDelayVariance : Integer


---  
 #  GrainLength : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> The length of a grain, in milliseconds.
> ``` lang=cpp, name=Nada
> var GrainLength : Integer


---  
 #  GrainLengthVariance : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> The variance for randomizing the grain length, in milliseconds.
> ``` lang=cpp, name=Nada
> var GrainLengthVariance : Integer


---  
 #  GrainPanningValue : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The value used to pan the grains left or right. A value of 0 will be heard equally from the left and right, 1.0 will be heard only on the right, and -1.0 will be only left.
> ``` lang=cpp, name=Nada
> var GrainPanningValue : Real


---  
 #  GrainPanningVariance : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The variance for randomizing the grain panning value.
> ``` lang=cpp, name=Nada
> var GrainPanningVariance : Real


---  
 #  GrainResampleRate : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The rate at which grains resample their audio data. A value of 1.0 will play normally, 0.5 will play at half speed, and -1.0 will play at normal speed backward. Cannot be 0.
> ``` lang=cpp, name=Nada
> var GrainResampleRate : Real


---  
 #  GrainResampleRateVariance : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The variance for randomizing the grain resample rate.
> ``` lang=cpp, name=Nada
> var GrainResampleRateVariance : Real


---  
 #  GrainVolume : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The volume modifier applied to the grains.
> ``` lang=cpp, name=Nada
> var GrainVolume : Real


---  
 #  GrainVolumeVariance : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The variance for randomizing the grain volume.
> ``` lang=cpp, name=Nada
> var GrainVolumeVariance : Real


---  
 #  RandomLocationValue : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The value for controlling how many grains have randomized starting positions in the audio. A value of 0 will be completely sequential, while 1.0 will be completely random.
> ``` lang=cpp, name=Nada
> var RandomLocationValue : Real


---  
 #  WindowAttack : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> The window attack time, in milliseconds. Does not have an effect on some windows.
> ``` lang=cpp, name=Nada
> var WindowAttack : Integer


---  
 #  WindowRelease : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> The window release time, in milliseconds. Does not have an effect on some windows.
> ``` lang=cpp, name=Nada
> var WindowRelease : Integer


---  
 #  WindowType : [GranularSynthWindows](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#granularsynthwindows)

> The type of window, or volume envelope, used for each grain.
> ``` lang=cpp, name=Nada
> var WindowType : GranularSynthWindows


---  
 #  Methods


---  
 #  Play : Void

> Starts playing new grains.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Play()
> ``` 


---  
 #  SetSound : Void

> Sets the Sound resource that will be used for the grains, along with an optional start and stop time. If the stopTime is 0.0, all audio from the Sound will be used.
> |Name|Type|Description|
> |---|---|---|
> |sound|[sound](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sound.md)| |
> |startTime|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |stopTime|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function SetSound(sound : Sound, startTime : Real, stopTime : Real)
> ``` 


---  
 #  Stop : Void

> Stops playing new grains but continues to play current ones.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Stop()
> ``` 


---  
 

 
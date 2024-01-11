 `Sound`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Play](granularsynthnode.md#play-void)|[ BufferScanRate](granularsynthnode.md#bufferscanrate-zilch-engi)|[soundnode](soundnode.md)| |
|[ SetSound](granularsynthnode.md#setsound-void)|[ GrainDelay](granularsynthnode.md#graindelay-zilch-engine-d)| | |
|[ Stop](granularsynthnode.md#stop-void)|[ GrainDelayVariance](granularsynthnode.md#graindelayvariance-zero)| | |
| |[ GrainLength](granularsynthnode.md#grainlength-zilch-engine)| | |
| |[ GrainLengthVariance](granularsynthnode.md#grainlengthvariance-zero)| | |
| |[ GrainPanningValue](granularsynthnode.md#grainpanningvalue-zilch-e)| | |
| |[ GrainPanningVariance](granularsynthnode.md#grainpanningvariance-zer)| | |
| |[ GrainResampleRate](granularsynthnode.md#grainresamplerate-zilch-e)| | |
| |[ GrainResampleRateVariance](granularsynthnode.md#grainresampleratevarianc)| | |
| |[ GrainVolume](granularsynthnode.md#grainvolume-zilch-engine)| | |
| |[ GrainVolumeVariance](granularsynthnode.md#grainvolumevariance-zero)| | |
| |[ RandomLocationValue](granularsynthnode.md#randomlocationvalue-zero)| | |
| |[ WindowAttack](granularsynthnode.md#windowattack-zilch-engine)| | |
| |[ WindowRelease](granularsynthnode.md#windowrelease-zilch-engin)| | |
| |[ WindowType](granularsynthnode.md#windowtype-zilch-engine-d)| | |


 #  Properties


---  
 #  BufferScanRate : [real](../nada_base_types/real.md)

> The rate at which the synthesizer scans the buffer as it creates grains. A value of 1.0 will move through the audio data at the same rate as it would normally be played, 0.5 will move at half speed, and -1.0 will move at normal speed backward. A value of 0.0 will make the synthesizer repeat the same audio continuously.
> ```TS:Nada
> var BufferScanRate : Real


---  
 #  GrainDelay : [integer](../nada_base_types/integer.md)

> The number of milliseconds to wait before playing another grain.
> ```TS:Nada
> var GrainDelay : Integer


---  
 #  GrainDelayVariance : [integer](../nada_base_types/integer.md)

> The variance for randomizing the grain delay, in milliseconds.
> ```TS:Nada
> var GrainDelayVariance : Integer


---  
 #  GrainLength : [integer](../nada_base_types/integer.md)

> The length of a grain, in milliseconds.
> ```TS:Nada
> var GrainLength : Integer


---  
 #  GrainLengthVariance : [integer](../nada_base_types/integer.md)

> The variance for randomizing the grain length, in milliseconds.
> ```TS:Nada
> var GrainLengthVariance : Integer


---  
 #  GrainPanningValue : [real](../nada_base_types/real.md)

> The value used to pan the grains left or right. A value of 0 will be heard equally from the left and right, 1.0 will be heard only on the right, and -1.0 will be only left.
> ```TS:Nada
> var GrainPanningValue : Real


---  
 #  GrainPanningVariance : [real](../nada_base_types/real.md)

> The variance for randomizing the grain panning value.
> ```TS:Nada
> var GrainPanningVariance : Real


---  
 #  GrainResampleRate : [real](../nada_base_types/real.md)

> The rate at which grains resample their audio data. A value of 1.0 will play normally, 0.5 will play at half speed, and -1.0 will play at normal speed backward. Cannot be 0.
> ```TS:Nada
> var GrainResampleRate : Real


---  
 #  GrainResampleRateVariance : [real](../nada_base_types/real.md)

> The variance for randomizing the grain resample rate.
> ```TS:Nada
> var GrainResampleRateVariance : Real


---  
 #  GrainVolume : [real](../nada_base_types/real.md)

> The volume modifier applied to the grains.
> ```TS:Nada
> var GrainVolume : Real


---  
 #  GrainVolumeVariance : [real](../nada_base_types/real.md)

> The variance for randomizing the grain volume.
> ```TS:Nada
> var GrainVolumeVariance : Real


---  
 #  RandomLocationValue : [real](../nada_base_types/real.md)

> The value for controlling how many grains have randomized starting positions in the audio. A value of 0 will be completely sequential, while 1.0 will be completely random.
> ```TS:Nada
> var RandomLocationValue : Real


---  
 #  WindowAttack : [integer](../nada_base_types/integer.md)

> The window attack time, in milliseconds. Does not have an effect on some windows.
> ```TS:Nada
> var WindowAttack : Integer


---  
 #  WindowRelease : [integer](../nada_base_types/integer.md)

> The window release time, in milliseconds. Does not have an effect on some windows.
> ```TS:Nada
> var WindowRelease : Integer


---  
 #  WindowType : [GranularSynthWindows](../enum_reference.md#granularsynthwindows)

> The type of window, or volume envelope, used for each grain.
> ```TS:Nada
> var WindowType : GranularSynthWindows


---  
 #  Methods


---  
 #  Play : Void

> Starts playing new grains.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Play()
> ``` 


---  
 #  SetSound : Void

> Sets the Sound resource that will be used for the grains, along with an optional start and stop time. If the stopTime is 0.0, all audio from the Sound will be used.
> |Name|Type|Description|
> |---|---|---|
> |sound|[sound](sound.md)| |
> |startTime|[real](../nada_base_types/real.md)| |
> |stopTime|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function SetSound(sound : Sound, startTime : Real, stopTime : Real)
> ``` 


---  
 #  Stop : Void

> Stops playing new grains but continues to play current ones.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Stop()
> ``` 


---  
 

 
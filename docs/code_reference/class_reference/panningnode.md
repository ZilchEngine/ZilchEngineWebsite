 `Sound`

(NOTE) Changes the left and right channel volumes of its input SoundNode's audio separately.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[InterpolateLeftVolume](panningnode.md#interpolateleftvolume-vo)|[LeftVolume](panningnode.md#leftvolume-zilch-engine-d)|[soundnode](soundnode.md)| |
|[InterpolateRightVolume](panningnode.md#interpolaterightvolume-v)|[RightVolume](panningnode.md#rightvolume-zilch-engine)| | |
|[InterpolateVolumes](panningnode.md#interpolatevolumes-void)|[SumToMono](panningnode.md#sumtomono-zilch-engine-do)| | |


 #  Properties


---  
 #  LeftVolume : [real](../nada_base_types/real.md)

> The volume multiplier applied to audio in the left channel.
> ```TS:Nada
> var LeftVolume : Real


---  
 #  RightVolume : [real](../nada_base_types/real.md)

> The volume multiplier applied to audio in the right channel.
> ```TS:Nada
> var RightVolume : Real


---  
 #  SumToMono : [boolean](../nada_base_types/boolean.md)

> If this property is true, the audio will be combined into a single channel before being split between the right and left channels. If it is false and the audio has more than two channels, it will be combined into only two channels before being processed.
> ```TS:Nada
> var SumToMono : Boolean


---  
 #  Methods


---  
 #  InterpolateLeftVolume : Void

> Interpolates the LeftVolume property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |volume|[real](../nada_base_types/real.md)| |
> |time|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function InterpolateLeftVolume(volume : Real, time : Real)
> ``` 


---  
 #  InterpolateRightVolume : Void

> Interpolates the RightVolume property from its current value to the value passed in as the first parameter, over the number of seconds passed in as the second parameter.
> |Name|Type|Description|
> |---|---|---|
> |volume|[real](../nada_base_types/real.md)| |
> |time|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function InterpolateRightVolume(volume : Real, time : Real)
> ``` 


---  
 #  InterpolateVolumes : Void

> Interpolates both left and right volume properties at once. The first parameter is the value to change the LeftVolume to, the second is the RightVolume, and the third is the number of seconds to use for the interpolation.
> |Name|Type|Description|
> |---|---|---|
> |leftVolume|[real](../nada_base_types/real.md)| |
> |rightVolume|[real](../nada_base_types/real.md)| |
> |time|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function InterpolateVolumes(leftVolume : Real, rightVolume : Real, time : Real)
> ``` 


---  
 

 
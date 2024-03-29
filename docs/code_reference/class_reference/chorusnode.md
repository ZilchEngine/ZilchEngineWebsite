 `Sound`

(NOTE) Applies a chorus filter to audio generated by its input SoundNodes.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[FeedbackPercent](chorusnode.md#feedbackpercent-zilch-eng)|[soundnode](soundnode.md)| |
| |[FeedbackValue](chorusnode.md#feedbackvalue-zilch-engin)| | |
| |[MaxDelayMillisec](chorusnode.md#maxdelaymillisec-zilch-en)| | |
| |[MinDelayMillisec](chorusnode.md#mindelaymillisec-zilch-en)| | |
| |[ModulationFrequency](chorusnode.md#modulationfrequency-zero)| | |
| |[OffsetMillisec](chorusnode.md#offsetmillisec-zilch-engi)| | |


 #  Properties


---  
 #  FeedbackPercent : [real](../nada_base_types/real.md)

> DEPRECATED The FeedbackValue property should be used instead.
> ```TS:Nada
> var FeedbackPercent : Real


---  
 #  FeedbackValue : [real](../nada_base_types/real.md)

> The percentage of output (0 - 1.0) which is fed back into the filter as input.
> ```TS:Nada
> var FeedbackValue : Real


---  
 #  MaxDelayMillisec : [real](../nada_base_types/real.md)

> The maximum delay reached by the modulation. It will oscillate between the MinDelayMillisec value and this value at the frequency set by the ModulationFrequency property.
> ```TS:Nada
> var MaxDelayMillisec : Real


---  
 #  MinDelayMillisec : [real](../nada_base_types/real.md)

> The minimum delay reached by the modulation. It will oscillate between the this value and the MaxDelayMillisec value at the frequency set by the ModulationFrequency property.
> ```TS:Nada
> var MinDelayMillisec : Real


---  
 #  ModulationFrequency : [real](../nada_base_types/real.md)

> The frequency of the oscillator which varies the modulation.
> ```TS:Nada
> var ModulationFrequency : Real


---  
 #  OffsetMillisec : [real](../nada_base_types/real.md)

> The offset value of the chorus filter, in milliseconds.
> ```TS:Nada
> var OffsetMillisec : Real


---  
 #  Methods


---  
 

 
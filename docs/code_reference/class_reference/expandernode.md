 `Sound`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ AttackMillisec](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/expandernode.md#attackmillisec-zilch-engi)|[soundnode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundnode.md)| |
| |[ InputGainDecibels](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/expandernode.md#inputgaindecibels-zilch-e)| | |
| |[ KneeWidth](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/expandernode.md#kneewidth-zilch-engine-do)| | |
| |[ OutputGainDecibels](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/expandernode.md#outputgaindecibels-zero)| | |
| |[ Ratio](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/expandernode.md#ratio-zilch-engine-docume)| | |
| |[ ReleaseMillisec](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/expandernode.md#releasemillisec-zilch-eng)| | |
| |[ ThresholdDecibels](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/expandernode.md#thresholddecibels-zilch-e)| | |


 #  Properties


---  
 #  AttackMillisec : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The time for the expander to ramp to full effect after the input reaches the threshold.
> ``` lang=cpp, name=Nada
> var AttackMillisec : Real


---  
 #  InputGainDecibels : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The volume adjustment applied to the audio input, in decibels.
> ``` lang=cpp, name=Nada
> var InputGainDecibels : Real


---  
 #  KneeWidth : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The knee width of the expander, in decibels.
> ``` lang=cpp, name=Nada
> var KneeWidth : Real


---  
 #  OutputGainDecibels : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The volume adjustment applied to the expander output, in decibels.
> ``` lang=cpp, name=Nada
> var OutputGainDecibels : Real


---  
 #  Ratio : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The ratio of the volume reduction applied by the expander.
> ``` lang=cpp, name=Nada
> var Ratio : Real


---  
 #  ReleaseMillisec : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The time for the expander to ramp from full effect to off after the input goes above the threshold.
> ``` lang=cpp, name=Nada
> var ReleaseMillisec : Real


---  
 #  ThresholdDecibels : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The threshold, in decibels, at which the volume of the input is affected by the expander.
> ``` lang=cpp, name=Nada
> var ThresholdDecibels : Real


---  
 #  Methods


---  
 

 
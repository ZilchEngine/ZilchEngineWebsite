 `Sound`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AdditiveSynthNode](audio.md#additivesynthnode-zilch-e)|[ DispatchMicrophoneCompressedByteData](audio.md#dispatchmicrophonecompre)|[system](system.md)| |
|[ AddNoiseNode](audio.md#addnoisenode-zilch-engine)|[ DispatchMicrophoneUncompressedFloatData](audio.md#dispatchmicrophoneuncomp)| | |
|[ BandPassNode](audio.md#bandpassnode-zilch-engine)|[ LatencySetting](audio.md#latencysetting-zilch-engi)| | |
|[ ChorusNode](audio.md#chorusnode-zilch-engine-d)|[ MuteAllAudio](audio.md#muteallaudio-zilch-engine)| | |
|[ CompressorNode](audio.md#compressornode-zilch-engi)|[ OutputChannels](audio.md#outputchannels-zilch-engi)| | |
|[ CustomAudioNode](audio.md#customaudionode-zilch-eng)|[ PeakInputLevel](audio.md#peakinputlevel-zilch-engi)| | |
|[ DelayNode](audio.md#delaynode-zilch-engine-do)|[ PeakOutputLevel](audio.md#peakoutputlevel-zilch-eng)| | |
|[ EqualizerNode](audio.md#equalizernode-zilch-engin)|[ RMSOutputLevel](audio.md#rmsoutputlevel-zilch-engi)| | |
|[ ExpanderNode](audio.md#expandernode-zilch-engine)|[ SystemVolume](audio.md#systemvolume-zilch-engine)| | |
|[ FlangerNode](audio.md#flangernode-zilch-engine)| | | |
|[ GeneratedWaveNode](audio.md#generatedwavenode-zilch-e)| | | |
|[ GetNodeGraphInfo](audio.md#getnodegraphinfo-zilch-en)| | | |
|[ GranularSynthNode](audio.md#granularsynthnode-zilch-e)| | | |
|[ HighPassNode](audio.md#highpassnode-zilch-engine)| | | |
|[ LowPassNode](audio.md#lowpassnode-zilch-engine)| | | |
|[ MicrophoneInputNode](audio.md#microphoneinputnode-zero)| | | |
|[ ModulationNode](audio.md#modulationnode-zilch-engi)| | | |
|[ PanningNode](audio.md#panningnode-zilch-engine)| | | |
|[ PitchNode](audio.md#pitchnode-zilch-engine-do)| | | |
|[ RecordingNode](audio.md#recordingnode-zilch-engin)| | | |
|[ ReverbNode](audio.md#reverbnode-zilch-engine-d)| | | |
|[ SaveAudioNode](audio.md#saveaudionode-zilch-engin)| | | |
|[ SoundBuffer](audio.md#soundbuffer-zilch-engine)| | | |
|[ VolumeNode](audio.md#volumenode-zilch-engine-d)| | | |


 #  Properties


---  
 #  DispatchMicrophoneCompressedByteData : [boolean](../nada_base_types/boolean.md)

> 
> ```TS:Nada
> var DispatchMicrophoneCompressedByteData : Boolean


---  
 #  DispatchMicrophoneUncompressedFloatData : [boolean](../nada_base_types/boolean.md)

> 
> ```TS:Nada
> var DispatchMicrophoneUncompressedFloatData : Boolean


---  
 #  LatencySetting : [AudioLatency](../enum_reference.md#audiolatency)

> 
> ```TS:Nada
> var LatencySetting : AudioLatency


---  
 #  MuteAllAudio : [boolean](../nada_base_types/boolean.md)

> 
> ```TS:Nada
> var MuteAllAudio : Boolean


---  
 #  OutputChannels : [integer](../nada_base_types/integer.md)

 `read-only`

> 
> ```TS:Nada
> var OutputChannels : Integer


---  
 #  PeakInputLevel : [real](../nada_base_types/real.md)

 `read-only`

> 
> ```TS:Nada
> var PeakInputLevel : Real


---  
 #  PeakOutputLevel : [real](../nada_base_types/real.md)

 `read-only`

> 
> ```TS:Nada
> var PeakOutputLevel : Real


---  
 #  RMSOutputLevel : [real](../nada_base_types/real.md)

 `read-only`

> 
> ```TS:Nada
> var RMSOutputLevel : Real


---  
 #  SystemVolume : [real](../nada_base_types/real.md)

> 
> ```TS:Nada
> var SystemVolume : Real


---  
 #  Methods


---  
 #  AdditiveSynthNode : [additivesynthnode](additivesynthnode.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function AdditiveSynthNode() : AdditiveSynthNode
> ``` 


---  
 #  AddNoiseNode : [addnoisenode](addnoisenode.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function AddNoiseNode() : AddNoiseNode
> ``` 


---  
 #  BandPassNode : [bandpassnode](bandpassnode.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function BandPassNode() : BandPassNode
> ``` 


---  
 #  ChorusNode : [chorusnode](chorusnode.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ChorusNode() : ChorusNode
> ``` 


---  
 #  CompressorNode : [compressornode](compressornode.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function CompressorNode() : CompressorNode
> ``` 


---  
 #  CustomAudioNode : [customaudionode](customaudionode.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function CustomAudioNode() : CustomAudioNode
> ``` 


---  
 #  DelayNode : [delaynode](delaynode.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function DelayNode() : DelayNode
> ``` 


---  
 #  EqualizerNode : [equalizernode](equalizernode.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function EqualizerNode() : EqualizerNode
> ``` 


---  
 #  ExpanderNode : [expandernode](expandernode.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ExpanderNode() : ExpanderNode
> ``` 


---  
 #  FlangerNode : [flangernode](flangernode.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function FlangerNode() : FlangerNode
> ``` 


---  
 #  GeneratedWaveNode : [generatedwavenode](generatedwavenode.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function GeneratedWaveNode() : GeneratedWaveNode
> ``` 


---  
 #  GetNodeGraphInfo : [nodeinfolistrange](nodeinfolistrange.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function GetNodeGraphInfo() : NodeInfoListRange
> ``` 


---  
 #  GranularSynthNode : [granularsynthnode](granularsynthnode.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function GranularSynthNode() : GranularSynthNode
> ``` 


---  
 #  HighPassNode : [highpassnode](highpassnode.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function HighPassNode() : HighPassNode
> ``` 


---  
 #  LowPassNode : [lowpassnode](lowpassnode.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function LowPassNode() : LowPassNode
> ``` 


---  
 #  MicrophoneInputNode : [microphoneinputnode](microphoneinputnode.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function MicrophoneInputNode() : MicrophoneInputNode
> ``` 


---  
 #  ModulationNode : [modulationnode](modulationnode.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ModulationNode() : ModulationNode
> ``` 


---  
 #  PanningNode : [panningnode](panningnode.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function PanningNode() : PanningNode
> ``` 


---  
 #  PitchNode : [pitchnode](pitchnode.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function PitchNode() : PitchNode
> ``` 


---  
 #  RecordingNode : [recordingnode](recordingnode.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function RecordingNode() : RecordingNode
> ``` 


---  
 #  ReverbNode : [reverbnode](reverbnode.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ReverbNode() : ReverbNode
> ``` 


---  
 #  SaveAudioNode : [saveaudionode](saveaudionode.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function SaveAudioNode() : SaveAudioNode
> ``` 


---  
 #  SoundBuffer : [soundbuffer](soundbuffer.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function SoundBuffer() : SoundBuffer
> ``` 


---  
 #  VolumeNode : [volumenode](volumenode.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function VolumeNode() : VolumeNode
> ``` 


---  
 

 
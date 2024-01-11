 `Sound`

(NOTE) Used with a CustomAudioNode to play audio data directly.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddMicUncompressedData](soundbuffer.md#addmicuncompresseddata-v)|[ SampleCount](soundbuffer.md#samplecount-zilch-engine)|[referencecountedobject](referencecountedobject.md)| |
|[ AddSampleToBuffer](soundbuffer.md#addsampletobuffer-void)| | | |
|[ GetSampleAtIndex](soundbuffer.md#getsampleatindex-zilch-en)| | | |
|[ Reset](soundbuffer.md#reset-void)| | | |


 #  Properties


---  
 #  SampleCount : [integer](../nada_base_types/integer.md)

 `read-only`

> The number of samples currently in the buffer.
> ``` lang=cpp, name=Nada
> var SampleCount : Integer


---  
 #  Methods


---  
 #  AddMicUncompressedData : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ||Array[[real](../nada_base_types/real.md)]| |
> ``` lang=cpp, name=Nada
> function AddMicUncompressedData( : Array[Real])
> ``` 


---  
 #  AddSampleToBuffer : Void

> Adds a new audio sample to the end of the buffer.
> |Name|Type|Description|
> |---|---|---|
> |sample|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function AddSampleToBuffer(sample : Real)
> ``` 


---  
 #  GetSampleAtIndex : [real](../nada_base_types/real.md)

> Returns the sample at a specific index from the beginning of the buffer.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function GetSampleAtIndex(index : Integer) : Real
> ``` 


---  
 #  Reset : Void

> Removes all data from the buffer and resets it.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Reset()
> ``` 


---  
 

 
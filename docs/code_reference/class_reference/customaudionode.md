 `Sound`

(NOTE) Uses a SoundBuffer to send audio data directly to the audio engine.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ SendBuffer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customaudionode.md#sendbuffer-void)|[ Channels](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customaudionode.md#channels-zilch-engine-doc)|[soundnode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundnode.md)| |
|[ SendMicCompressedData](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customaudionode.md#sendmiccompresseddata-vo)|[ MinimumBufferSize](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customaudionode.md#minimumbuffersize-zilch-e)| | |
|[ SendMicUncompressedData](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customaudionode.md#sendmicuncompresseddata)|[ SystemSampleRate](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customaudionode.md#systemsamplerate-zilch-en)| | |
|[ SendPartialBuffer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customaudionode.md#sendpartialbuffer-void)| | | |


 #  Properties


---  
 #  Channels : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> The number of audio channels that will be in the buffer.
> ``` lang=cpp, name=Nada
> var Channels : Integer


---  
 #  MinimumBufferSize : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> The minimum number of samples that should be sent when a NeedMoreSamples event is received.
> ``` lang=cpp, name=Nada
> var MinimumBufferSize : Integer


---  
 #  SystemSampleRate : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> The sample rate currently being used by the audio system.
> ``` lang=cpp, name=Nada
> var SystemSampleRate : Integer


---  
 #  Methods


---  
 #  SendBuffer : Void

> Sends a buffer of audio samples to the audio system for output.
> |Name|Type|Description|
> |---|---|---|
> |buffer|[soundbuffer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundbuffer.md)| |
> ``` lang=cpp, name=Nada
> function SendBuffer(buffer : SoundBuffer)
> ``` 


---  
 #  SendMicCompressedData : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ||Array[[byte](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/byte.md)]| |
> ``` lang=cpp, name=Nada
> function SendMicCompressedData( : Array[Byte])
> ``` 


---  
 #  SendMicUncompressedData : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ||Array[[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)]| |
> ``` lang=cpp, name=Nada
> function SendMicUncompressedData( : Array[Real])
> ``` 


---  
 #  SendPartialBuffer : Void

> Sends a partial buffer of audio samples to the audio system for output.
> |Name|Type|Description|
> |---|---|---|
> |buffer|[soundbuffer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/soundbuffer.md)| |
> |startAtIndex|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |howManySamples|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function SendPartialBuffer(buffer : SoundBuffer, startAtIndex : Integer, howManySamples : Integer)
> ``` 


---  
 

 
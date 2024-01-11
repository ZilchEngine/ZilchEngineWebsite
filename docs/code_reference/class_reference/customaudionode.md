 `Sound`

(NOTE) Uses a SoundBuffer to send audio data directly to the audio engine.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ SendBuffer](customaudionode.md#sendbuffer-void)|[ Channels](customaudionode.md#channels-zilch-engine-doc)|[soundnode](soundnode.md)| |
|[ SendMicCompressedData](customaudionode.md#sendmiccompresseddata-vo)|[ MinimumBufferSize](customaudionode.md#minimumbuffersize-zilch-e)| | |
|[ SendMicUncompressedData](customaudionode.md#sendmicuncompresseddata)|[ SystemSampleRate](customaudionode.md#systemsamplerate-zilch-en)| | |
|[ SendPartialBuffer](customaudionode.md#sendpartialbuffer-void)| | | |


 #  Properties


---  
 #  Channels : [integer](../nada_base_types/integer.md)

> The number of audio channels that will be in the buffer.
> ```TS:Nada
> var Channels : Integer


---  
 #  MinimumBufferSize : [integer](../nada_base_types/integer.md)

 `read-only`

> The minimum number of samples that should be sent when a NeedMoreSamples event is received.
> ```TS:Nada
> var MinimumBufferSize : Integer


---  
 #  SystemSampleRate : [integer](../nada_base_types/integer.md)

 `read-only`

> The sample rate currently being used by the audio system.
> ```TS:Nada
> var SystemSampleRate : Integer


---  
 #  Methods


---  
 #  SendBuffer : Void

> Sends a buffer of audio samples to the audio system for output.
> |Name|Type|Description|
> |---|---|---|
> |buffer|[soundbuffer](soundbuffer.md)| |
> ```TS:Nada
> function SendBuffer(buffer : SoundBuffer)
> ``` 


---  
 #  SendMicCompressedData : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ||Array[[byte](../nada_base_types/byte.md)]| |
> ```TS:Nada
> function SendMicCompressedData( : Array[Byte])
> ``` 


---  
 #  SendMicUncompressedData : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ||Array[[real](../nada_base_types/real.md)]| |
> ```TS:Nada
> function SendMicUncompressedData( : Array[Real])
> ``` 


---  
 #  SendPartialBuffer : Void

> Sends a partial buffer of audio samples to the audio system for output.
> |Name|Type|Description|
> |---|---|---|
> |buffer|[soundbuffer](soundbuffer.md)| |
> |startAtIndex|[integer](../nada_base_types/integer.md)| |
> |howManySamples|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function SendPartialBuffer(buffer : SoundBuffer, startAtIndex : Integer, howManySamples : Integer)
> ``` 


---  
 

 
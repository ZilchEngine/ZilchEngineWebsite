 `Event` `Engine`



(NOTE) Sent out when AsyncProcess completes a partial read for a stream or the stream has finished reading all data.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/asyncprocessevent.md#asyncprocessevent-void)|[ Bytes](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/asyncprocessevent.md#bytes-zilch-engine-docume)|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
| |[ StreamType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/asyncprocessevent.md#streamtype-zilch-engine-d)| | |


 #  Properties


---  
 #  Bytes : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> Bytes being read from a stream. Note: These bytes may not form a valid string if the stream type was non ascii (e.g. utf-8).
> ``` lang=cpp, name=Nada
> var Bytes : String


---  
 #  StreamType : [StreamType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#streamtype)

> The type of stream that sent this event.
> ``` lang=cpp, name=Nada
> var StreamType : StreamType


---  
 #  Methods


---  
 #  AsyncProcessEvent : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function AsyncProcessEvent()
> ``` 


---  
 

 
 `Event` `Engine`



(NOTE) Sent out when AsyncProcess completes a partial read for a stream or the stream has finished reading all data.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](asyncprocessevent.md#asyncprocessevent-void)|[Bytes](asyncprocessevent.md#bytes-zilch-engine-docume)|[event](event.md)| |
| |[StreamType](asyncprocessevent.md#streamtype-zilch-engine-d)| | |


 #  Properties


---  
 #  Bytes : [string](../nada_base_types/string.md)

> Bytes being read from a stream. Note: These bytes may not form a valid string if the stream type was non ascii (e.g. utf-8).
> ```TS:Nada
> var Bytes : String


---  
 #  StreamType : [StreamType](../enum_reference.md#streamtype)

> The type of stream that sent this event.
> ```TS:Nada
> var StreamType : StreamType


---  
 #  Methods


---  
 #  AsyncProcessEvent : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function AsyncProcessEvent()
> ``` 


---  
 

 
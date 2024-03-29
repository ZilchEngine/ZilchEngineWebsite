 `Event` `Networking`



(NOTE) Dispatched before a received net event is dispatched.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[Destination](neteventreceived.md#destination-zilch-engine)|[event](event.md)| |
| |[NetEvent](neteventreceived.md#netevent-zilch-engine-doc)| | |
| |[ReturnAllow](neteventreceived.md#returnallow-zilch-engine)| | |
| |[TheirNetPeerId](neteventreceived.md#theirnetpeerid-zilch-engi)| | |


 #  Properties


---  
 #  Destination : [cog](cog.md)

 `read-only`

> Dispatch destination object (null if the net object could not be found locally).
> ```TS:Nada
> var Destination : Cog


---  
 #  NetEvent : [event](event.md)

 `read-only`

> Network event received.
> ```TS:Nada
> var NetEvent : Event


---  
 #  ReturnAllow : [boolean](../nada_base_types/boolean.md)

> Return: Allow the received network event to be dispatched on the destination object?
> ```TS:Nada
> var ReturnAllow : Boolean


---  
 #  TheirNetPeerId : [integer](../nada_base_types/integer.md)

 `read-only`

> Their net peer ID.
> ```TS:Nada
> var TheirNetPeerId : Integer


---  
 #  Methods


---  
 

 
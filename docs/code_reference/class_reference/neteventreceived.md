 `Event` `Networking`



(NOTE) Dispatched before a received net event is dispatched.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ Destination](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/neteventreceived.md#destination-zilch-engine)|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
| |[ NetEvent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/neteventreceived.md#netevent-zilch-engine-doc)| | |
| |[ ReturnAllow](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/neteventreceived.md#returnallow-zilch-engine)| | |
| |[ TheirNetPeerId](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/neteventreceived.md#theirnetpeerid-zilch-engi)| | |


 #  Properties


---  
 #  Destination : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

 `read-only`

> Dispatch destination object (null if the net object could not be found locally).
> ``` lang=cpp, name=Nada
> var Destination : Cog


---  
 #  NetEvent : [event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)

 `read-only`

> Network event received.
> ``` lang=cpp, name=Nada
> var NetEvent : Event


---  
 #  ReturnAllow : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Return: Allow the received network event to be dispatched on the destination object?
> ``` lang=cpp, name=Nada
> var ReturnAllow : Boolean


---  
 #  TheirNetPeerId : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Their net peer ID.
> ``` lang=cpp, name=Nada
> var TheirNetPeerId : Integer


---  
 #  Methods


---  
 

 
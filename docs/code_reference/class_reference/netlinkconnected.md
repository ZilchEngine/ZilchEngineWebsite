 `Event` `Networking`



(NOTE) Dispatched after sending or receiving a connect confirmation.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ Direction](netlinkconnected.md#direction-zilch-engine-do)|[event](event.md)| |
| |[ TheirIpAddress](netlinkconnected.md#theiripaddress-zilch-engi)| | |
| |[ TheirNetPeerId](netlinkconnected.md#theirnetpeerid-zilch-engi)| | |


 #  Properties


---  
 #  Direction : [TransmissionDirection](../enum_reference.md#transmissiondirection)

 `read-only`

> Transmission direction.
> ``` lang=cpp, name=Nada
> var Direction : TransmissionDirection


---  
 #  TheirIpAddress : [ipaddress](ipaddress.md)

 `read-only`

> Their IP address (as seen from our perspective).
> ``` lang=cpp, name=Nada
> var TheirIpAddress : IpAddress


---  
 #  TheirNetPeerId : [integer](../nada_base_types/integer.md)

 `read-only`

> Their net peer ID.
> ``` lang=cpp, name=Nada
> var TheirNetPeerId : Integer


---  
 #  Methods


---  
 

 
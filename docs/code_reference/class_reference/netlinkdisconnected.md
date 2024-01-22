 `Event` `Networking`



(NOTE) Dispatched after sending or receiving a disconnect notice. Their net peer ID is released and link is destroyed immediately after this.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[Direction](netlinkdisconnected.md#direction-zilch-engine-do)|[event](event.md)| |
| |[DisconnectReason](netlinkdisconnected.md#disconnectreason-zilch-en)| | |
| |[RequestBundle](netlinkdisconnected.md#requestbundle-zilch-engin)| | |
| |[TheirIpAddress](netlinkdisconnected.md#theiripaddress-zilch-engi)| | |
| |[TheirNetPeerId](netlinkdisconnected.md#theirnetpeerid-zilch-engi)| | |


 #  Properties


---  
 #  Direction : [TransmissionDirection](../enum_reference.md#transmissiondirection)

 `read-only`

> Transmission direction.
> ```TS:Nada
> var Direction : TransmissionDirection


---  
 #  DisconnectReason : [DisconnectReason](../enum_reference.md#disconnectreason)

 `read-only`

> Disconnect reason.
> ```TS:Nada
> var DisconnectReason : DisconnectReason


---  
 #  RequestBundle : [eventbundle](eventbundle.md)

 `read-only`

> Bundled request event data.
> ```TS:Nada
> var RequestBundle : EventBundle


---  
 #  TheirIpAddress : [ipaddress](ipaddress.md)

 `read-only`

> Their IP address (as seen from our perspective).
> ```TS:Nada
> var TheirIpAddress : IpAddress


---  
 #  TheirNetPeerId : [integer](../nada_base_types/integer.md)

 `read-only`

> Their net peer ID.
> ```TS:Nada
> var TheirNetPeerId : Integer


---  
 #  Methods


---  
 

 
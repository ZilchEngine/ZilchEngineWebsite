 `Event` `Networking`



(NOTE) Dispatched after sending or receiving a disconnect notice. Their net peer ID is released and link is destroyed immediately after this.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ Direction](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netlinkdisconnected.md#direction-zilch-engine-do)|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
| |[ DisconnectReason](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netlinkdisconnected.md#disconnectreason-zilch-en)| | |
| |[ RequestBundle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netlinkdisconnected.md#requestbundle-zilch-engin)| | |
| |[ TheirIpAddress](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netlinkdisconnected.md#theiripaddress-zilch-engi)| | |
| |[ TheirNetPeerId](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netlinkdisconnected.md#theirnetpeerid-zilch-engi)| | |


 #  Properties


---  
 #  Direction : [TransmissionDirection](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#transmissiondirection)

 `read-only`

> Transmission direction.
> ``` lang=cpp, name=Nada
> var Direction : TransmissionDirection


---  
 #  DisconnectReason : [DisconnectReason](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#disconnectreason)

 `read-only`

> Disconnect reason.
> ``` lang=cpp, name=Nada
> var DisconnectReason : DisconnectReason


---  
 #  RequestBundle : [eventbundle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/eventbundle.md)

 `read-only`

> Bundled request event data.
> ``` lang=cpp, name=Nada
> var RequestBundle : EventBundle


---  
 #  TheirIpAddress : [ipaddress](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ipaddress.md)

 `read-only`

> Their IP address (as seen from our perspective).
> ``` lang=cpp, name=Nada
> var TheirIpAddress : IpAddress


---  
 #  TheirNetPeerId : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Their net peer ID.
> ``` lang=cpp, name=Nada
> var TheirNetPeerId : Integer


---  
 #  Methods


---  
 

 
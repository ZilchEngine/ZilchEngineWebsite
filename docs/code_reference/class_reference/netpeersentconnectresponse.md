 `Event` `Networking`



(NOTE) Dispatched after sending a connect response. If denied, their net peer ID is released and link is destroyed immediately after this.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ OurConnectResponse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeersentconnectresponse.md#ourconnectresponse-zero)|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
| |[ OurIpAddress](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeersentconnectresponse.md#ouripaddress-zilch-engine)| | |
| |[ OurResponseBundle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeersentconnectresponse.md#ourresponsebundle-zilch-e)| | |
| |[ TheirIpAddress](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeersentconnectresponse.md#theiripaddress-zilch-engi)| | |
| |[ TheirNetPeerId](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeersentconnectresponse.md#theirnetpeerid-zilch-engi)| | |
| |[ TheirPendingUserAddRequestCount](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeersentconnectresponse.md#theirpendinguseraddreque)| | |
| |[ TheirRequestBundle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeersentconnectresponse.md#theirrequestbundle-zero)| | |


 #  Properties


---  
 #  OurConnectResponse : [ConnectResponse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#connectresponse)

 `read-only`

> Our connect response.
> ``` lang=cpp, name=Nada
> var OurConnectResponse : ConnectResponse


---  
 #  OurIpAddress : [ipaddress](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ipaddress.md)

 `read-only`

> Our IP address (as seen from their perspective).
> ``` lang=cpp, name=Nada
> var OurIpAddress : IpAddress


---  
 #  OurResponseBundle : [eventbundle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/eventbundle.md)

 `read-only`

> Our bundled response event data.
> ``` lang=cpp, name=Nada
> var OurResponseBundle : EventBundle


---  
 #  TheirIpAddress : [ipaddress](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ipaddress.md)

 `read-only`

> Their IP address (as seen from our perspective).
> ``` lang=cpp, name=Nada
> var TheirIpAddress : IpAddress


---  
 #  TheirNetPeerId : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Their net peer ID (set only if accepted).
> ``` lang=cpp, name=Nada
> var TheirNetPeerId : Integer


---  
 #  TheirPendingUserAddRequestCount : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Their pending user add requests following this connect request (within the same frame).
> ``` lang=cpp, name=Nada
> var TheirPendingUserAddRequestCount : Integer


---  
 #  TheirRequestBundle : [eventbundle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/eventbundle.md)

 `read-only`

> Their bundled request event data.
> ``` lang=cpp, name=Nada
> var TheirRequestBundle : EventBundle


---  
 #  Methods


---  
 

 
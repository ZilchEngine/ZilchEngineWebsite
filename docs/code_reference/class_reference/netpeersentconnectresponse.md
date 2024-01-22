 `Event` `Networking`



(NOTE) Dispatched after sending a connect response. If denied, their net peer ID is released and link is destroyed immediately after this.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[OurConnectResponse](netpeersentconnectresponse.md#ourconnectresponse-zero)|[event](event.md)| |
| |[OurIpAddress](netpeersentconnectresponse.md#ouripaddress-zilch-engine)| | |
| |[OurResponseBundle](netpeersentconnectresponse.md#ourresponsebundle-zilch-e)| | |
| |[TheirIpAddress](netpeersentconnectresponse.md#theiripaddress-zilch-engi)| | |
| |[TheirNetPeerId](netpeersentconnectresponse.md#theirnetpeerid-zilch-engi)| | |
| |[TheirPendingUserAddRequestCount](netpeersentconnectresponse.md#theirpendinguseraddreque)| | |
| |[TheirRequestBundle](netpeersentconnectresponse.md#theirrequestbundle-zero)| | |


 #  Properties


---  
 #  OurConnectResponse : [ConnectResponse](../enum_reference.md#connectresponse)

 `read-only`

> Our connect response.
> ```TS:Nada
> var OurConnectResponse : ConnectResponse


---  
 #  OurIpAddress : [ipaddress](ipaddress.md)

 `read-only`

> Our IP address (as seen from their perspective).
> ```TS:Nada
> var OurIpAddress : IpAddress


---  
 #  OurResponseBundle : [eventbundle](eventbundle.md)

 `read-only`

> Our bundled response event data.
> ```TS:Nada
> var OurResponseBundle : EventBundle


---  
 #  TheirIpAddress : [ipaddress](ipaddress.md)

 `read-only`

> Their IP address (as seen from our perspective).
> ```TS:Nada
> var TheirIpAddress : IpAddress


---  
 #  TheirNetPeerId : [integer](../nada_base_types/integer.md)

 `read-only`

> Their net peer ID (set only if accepted).
> ```TS:Nada
> var TheirNetPeerId : Integer


---  
 #  TheirPendingUserAddRequestCount : [integer](../nada_base_types/integer.md)

 `read-only`

> Their pending user add requests following this connect request (within the same frame).
> ```TS:Nada
> var TheirPendingUserAddRequestCount : Integer


---  
 #  TheirRequestBundle : [eventbundle](eventbundle.md)

 `read-only`

> Their bundled request event data.
> ```TS:Nada
> var TheirRequestBundle : EventBundle


---  
 #  Methods


---  
 

 
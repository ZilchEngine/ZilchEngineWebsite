 `Event` `Networking`



(NOTE) Dispatched after receiving a connect request. If accepted, their net peer ID is assigned immediately after this. Return true to accept the connect request, else false.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ OurIpAddress](netpeerreceivedconnectrequest.md#ouripaddress-zilch-engine)|[event](event.md)| |
| |[ ReturnOurConnectResponse](netpeerreceivedconnectrequest.md#returnourconnectresponse)| | |
| |[ ReturnOurResponseBundle](netpeerreceivedconnectrequest.md#returnourresponsebundle)| | |
| |[ TheirIpAddress](netpeerreceivedconnectrequest.md#theiripaddress-zilch-engi)| | |
| |[ TheirPendingUserAddRequestCount](netpeerreceivedconnectrequest.md#theirpendinguseraddreque)| | |
| |[ TheirRequestBundle](netpeerreceivedconnectrequest.md#theirrequestbundle-zero)| | |


 #  Properties


---  
 #  OurIpAddress : [ipaddress](ipaddress.md)

 `read-only`

> Our IP address (as seen from their perspective).
> ```TS:Nada
> var OurIpAddress : IpAddress


---  
 #  ReturnOurConnectResponse : [boolean](../nada_base_types/boolean.md)

> Return: Our connect response (accept the connect request?).
> ```TS:Nada
> var ReturnOurConnectResponse : Boolean


---  
 #  ReturnOurResponseBundle : [eventbundle](eventbundle.md)

> Return: Our bundled response event data.
> ```TS:Nada
> var ReturnOurResponseBundle : EventBundle


---  
 #  TheirIpAddress : [ipaddress](ipaddress.md)

 `read-only`

> Their IP address (as seen from our perspective).
> ```TS:Nada
> var TheirIpAddress : IpAddress


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
 

 
 `Event` `Networking`



(NOTE) Dispatched after sending a connect request.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ OurPendingUserAddRequestCount](netpeersentconnectrequest.md#ourpendinguseraddrequest)|[event](event.md)| |
| |[ OurRequestBundle](netpeersentconnectrequest.md#ourrequestbundle-zilch-en)| | |
| |[ TheirIpAddress](netpeersentconnectrequest.md#theiripaddress-zilch-engi)| | |


 #  Properties


---  
 #  OurPendingUserAddRequestCount : [integer](../nada_base_types/integer.md)

 `read-only`

> Our pending user add requests following this connect request (within the same frame).
> ``` lang=cpp, name=Nada
> var OurPendingUserAddRequestCount : Integer


---  
 #  OurRequestBundle : [eventbundle](eventbundle.md)

 `read-only`

> Our bundled request event data.
> ``` lang=cpp, name=Nada
> var OurRequestBundle : EventBundle


---  
 #  TheirIpAddress : [ipaddress](ipaddress.md)

 `read-only`

> Their IP address (as seen from our perspective).
> ``` lang=cpp, name=Nada
> var TheirIpAddress : IpAddress


---  
 #  Methods


---  
 

 
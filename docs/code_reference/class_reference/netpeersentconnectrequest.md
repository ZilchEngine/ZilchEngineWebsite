 `Event` `Networking`



(NOTE) Dispatched after sending a connect request.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ OurPendingUserAddRequestCount](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeersentconnectrequest.md#ourpendinguseraddrequest)|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
| |[ OurRequestBundle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeersentconnectrequest.md#ourrequestbundle-zilch-en)| | |
| |[ TheirIpAddress](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeersentconnectrequest.md#theiripaddress-zilch-engi)| | |


 #  Properties


---  
 #  OurPendingUserAddRequestCount : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Our pending user add requests following this connect request (within the same frame).
> ``` lang=cpp, name=Nada
> var OurPendingUserAddRequestCount : Integer


---  
 #  OurRequestBundle : [eventbundle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/eventbundle.md)

 `read-only`

> Our bundled request event data.
> ``` lang=cpp, name=Nada
> var OurRequestBundle : EventBundle


---  
 #  TheirIpAddress : [ipaddress](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ipaddress.md)

 `read-only`

> Their IP address (as seen from our perspective).
> ``` lang=cpp, name=Nada
> var TheirIpAddress : IpAddress


---  
 #  Methods


---  
 

 
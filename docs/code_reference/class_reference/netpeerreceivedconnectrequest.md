 `Event` `Networking`



(NOTE) Dispatched after receiving a connect request. If accepted, their net peer ID is assigned immediately after this. Return true to accept the connect request, else false.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ OurIpAddress](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeerreceivedconnectrequest.md#ouripaddress-zilch-engine)|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
| |[ ReturnOurConnectResponse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeerreceivedconnectrequest.md#returnourconnectresponse)| | |
| |[ ReturnOurResponseBundle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeerreceivedconnectrequest.md#returnourresponsebundle)| | |
| |[ TheirIpAddress](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeerreceivedconnectrequest.md#theiripaddress-zilch-engi)| | |
| |[ TheirPendingUserAddRequestCount](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeerreceivedconnectrequest.md#theirpendinguseraddreque)| | |
| |[ TheirRequestBundle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeerreceivedconnectrequest.md#theirrequestbundle-zero)| | |


 #  Properties


---  
 #  OurIpAddress : [ipaddress](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ipaddress.md)

 `read-only`

> Our IP address (as seen from their perspective).
> ``` lang=cpp, name=Nada
> var OurIpAddress : IpAddress


---  
 #  ReturnOurConnectResponse : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Return: Our connect response (accept the connect request?).
> ``` lang=cpp, name=Nada
> var ReturnOurConnectResponse : Boolean


---  
 #  ReturnOurResponseBundle : [eventbundle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/eventbundle.md)

> Return: Our bundled response event data.
> ``` lang=cpp, name=Nada
> var ReturnOurResponseBundle : EventBundle


---  
 #  TheirIpAddress : [ipaddress](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ipaddress.md)

 `read-only`

> Their IP address (as seen from our perspective).
> ``` lang=cpp, name=Nada
> var TheirIpAddress : IpAddress


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
 

 
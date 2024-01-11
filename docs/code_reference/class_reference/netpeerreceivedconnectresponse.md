 `Event` `Networking`



(NOTE) Dispatched after receiving a connect response. If accepted, our net peer ID is set immediately before this and a connect confirmation is sent after this. If denied, our net peer ID is cleared and link is destroyed immediately after this.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ OurIpAddress](netpeerreceivedconnectresponse.md#ouripaddress-zilch-engine)|[event](event.md)| |
| |[ OurNetPeerId](netpeerreceivedconnectresponse.md#ournetpeerid-zilch-engine)| | |
| |[ OurPendingUserAddRequestCount](netpeerreceivedconnectresponse.md#ourpendinguseraddrequest)| | |
| |[ OurRequestBundle](netpeerreceivedconnectresponse.md#ourrequestbundle-zilch-en)| | |
| |[ TheirConnectResponse](netpeerreceivedconnectresponse.md#theirconnectresponse-zer)| | |
| |[ TheirIpAddress](netpeerreceivedconnectresponse.md#theiripaddress-zilch-engi)| | |
| |[ TheirResponseBundle](netpeerreceivedconnectresponse.md#theirresponsebundle-zero)| | |


 #  Properties


---  
 #  OurIpAddress : [ipaddress](ipaddress.md)

 `read-only`

> Our IP address (as seen from their perspective).
> ``` lang=cpp, name=Nada
> var OurIpAddress : IpAddress


---  
 #  OurNetPeerId : [integer](../nada_base_types/integer.md)

 `read-only`

> Our net peer ID (set only if accepted).
> ``` lang=cpp, name=Nada
> var OurNetPeerId : Integer


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
 #  TheirConnectResponse : [ConnectResponse](../enum_reference.md#connectresponse)

 `read-only`

> Their connect response.
> ``` lang=cpp, name=Nada
> var TheirConnectResponse : ConnectResponse


---  
 #  TheirIpAddress : [ipaddress](ipaddress.md)

 `read-only`

> Their IP address (as seen from our perspective).
> ``` lang=cpp, name=Nada
> var TheirIpAddress : IpAddress


---  
 #  TheirResponseBundle : [eventbundle](eventbundle.md)

 `read-only`

> Their bundled response event data.
> ``` lang=cpp, name=Nada
> var TheirResponseBundle : EventBundle


---  
 #  Methods


---  
 

 
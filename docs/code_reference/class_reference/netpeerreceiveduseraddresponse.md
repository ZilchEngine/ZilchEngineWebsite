 `Event` `Networking`



(NOTE) Dispatched after receiving a net user add response.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ OurNetUserId](netpeerreceiveduseraddresponse.md#ournetuserid-zilch-engine)|[event](event.md)| |
| |[ OurRequestBundle](netpeerreceiveduseraddresponse.md#ourrequestbundle-zilch-en)| | |
| |[ TheirAddResponse](netpeerreceiveduseraddresponse.md#theiraddresponse-zilch-en)| | |
| |[ TheirIpAddress](netpeerreceiveduseraddresponse.md#theiripaddress-zilch-engi)| | |
| |[ TheirNetPeerId](netpeerreceiveduseraddresponse.md#theirnetpeerid-zilch-engi)| | |
| |[ TheirResponseBundle](netpeerreceiveduseraddresponse.md#theirresponsebundle-zero)| | |


 #  Properties


---  
 #  OurNetUserId : [integer](../nada_base_types/integer.md)

 `read-only`

> Our net user ID (set only if accepted).
> ``` lang=cpp, name=Nada
> var OurNetUserId : Integer


---  
 #  OurRequestBundle : [eventbundle](eventbundle.md)

 `read-only`

> Our bundled request event data.
> ``` lang=cpp, name=Nada
> var OurRequestBundle : EventBundle


---  
 #  TheirAddResponse : [NetUserAddResponse](../enum_reference.md#netuseraddresponse)

 `read-only`

> Their add response.
> ``` lang=cpp, name=Nada
> var TheirAddResponse : NetUserAddResponse


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
 #  TheirResponseBundle : [eventbundle](eventbundle.md)

 `read-only`

> Their bundled response event data.
> ``` lang=cpp, name=Nada
> var TheirResponseBundle : EventBundle


---  
 #  Methods


---  
 

 
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
> ```TS:Nada
> var OurNetUserId : Integer


---  
 #  OurRequestBundle : [eventbundle](eventbundle.md)

 `read-only`

> Our bundled request event data.
> ```TS:Nada
> var OurRequestBundle : EventBundle


---  
 #  TheirAddResponse : [NetUserAddResponse](../enum_reference.md#netuseraddresponse)

 `read-only`

> Their add response.
> ```TS:Nada
> var TheirAddResponse : NetUserAddResponse


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
 #  TheirResponseBundle : [eventbundle](eventbundle.md)

 `read-only`

> Their bundled response event data.
> ```TS:Nada
> var TheirResponseBundle : EventBundle


---  
 #  Methods


---  
 

 
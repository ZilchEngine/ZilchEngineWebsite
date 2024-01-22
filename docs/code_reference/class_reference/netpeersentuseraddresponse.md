 `Event` `Networking`



(NOTE) Dispatched after sending a net user add response.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[OurAddResponse](netpeersentuseraddresponse.md#ouraddresponse-zilch-engi)|[event](event.md)| |
| |[OurResponseBundle](netpeersentuseraddresponse.md#ourresponsebundle-zilch-e)| | |
| |[TheirIpAddress](netpeersentuseraddresponse.md#theiripaddress-zilch-engi)| | |
| |[TheirNetPeerId](netpeersentuseraddresponse.md#theirnetpeerid-zilch-engi)| | |
| |[TheirNetUser](netpeersentuseraddresponse.md#theirnetuser-zilch-engine)| | |
| |[TheirNetUserId](netpeersentuseraddresponse.md#theirnetuserid-zilch-engi)| | |
| |[TheirRequestBundle](netpeersentuseraddresponse.md#theirrequestbundle-zero)| | |


 #  Properties


---  
 #  OurAddResponse : [NetUserAddResponse](../enum_reference.md#netuseraddresponse)

 `read-only`

> Our add response.
> ```TS:Nada
> var OurAddResponse : NetUserAddResponse


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

> Their net peer ID.
> ```TS:Nada
> var TheirNetPeerId : Integer


---  
 #  TheirNetUser : [cog](cog.md)

 `read-only`

> Their net user object about to be added (set only if accepted).
> ```TS:Nada
> var TheirNetUser : Cog


---  
 #  TheirNetUserId : [integer](../nada_base_types/integer.md)

 `read-only`

> Their net user ID (set only if accepted).
> ```TS:Nada
> var TheirNetUserId : Integer


---  
 #  TheirRequestBundle : [eventbundle](eventbundle.md)

 `read-only`

> Their bundled request event data.
> ```TS:Nada
> var TheirRequestBundle : EventBundle


---  
 #  Methods


---  
 

 
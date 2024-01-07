 `Event` `Networking`



(NOTE) Dispatched after sending a net user add response.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ OurAddResponse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeersentuseraddresponse.md#ouraddresponse-zilch-engi)|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
| |[ OurResponseBundle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeersentuseraddresponse.md#ourresponsebundle-zilch-e)| | |
| |[ TheirIpAddress](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeersentuseraddresponse.md#theiripaddress-zilch-engi)| | |
| |[ TheirNetPeerId](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeersentuseraddresponse.md#theirnetpeerid-zilch-engi)| | |
| |[ TheirNetUser](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeersentuseraddresponse.md#theirnetuser-zilch-engine)| | |
| |[ TheirNetUserId](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeersentuseraddresponse.md#theirnetuserid-zilch-engi)| | |
| |[ TheirRequestBundle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeersentuseraddresponse.md#theirrequestbundle-zero)| | |


 #  Properties


---  
 #  OurAddResponse : [NetUserAddResponse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#netuseraddresponse)

 `read-only`

> Our add response.
> ``` lang=cpp, name=Nada
> var OurAddResponse : NetUserAddResponse


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

> Their net peer ID.
> ``` lang=cpp, name=Nada
> var TheirNetPeerId : Integer


---  
 #  TheirNetUser : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

 `read-only`

> Their net user object about to be added (set only if accepted).
> ``` lang=cpp, name=Nada
> var TheirNetUser : Cog


---  
 #  TheirNetUserId : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Their net user ID (set only if accepted).
> ``` lang=cpp, name=Nada
> var TheirNetUserId : Integer


---  
 #  TheirRequestBundle : [eventbundle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/eventbundle.md)

 `read-only`

> Their bundled request event data.
> ``` lang=cpp, name=Nada
> var TheirRequestBundle : EventBundle


---  
 #  Methods


---  
 

 
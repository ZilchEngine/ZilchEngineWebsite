 `Event` `Networking`



(NOTE) Dispatched after receiving a net user add response.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ OurNetUserId](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeerreceiveduseraddresponse.md#ournetuserid-zilch-engine)|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
| |[ OurRequestBundle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeerreceiveduseraddresponse.md#ourrequestbundle-zilch-en)| | |
| |[ TheirAddResponse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeerreceiveduseraddresponse.md#theiraddresponse-zilch-en)| | |
| |[ TheirIpAddress](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeerreceiveduseraddresponse.md#theiripaddress-zilch-engi)| | |
| |[ TheirNetPeerId](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeerreceiveduseraddresponse.md#theirnetpeerid-zilch-engi)| | |
| |[ TheirResponseBundle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeerreceiveduseraddresponse.md#theirresponsebundle-zero)| | |


 #  Properties


---  
 #  OurNetUserId : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Our net user ID (set only if accepted).
> ``` lang=cpp, name=Nada
> var OurNetUserId : Integer


---  
 #  OurRequestBundle : [eventbundle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/eventbundle.md)

 `read-only`

> Our bundled request event data.
> ``` lang=cpp, name=Nada
> var OurRequestBundle : EventBundle


---  
 #  TheirAddResponse : [NetUserAddResponse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#netuseraddresponse)

 `read-only`

> Their add response.
> ``` lang=cpp, name=Nada
> var TheirAddResponse : NetUserAddResponse


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
 #  TheirResponseBundle : [eventbundle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/eventbundle.md)

 `read-only`

> Their bundled response event data.
> ``` lang=cpp, name=Nada
> var TheirResponseBundle : EventBundle


---  
 #  Methods


---  
 

 
 `Event` `Networking`



(NOTE) Dispatched after receiving a net user add request.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ ReturnOurAddResponse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeerreceiveduseraddrequest.md#returnouraddresponse-zer)|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
| |[ ReturnOurResponseBundle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeerreceiveduseraddrequest.md#returnourresponsebundle)| | |
| |[ ReturnTheirNetUser](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeerreceiveduseraddrequest.md#returntheirnetuser-zero)| | |
| |[ TheirIpAddress](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeerreceiveduseraddrequest.md#theiripaddress-zilch-engi)| | |
| |[ TheirNetPeerId](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeerreceiveduseraddrequest.md#theirnetpeerid-zilch-engi)| | |
| |[ TheirNetUserId](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeerreceiveduseraddrequest.md#theirnetuserid-zilch-engi)| | |
| |[ TheirRequestBundle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeerreceiveduseraddrequest.md#theirrequestbundle-zero)| | |


 #  Properties


---  
 #  ReturnOurAddResponse : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Return: Our add response (accept the add request?).
> ``` lang=cpp, name=Nada
> var ReturnOurAddResponse : Boolean


---  
 #  ReturnOurResponseBundle : [eventbundle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/eventbundle.md)

> Return: Our bundled response event data.
> ``` lang=cpp, name=Nada
> var ReturnOurResponseBundle : EventBundle


---  
 #  ReturnTheirNetUser : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Return: Their network user object (must have a NetUser component).
> ``` lang=cpp, name=Nada
> var ReturnTheirNetUser : Cog


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
 #  TheirNetUserId : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Their net user ID (released back to the store if not accepted).
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
 

 
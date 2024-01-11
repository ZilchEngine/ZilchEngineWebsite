 `Event` `Networking`



(NOTE) Dispatched after receiving a net user add request.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ ReturnOurAddResponse](netpeerreceiveduseraddrequest.md#returnouraddresponse-zer)|[event](event.md)| |
| |[ ReturnOurResponseBundle](netpeerreceiveduseraddrequest.md#returnourresponsebundle)| | |
| |[ ReturnTheirNetUser](netpeerreceiveduseraddrequest.md#returntheirnetuser-zero)| | |
| |[ TheirIpAddress](netpeerreceiveduseraddrequest.md#theiripaddress-zilch-engi)| | |
| |[ TheirNetPeerId](netpeerreceiveduseraddrequest.md#theirnetpeerid-zilch-engi)| | |
| |[ TheirNetUserId](netpeerreceiveduseraddrequest.md#theirnetuserid-zilch-engi)| | |
| |[ TheirRequestBundle](netpeerreceiveduseraddrequest.md#theirrequestbundle-zero)| | |


 #  Properties


---  
 #  ReturnOurAddResponse : [boolean](../nada_base_types/boolean.md)

> Return: Our add response (accept the add request?).
> ``` lang=cpp, name=Nada
> var ReturnOurAddResponse : Boolean


---  
 #  ReturnOurResponseBundle : [eventbundle](eventbundle.md)

> Return: Our bundled response event data.
> ``` lang=cpp, name=Nada
> var ReturnOurResponseBundle : EventBundle


---  
 #  ReturnTheirNetUser : [cog](cog.md)

> Return: Their network user object (must have a NetUser component).
> ``` lang=cpp, name=Nada
> var ReturnTheirNetUser : Cog


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
 #  TheirNetUserId : [integer](../nada_base_types/integer.md)

 `read-only`

> Their net user ID (released back to the store if not accepted).
> ``` lang=cpp, name=Nada
> var TheirNetUserId : Integer


---  
 #  TheirRequestBundle : [eventbundle](eventbundle.md)

 `read-only`

> Their bundled request event data.
> ``` lang=cpp, name=Nada
> var TheirRequestBundle : EventBundle


---  
 #  Methods


---  
 

 
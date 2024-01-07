 `Networking`

(NOTE) Describes a network host.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ BasicHostInfo](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/nethost.md#basichostinfo-zilch-engin)|[safeid32](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/safeid32.md)| |
| |[ ExtraHostInfo](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/nethost.md#extrahostinfo-zilch-engin)| | |
| |[ IpAddress](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/nethost.md#ipaddress-zilch-engine-do)| | |
| |[ Latency](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/nethost.md#latency-zilch-engine-docu)| | |
| |[ Network](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/nethost.md#network-zilch-engine-docu)| | |
| |[ RoundTripTime](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/nethost.md#roundtriptime-zilch-engin)| | |


 #  Properties


---  
 #  BasicHostInfo : [eventbundle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/eventbundle.md)

 `read-only`

> Basic host info (limited to 480 bytes).
> ``` lang=cpp, name=Nada
> var BasicHostInfo : EventBundle


---  
 #  ExtraHostInfo : [eventbundle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/eventbundle.md)

 `read-only`

> Extra host info.
> ``` lang=cpp, name=Nada
> var ExtraHostInfo : EventBundle


---  
 #  IpAddress : [ipaddress](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ipaddress.md)

 `read-only`

> Host's IP address.
> ``` lang=cpp, name=Nada
> var IpAddress : IpAddress


---  
 #  Latency : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Returns the estimated latency ((RTT/2)) in milliseconds from our peer to this host.
> ``` lang=cpp, name=Nada
> var Latency : Integer


---  
 #  Network : [Network](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#network)

 `read-only`

> Host's network residence.
> ``` lang=cpp, name=Nada
> var Network : Network


---  
 #  RoundTripTime : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Returns the round-trip time (RTT) in milliseconds from our peer to this host.
> ``` lang=cpp, name=Nada
> var RoundTripTime : Integer


---  
 #  Methods


---  
 

 
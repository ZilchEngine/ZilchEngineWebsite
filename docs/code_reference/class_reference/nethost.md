 `Networking`

(NOTE) Describes a network host.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[BasicHostInfo](nethost.md#basichostinfo-zilch-engin)|[safeid32](safeid32.md)| |
| |[ExtraHostInfo](nethost.md#extrahostinfo-zilch-engin)| | |
| |[IpAddress](nethost.md#ipaddress-zilch-engine-do)| | |
| |[Latency](nethost.md#latency-zilch-engine-docu)| | |
| |[Network](nethost.md#network-zilch-engine-docu)| | |
| |[RoundTripTime](nethost.md#roundtriptime-zilch-engin)| | |


 #  Properties


---  
 #  BasicHostInfo : [eventbundle](eventbundle.md)

 `read-only`

> Basic host info (limited to 480 bytes).
> ```TS:Nada
> var BasicHostInfo : EventBundle


---  
 #  ExtraHostInfo : [eventbundle](eventbundle.md)

 `read-only`

> Extra host info.
> ```TS:Nada
> var ExtraHostInfo : EventBundle


---  
 #  IpAddress : [ipaddress](ipaddress.md)

 `read-only`

> Host's IP address.
> ```TS:Nada
> var IpAddress : IpAddress


---  
 #  Latency : [integer](../nada_base_types/integer.md)

 `read-only`

> Returns the estimated latency ((RTT/2)) in milliseconds from our peer to this host.
> ```TS:Nada
> var Latency : Integer


---  
 #  Network : [Network](../enum_reference.md#network)

 `read-only`

> Host's network residence.
> ```TS:Nada
> var Network : Network


---  
 #  RoundTripTime : [integer](../nada_base_types/integer.md)

 `read-only`

> Returns the round-trip time (RTT) in milliseconds from our peer to this host.
> ```TS:Nada
> var RoundTripTime : Integer


---  
 #  Methods


---  
 

 
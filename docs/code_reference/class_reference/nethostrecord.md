 `Networking`

(NOTE) NetHostRecord. A record that contains the basic information of a game server. After a certain lifetime records expire on the master server.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ BasicHostInfo](nethostrecord.md#basichostinfo-zilch-engin)|[safeid32](safeid32.md)| |
| |[ IpAddress](nethostrecord.md#ipaddress-zilch-engine-do)| | |
| |[ Lifetime](nethostrecord.md#lifetime-zilch-engine-doc)| | |


 #  Properties


---  
 #  BasicHostInfo : [eventbundle](eventbundle.md)

 `read-only`

> The info published along with their record. Contains game server specific data.
> ```TS:Nada
> var BasicHostInfo : EventBundle


---  
 #  IpAddress : [ipaddress](ipaddress.md)

 `read-only`

> The IpAddress associated with this record. This is who published it.
> ```TS:Nada
> var IpAddress : IpAddress


---  
 #  Lifetime : [real](../nada_base_types/real.md)

 `read-only`

> How long has this record been alive in seconds?
> ```TS:Nada
> var Lifetime : Real


---  
 #  Methods


---  
 

 
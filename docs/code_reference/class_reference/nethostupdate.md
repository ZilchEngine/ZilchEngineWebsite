 `Event` `Networking`



(NOTE) Dispatched when a host discovery operation update occurs.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ Host](nethostupdate.md#host-zilch-engine-documen)|[event](event.md)| |
| |[ Network](nethostupdate.md#network-zilch-engine-docu)| | |
| |[ RefreshResult](nethostupdate.md#refreshresult-zilch-engin)| | |
| |[ ResponseTime](nethostupdate.md#responsetime-zilch-engine)| | |


 #  Properties


---  
 #  Host : [nethost](nethost.md)

 `read-only`

> Host discovered or refreshed (will contain the first host updated if this is a list update).
> ```TS:Nada
> var Host : NetHost


---  
 #  Network : [Network](../enum_reference.md#network)

 `read-only`

> Operation target network.
> ```TS:Nada
> var Network : Network


---  
 #  RefreshResult : [NetRefreshResult](../enum_reference.md#netrefreshresult)

 `read-only`

> Whether or not the operation completed successfully.
> ```TS:Nada
> var RefreshResult : NetRefreshResult


---  
 #  ResponseTime : [real](../nada_base_types/real.md)

 `read-only`

> Operation response time (from request to completion).
> ```TS:Nada
> var ResponseTime : Real


---  
 #  Methods


---  
 

 
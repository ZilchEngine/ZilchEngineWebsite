 `Event` `Networking`



(NOTE) Dispatched after an outgoing/incoming net channel property change is detected during a particular replication phase.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ ChannelName](netchannelpropertychange.md#channelname-zilch-engine)|[event](event.md)| |
| |[ ComponentName](netchannelpropertychange.md#componentname-zilch-engin)| | |
| |[ Direction](netchannelpropertychange.md#direction-zilch-engine-do)| | |
| |[ Object](netchannelpropertychange.md#object-zilch-engine-docum)| | |
| |[ PropertyName](netchannelpropertychange.md#propertyname-zilch-engine)| | |
| |[ ReplicationPhase](netchannelpropertychange.md#replicationphase-zilch-en)| | |
| |[ Timestamp](netchannelpropertychange.md#timestamp-zilch-engine-do)| | |


 #  Properties


---  
 #  ChannelName : [string](../nada_base_types/string.md)

 `read-only`

> The changed net channel.
> ```TS:Nada
> var ChannelName : String


---  
 #  ComponentName : [string](../nada_base_types/string.md)

 `read-only`

> The component which declared the changed net property.
> ```TS:Nada
> var ComponentName : String


---  
 #  Direction : [TransmissionDirection](../enum_reference.md#transmissiondirection)

 `read-only`

> The change direction.
> ```TS:Nada
> var Direction : TransmissionDirection


---  
 #  Object : [cog](cog.md)

 `read-only`

> The changed net object.
> ```TS:Nada
> var Object : Cog


---  
 #  PropertyName : [string](../nada_base_types/string.md)

 `read-only`

> The changed net property.
> ```TS:Nada
> var PropertyName : String


---  
 #  ReplicationPhase : [ReplicationPhase](../enum_reference.md#replicationphase)

 `read-only`

> The replication phase.
> ```TS:Nada
> var ReplicationPhase : ReplicationPhase


---  
 #  Timestamp : [real](../nada_base_types/real.md)

 `read-only`

> The time this change occurred.
> ```TS:Nada
> var Timestamp : Real


---  
 #  Methods


---  
 

 
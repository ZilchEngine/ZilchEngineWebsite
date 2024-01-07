 `Event` `Networking`



(NOTE) Dispatched after an outgoing/incoming net channel property change is detected during a particular replication phase.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ ChannelName](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannelpropertychange.md#channelname-zilch-engine)|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
| |[ ComponentName](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannelpropertychange.md#componentname-zilch-engin)| | |
| |[ Direction](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannelpropertychange.md#direction-zilch-engine-do)| | |
| |[ Object](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannelpropertychange.md#object-zilch-engine-docum)| | |
| |[ PropertyName](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannelpropertychange.md#propertyname-zilch-engine)| | |
| |[ ReplicationPhase](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannelpropertychange.md#replicationphase-zilch-en)| | |
| |[ Timestamp](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannelpropertychange.md#timestamp-zilch-engine-do)| | |


 #  Properties


---  
 #  ChannelName : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

 `read-only`

> The changed net channel.
> ``` lang=cpp, name=Nada
> var ChannelName : String


---  
 #  ComponentName : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

 `read-only`

> The component which declared the changed net property.
> ``` lang=cpp, name=Nada
> var ComponentName : String


---  
 #  Direction : [TransmissionDirection](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#transmissiondirection)

 `read-only`

> The change direction.
> ``` lang=cpp, name=Nada
> var Direction : TransmissionDirection


---  
 #  Object : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

 `read-only`

> The changed net object.
> ``` lang=cpp, name=Nada
> var Object : Cog


---  
 #  PropertyName : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

 `read-only`

> The changed net property.
> ``` lang=cpp, name=Nada
> var PropertyName : String


---  
 #  ReplicationPhase : [ReplicationPhase](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#replicationphase)

 `read-only`

> The replication phase.
> ``` lang=cpp, name=Nada
> var ReplicationPhase : ReplicationPhase


---  
 #  Timestamp : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

 `read-only`

> The time this change occurred.
> ``` lang=cpp, name=Nada
> var Timestamp : Real


---  
 #  Methods


---  
 

 
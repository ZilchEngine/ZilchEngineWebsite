 `Networking`



(NOTE) Network Channel Type. Configures the replication of a set of properties on the network.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ResetConfig](netchanneltype.md#resetconfig-void)|[AcceptIncomingChanges](netchanneltype.md#acceptincomingchanges-ze)|[safeid32object](safeid32object.md)| |
|[SetConfig](netchanneltype.md#setconfig-void)|[AccurateTimestampOnChange](netchanneltype.md#accuratetimestamponchang)| | |
| |[AllowNapping](netchanneltype.md#allownapping-zilch-engine)| | |
| |[AllowRelay](netchanneltype.md#allowrelay-zilch-engine-d)| | |
| |[AuthorityDefault](netchanneltype.md#authoritydefault-zilch-en)| | |
| |[AuthorityMode](netchanneltype.md#authoritymode-zilch-engin)| | |
| |[AwakeDetectionInterval](netchanneltype.md#awakedetectioninterval-z)| | |
| |[AwakeDuration](netchanneltype.md#awakeduration-zilch-engin)| | |
| |[DetectionMode](netchanneltype.md#detectionmode-zilch-engin)| | |
| |[DetectOutgoingChanges](netchanneltype.md#detectoutgoingchanges-ze)| | |
| |[EventOnIncomingPropertyChange](netchanneltype.md#eventonincomingpropertyc)| | |
| |[EventOnOutgoingPropertyChange](netchanneltype.md#eventonoutgoingpropertyc)| | |
| |[Name](netchanneltype.md#name-zilch-engine-documen)| | |
| |[NapDetectionInterval](netchanneltype.md#napdetectioninterval-zer)| | |
| |[ReliabilityMode](netchanneltype.md#reliabilitymode-zilch-eng)| | |
| |[ReplicateOnOffline](netchanneltype.md#replicateonoffline-zero)| | |
| |[ReplicateOnOnline](netchanneltype.md#replicateononline-zilch-e)| | |
| |[SerializationMode](netchanneltype.md#serializationmode-zilch-e)| | |
| |[TransferMode](netchanneltype.md#transfermode-zilch-engine)| | |


 #  Properties


---  
 #  AcceptIncomingChanges : [boolean](../nada_base_types/boolean.md)

> Controls whether or not net channels should accept incoming changes.
> ```TS:Nada
> var AcceptIncomingChanges : Boolean


---  
 #  AccurateTimestampOnChange : [boolean](../nada_base_types/boolean.md)

> Controls whether or not the net channel will serialize an accurate timestamp value when changed, or will instead accept an estimated timestamp value. (This setting may be overridden for net channels belonging to a specific net object by enabling the corresponding net object setting)
> ```TS:Nada
> var AccurateTimestampOnChange : Boolean


---  
 #  AllowNapping : [boolean](../nada_base_types/boolean.md)

> Controls whether or not net channels may nap (perform change detection on longer intervals) if they haven't changed in a while.
> ```TS:Nada
> var AllowNapping : Boolean


---  
 #  AllowRelay : [boolean](../nada_base_types/boolean.md)

> Controls whether or not net channels will have their changes immediately broadcast to all relevant, incidental peers (if any) once received. (Enabling this allows a server to automatically relay client authoritative changes to other clients, otherwise this must be done manually using NetChannel::ReplicateNow)
> ```TS:Nada
> var AllowRelay : Boolean


---  
 #  AuthorityDefault : [Authority](../enum_reference.md#authority)

> Controls which peer has the authority to observe and replicate property changes on each net channel by default. (Client: Indicates both the client and server are allowed to observe and replicate property changes) (Server: Indicates only the server is allowed to observe and replicate property changes) Only a single client, specified by NetObject::NetUserOwnerPeerId, may possess client authority at any given time. The server is still responsible for relaying contained property changes to other clients, but will not replicate contained property changes back to the authority client. However, the server is also still responsible for other replication commands (such as object creation/destruction), and these WILL be replicated to the authority client.
> ```TS:Nada
> var AuthorityDefault : Authority


---  
 #  AuthorityMode : [AuthorityMode](../enum_reference.md#authoritymode)

> Controls when net channels can modify their change authority. (Dynamic: Authority may be modified at any time, even after a net object is brought online) (Fixed: Authority may be modified only before a net object is brought online) (Cannot be modified at game runtime)
> ```TS:Nada
> var AuthorityMode : AuthorityMode


---  
 #  AwakeDetectionInterval : [integer](../nada_base_types/integer.md)

> Controls the frame interval in which awake net channels are observed for changes. (Cannot be modified at game runtime)
> ```TS:Nada
> var AwakeDetectionInterval : Integer


---  
 #  AwakeDuration : [integer](../nada_base_types/integer.md)

> Controls the frame duration following the last detected change in which net channels are considered actively changing and will be kept awake.
> ```TS:Nada
> var AwakeDuration : Integer


---  
 #  DetectionMode : [DetectionMode](../enum_reference.md#detectionmode)

> Controls how net channel changes are detected. (Assume: Assumes something has changed) (Manual: Detects changes manually using change flags) (Automatic: Detects changes automatically using comparisons) (Manumatic: Detects changes manually using change flags and automatically using comparisons)
> ```TS:Nada
> var DetectionMode : DetectionMode


---  
 #  DetectOutgoingChanges : [boolean](../nada_base_types/boolean.md)

> Controls whether or not net channels should detect outgoing changes.
> ```TS:Nada
> var DetectOutgoingChanges : Boolean


---  
 #  EventOnIncomingPropertyChange : [boolean](../nada_base_types/boolean.md)

> Controls whether or not net channels should dispatch NetChannelIncomingPropertyChange when an incoming net property change is accepted.
> ```TS:Nada
> var EventOnIncomingPropertyChange : Boolean


---  
 #  EventOnOutgoingPropertyChange : [boolean](../nada_base_types/boolean.md)

> Controls whether or not net channels should dispatch NetChannelOutgoingPropertyChange when an outgoing net property change is detected.
> ```TS:Nada
> var EventOnOutgoingPropertyChange : Boolean


---  
 #  Name : [string](../nada_base_types/string.md)

 `read-only`

> Net channel type name.
> ```TS:Nada
> var Name : String


---  
 #  NapDetectionInterval : [integer](../nada_base_types/integer.md)

> Controls the frame interval in which napping net channels are observed for changes. (Cannot be modified at game runtime)
> ```TS:Nada
> var NapDetectionInterval : Integer


---  
 #  ReliabilityMode : [ReliabilityMode](../enum_reference.md#reliabilitymode)

> Controls whether or not net channel changes will be retransmitted should they get lost over the network. (Unreliable: Lost changes are not retransmitted) (Reliable: Lost changes are retransmitted)
> ```TS:Nada
> var ReliabilityMode : ReliabilityMode


---  
 #  ReplicateOnOffline : [boolean](../nada_base_types/boolean.md)

> Controls whether or not the net channel will be replicated when the net object goes offline. If enabled, all net channel property values are guaranteed to be set immediately before the NetObjectOffline event. (Cannot be modified at game runtime)
> ```TS:Nada
> var ReplicateOnOffline : Boolean


---  
 #  ReplicateOnOnline : [boolean](../nada_base_types/boolean.md)

> Controls whether or not the net channel will be replicated when the net object comes online. If enabled, all net channel property values are guaranteed to be set immediately before the NetObjectOnline event. (Cannot be modified at game runtime)
> ```TS:Nada
> var ReplicateOnOnline : Boolean


---  
 #  SerializationMode : [SerializationMode](../enum_reference.md#serializationmode)

> Controls how net channels are serialized. (All: Serialize all net properties) (Changed: Serialize only net properties that have changed, using bit flags in between) (Cannot be modified at game runtime)
> ```TS:Nada
> var SerializationMode : SerializationMode


---  
 #  TransferMode : [TransferMode](../enum_reference.md#transfermode)

> Controls how net channel changes are to be ordered and released once received. (Immediate: Changes are released immediately once received, including late changes) (Sequenced: Changes are released immediately once received, discarding late changes) (Ordered: Changes are released immediately once preceding late changes have been received; forces all changes to be sent reliably) (Cannot be modified at game runtime)
> ```TS:Nada
> var TransferMode : TransferMode


---  
 #  Methods


---  
 #  ResetConfig : Void

> Resets all configuration settings.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ResetConfig()
> ``` 


---  
 #  SetConfig : Void

> Sets all configuration settings according to the specified NetChannelConfig resource.
> |Name|Type|Description|
> |---|---|---|
> |netChannelConfig|[netchannelconfig](netchannelconfig.md)| |
> ```TS:Nada
> function SetConfig(netChannelConfig : NetChannelConfig)
> ``` 


---  
 

 
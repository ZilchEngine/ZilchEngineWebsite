 `Resource` `Networking`



(NOTE) Network Channel Configuration. Defines a configuration for the replication of a set of properties on the network.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ AcceptIncomingChanges](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannelconfig.md#acceptincomingchanges-ze)|[dataresource](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/dataresource.md)| |
| |[ AccurateTimestampOnChange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannelconfig.md#accuratetimestamponchang)| | |
| |[ AllowNapping](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannelconfig.md#allownapping-zilch-engine)| | |
| |[ AllowRelay](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannelconfig.md#allowrelay-zilch-engine-d)| | |
| |[ AuthorityDefault](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannelconfig.md#authoritydefault-zilch-en)| | |
| |[ AuthorityMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannelconfig.md#authoritymode-zilch-engin)| | |
| |[ AwakeDetectionInterval](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannelconfig.md#awakedetectioninterval-z)| | |
| |[ AwakeDuration](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannelconfig.md#awakeduration-zilch-engin)| | |
| |[ DetectionMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannelconfig.md#detectionmode-zilch-engin)| | |
| |[ DetectOutgoingChanges](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannelconfig.md#detectoutgoingchanges-ze)| | |
| |[ EventOnIncomingPropertyChange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannelconfig.md#eventonincomingpropertyc)| | |
| |[ EventOnOutgoingPropertyChange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannelconfig.md#eventonoutgoingpropertyc)| | |
| |[ NapDetectionInterval](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannelconfig.md#napdetectioninterval-zer)| | |
| |[ ReliabilityMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannelconfig.md#reliabilitymode-zilch-eng)| | |
| |[ ReplicateOnOffline](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannelconfig.md#replicateonoffline-zero)| | |
| |[ ReplicateOnOnline](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannelconfig.md#replicateononline-zilch-e)| | |
| |[ SerializationMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannelconfig.md#serializationmode-zilch-e)| | |
| |[ TransferMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannelconfig.md#transfermode-zilch-engine)| | |


 #  Properties


---  
 #  AcceptIncomingChanges : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Controls whether or not net channels should accept incoming changes.
> ``` lang=cpp, name=Nada
> var AcceptIncomingChanges : Boolean


---  
 #  AccurateTimestampOnChange : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Controls whether or not the net channel will serialize an accurate timestamp value when changed, or will instead accept an estimated timestamp value. (This setting may be overridden for net channels belonging to a specific net object by enabling the corresponding net object setting)
> ``` lang=cpp, name=Nada
> var AccurateTimestampOnChange : Boolean


---  
 #  AllowNapping : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Controls whether or not net channels may nap (perform change detection on longer intervals) if they haven't changed in a while.
> ``` lang=cpp, name=Nada
> var AllowNapping : Boolean


---  
 #  AllowRelay : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Controls whether or not net channels will have their changes immediately broadcast to all relevant, incidental peers (if any) once received. (Enabling this allows a server to automatically relay client authoritative changes to other clients, otherwise this must be done manually using NetChannel::ReplicateNow)
> ``` lang=cpp, name=Nada
> var AllowRelay : Boolean


---  
 #  AuthorityDefault : [Authority](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#authority)

> Controls which peer has the authority to observe and replicate property changes on each net channel by default. (Client: Indicates both the client and server are allowed to observe and replicate property changes) (Server: Indicates only the server is allowed to observe and replicate property changes) Only a single client, specified by NetObject::NetUserOwnerPeerId, may possess client authority at any given time. The server is still responsible for relaying contained property changes to other clients, but will not replicate contained property changes back to the authority client. However, the server is also still responsible for other replication commands (such as object creation/destruction), and these WILL be replicated to the authority client.
> ``` lang=cpp, name=Nada
> var AuthorityDefault : Authority


---  
 #  AuthorityMode : [AuthorityMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#authoritymode)

> Controls when net channels can modify their change authority. (Dynamic: Authority may be modified at any time, even after a net object is brought online) (Fixed: Authority may be modified only before a net object is brought online)
> ``` lang=cpp, name=Nada
> var AuthorityMode : AuthorityMode


---  
 #  AwakeDetectionInterval : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> Controls the frame interval in which awake net channels are observed for changes.
> ``` lang=cpp, name=Nada
> var AwakeDetectionInterval : Integer


---  
 #  AwakeDuration : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> Controls the frame duration following the last detected change in which net channels are considered actively changing and will be kept awake.
> ``` lang=cpp, name=Nada
> var AwakeDuration : Integer


---  
 #  DetectionMode : [DetectionMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#detectionmode)

> Controls how net channel changes are detected. (Assume: Assumes something has changed) (Manual: Detects changes manually using change flags) (Automatic: Detects changes automatically using comparisons) (Manumatic: Detects changes manually using change flags and automatically using comparisons)
> ``` lang=cpp, name=Nada
> var DetectionMode : DetectionMode


---  
 #  DetectOutgoingChanges : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Controls whether or not net channels should detect outgoing changes.
> ``` lang=cpp, name=Nada
> var DetectOutgoingChanges : Boolean


---  
 #  EventOnIncomingPropertyChange : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Controls whether or not net channels should dispatch NetChannelIncomingPropertyChange when an incoming net property change is accepted.
> ``` lang=cpp, name=Nada
> var EventOnIncomingPropertyChange : Boolean


---  
 #  EventOnOutgoingPropertyChange : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Controls whether or not net channels should dispatch NetChannelOutgoingPropertyChange when an outgoing net property change is detected.
> ``` lang=cpp, name=Nada
> var EventOnOutgoingPropertyChange : Boolean


---  
 #  NapDetectionInterval : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> Controls the frame interval in which napping net channels are observed for changes.
> ``` lang=cpp, name=Nada
> var NapDetectionInterval : Integer


---  
 #  ReliabilityMode : [ReliabilityMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#reliabilitymode)

> Controls whether or not net channel changes will be retransmitted should they get lost over the network. (Unreliable: Lost changes are not retransmitted) (Reliable: Lost changes are retransmitted)
> ``` lang=cpp, name=Nada
> var ReliabilityMode : ReliabilityMode


---  
 #  ReplicateOnOffline : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Controls whether or not the net channel will be replicated when the net object goes offline. If enabled, all net channel property values are guaranteed to be set immediately before the NetObjectOffline event.
> ``` lang=cpp, name=Nada
> var ReplicateOnOffline : Boolean


---  
 #  ReplicateOnOnline : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Controls whether or not the net channel will be replicated when the net object comes online. If enabled, all net channel property values are guaranteed to be set immediately before the NetObjectOnline event.
> ``` lang=cpp, name=Nada
> var ReplicateOnOnline : Boolean


---  
 #  SerializationMode : [SerializationMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#serializationmode)

> Controls how net channels are serialized. (All: Serialize all net properties) (Changed: Serialize only net properties that have changed, using bit flags in between)
> ``` lang=cpp, name=Nada
> var SerializationMode : SerializationMode


---  
 #  TransferMode : [TransferMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#transfermode)

> Controls how net channel changes are to be ordered and released once received. (Immediate: Changes are released immediately once received, including late changes) (Sequenced: Changes are released immediately once received, discarding late changes) (Ordered: Changes are released immediately once preceding late changes have been received; forces all changes to be sent reliably)
> ``` lang=cpp, name=Nada
> var TransferMode : TransferMode


---  
 #  Methods


---  
 

 
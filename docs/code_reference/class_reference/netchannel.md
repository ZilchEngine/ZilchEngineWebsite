 `Networking`



(NOTE) Network Channel. Manages the replication of a set of properties on the network.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetNetProperty](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannel.md#getnetproperty-zilch-engi)|[ Authority](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannel.md#authority-zilch-engine-do)|[safeid32object](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/safeid32object.md)| |
|[ HasNetProperty](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannel.md#hasnetproperty-zilch-engi)|[ ChangeFlag](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannel.md#changeflag-zilch-engine-d)| | |
|[ ReplicateNow](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannel.md#replicatenow-zilch-engine)|[ IsNapping](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannel.md#isnapping-zilch-engine-do)| | |
|[ TakeNap](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannel.md#takenap-void)|[ IsScheduled](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannel.md#isscheduled-zilch-engine)| | |
|[ WakeUp](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannel.md#wakeup-void)|[ LastChangeTimePassed](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannel.md#lastchangetimepassed-zer)| | |
| |[ LastChangeTimestamp](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannel.md#lastchangetimestamp-zero)| | |
| |[ Name](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannel.md#name-zilch-engine-documen)| | |
| |[ NetChannelType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannel.md#netchanneltype-zilch-engi)| | |


 #  Properties


---  
 #  Authority : [Authority](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#authority)

> Controls which peer has the authority to observe and replicate property changes. (Client: Indicates both the client and server are allowed to observe and replicate property changes) (Server: Indicates only the server is allowed to observe and replicate property changes) Only a single client, specified by NetObject::NetUserOwnerPeerId, may possess client authority at any given time. The server is still responsible for relaying contained property changes to other clients, but will not replicate contained property changes back to the authority client. However, the server is also still responsible for other replication commands (such as object creation/destruction), and these WILL be replicated to the authority client.
> ``` lang=cpp, name=Nada
> var Authority : Authority


---  
 #  ChangeFlag : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Manual change flag (checked upon manual change observation).
> ``` lang=cpp, name=Nada
> var ChangeFlag : Boolean


---  
 #  IsNapping : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> Returns true if the net channel is currently napping (performing change detection on longer intervals), else false.
> ``` lang=cpp, name=Nada
> var IsNapping : Boolean


---  
 #  IsScheduled : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> Returns true if this net channel is scheduled for change observation, else false.
> ``` lang=cpp, name=Nada
> var IsScheduled : Boolean


---  
 #  LastChangeTimePassed : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

 `read-only`

> Elapsed time passed since this net channel was last changed, else 0.
> ``` lang=cpp, name=Nada
> var LastChangeTimePassed : Real


---  
 #  LastChangeTimestamp : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

 `read-only`

> Timestamp indicating when this net channel was last changed, else 0.
> ``` lang=cpp, name=Nada
> var LastChangeTimestamp : Real


---  
 #  Name : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

 `read-only`

> Net channel name.
> ``` lang=cpp, name=Nada
> var Name : String


---  
 #  NetChannelType : [netchanneltype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchanneltype.md)

 `read-only`

> Operating net channel type.
> ``` lang=cpp, name=Nada
> var NetChannelType : NetChannelType


---  
 #  Methods


---  
 #  GetNetProperty : [netproperty](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netproperty.md)

> [Client/Server] Returns the specified net property, else nullptr.
> |Name|Type|Description|
> |---|---|---|
> |component|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)| |
> |propertyName|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function GetNetProperty(component : Component, propertyName : String) : NetProperty
> ``` 


---  
 #  HasNetProperty : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> [Client/Server] Returns true if the net object has the specified net property, else false.
> |Name|Type|Description|
> |---|---|---|
> |component|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)| |
> |propertyName|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function HasNetProperty(component : Component, propertyName : String) : Boolean
> ``` 


---  
 #  ReplicateNow : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Replicates net property changes immediately (only if changes are detected). Will also update nap state as configured. Returns true if changes were replicated, else false.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ReplicateNow() : Boolean
> ``` 


---  
 #  TakeNap : Void

> Forces the net channel to start napping immediately.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function TakeNap()
> ``` 


---  
 #  WakeUp : Void

> Forces the net channel to stop napping immediately.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function WakeUp()
> ``` 


---  
 

 
 `Networking`



(NOTE) Network Channel. Manages the replication of a set of properties on the network.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[GetNetProperty](netchannel.md#getnetproperty-zilch-engi)|[Authority](netchannel.md#authority-zilch-engine-do)|[safeid32object](safeid32object.md)| |
|[HasNetProperty](netchannel.md#hasnetproperty-zilch-engi)|[ChangeFlag](netchannel.md#changeflag-zilch-engine-d)| | |
|[ReplicateNow](netchannel.md#replicatenow-zilch-engine)|[IsNapping](netchannel.md#isnapping-zilch-engine-do)| | |
|[TakeNap](netchannel.md#takenap-void)|[IsScheduled](netchannel.md#isscheduled-zilch-engine)| | |
|[WakeUp](netchannel.md#wakeup-void)|[LastChangeTimePassed](netchannel.md#lastchangetimepassed-zer)| | |
| |[LastChangeTimestamp](netchannel.md#lastchangetimestamp-zero)| | |
| |[Name](netchannel.md#name-zilch-engine-documen)| | |
| |[NetChannelType](netchannel.md#netchanneltype-zilch-engi)| | |


 #  Properties


---  
 #  Authority : [Authority](../enum_reference.md#authority)

> Controls which peer has the authority to observe and replicate property changes. (Client: Indicates both the client and server are allowed to observe and replicate property changes) (Server: Indicates only the server is allowed to observe and replicate property changes) Only a single client, specified by NetObject::NetUserOwnerPeerId, may possess client authority at any given time. The server is still responsible for relaying contained property changes to other clients, but will not replicate contained property changes back to the authority client. However, the server is also still responsible for other replication commands (such as object creation/destruction), and these WILL be replicated to the authority client.
> ```TS:Nada
> var Authority : Authority


---  
 #  ChangeFlag : [boolean](../nada_base_types/boolean.md)

> Manual change flag (checked upon manual change observation).
> ```TS:Nada
> var ChangeFlag : Boolean


---  
 #  IsNapping : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Returns true if the net channel is currently napping (performing change detection on longer intervals), else false.
> ```TS:Nada
> var IsNapping : Boolean


---  
 #  IsScheduled : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Returns true if this net channel is scheduled for change observation, else false.
> ```TS:Nada
> var IsScheduled : Boolean


---  
 #  LastChangeTimePassed : [real](../nada_base_types/real.md)

 `read-only`

> Elapsed time passed since this net channel was last changed, else 0.
> ```TS:Nada
> var LastChangeTimePassed : Real


---  
 #  LastChangeTimestamp : [real](../nada_base_types/real.md)

 `read-only`

> Timestamp indicating when this net channel was last changed, else 0.
> ```TS:Nada
> var LastChangeTimestamp : Real


---  
 #  Name : [string](../nada_base_types/string.md)

 `read-only`

> Net channel name.
> ```TS:Nada
> var Name : String


---  
 #  NetChannelType : [netchanneltype](netchanneltype.md)

 `read-only`

> Operating net channel type.
> ```TS:Nada
> var NetChannelType : NetChannelType


---  
 #  Methods


---  
 #  GetNetProperty : [netproperty](netproperty.md)

> [Client/Server] Returns the specified net property, else nullptr.
> |Name|Type|Description|
> |---|---|---|
> |component|[component](component.md)| |
> |propertyName|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function GetNetProperty(component : Component, propertyName : String) : NetProperty
> ``` 


---  
 #  HasNetProperty : [boolean](../nada_base_types/boolean.md)

> [Client/Server] Returns true if the net object has the specified net property, else false.
> |Name|Type|Description|
> |---|---|---|
> |component|[component](component.md)| |
> |propertyName|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function HasNetProperty(component : Component, propertyName : String) : Boolean
> ``` 


---  
 #  ReplicateNow : [boolean](../nada_base_types/boolean.md)

> Replicates net property changes immediately (only if changes are detected). Will also update nap state as configured. Returns true if changes were replicated, else false.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ReplicateNow() : Boolean
> ``` 


---  
 #  TakeNap : Void

> Forces the net channel to start napping immediately.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function TakeNap()
> ``` 


---  
 #  WakeUp : Void

> Forces the net channel to stop napping immediately.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function WakeUp()
> ``` 


---  
 

 
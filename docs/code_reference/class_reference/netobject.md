 `Component` `Networking`



(NOTE) Network Object. Manages the replication of a single object on the network.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ DispatchBroadcast](netobject.md#dispatchbroadcast-void)|[ AcceptIncomingChanges](netobject.md#acceptincomingchanges-ze)|[component](component.md)|[netpeer](netpeer.md)|
|[ DispatchLocal](netobject.md#dispatchlocal-void)|[ AccurateTimestampOnChange](netobject.md#accuratetimestamponchang)| |[netspace](netspace.md)|
|[ DispatchLocalAndBroadcast](netobject.md#dispatchlocalandbroadcas)|[ AccurateTimestampOnOffline](netobject.md#accuratetimestamponoffli)| |[netuser](netuser.md)|
|[ DispatchLocalAndRemote](netobject.md#dispatchlocalandremote-v)|[ AccurateTimestampOnOnline](netobject.md#accuratetimestampononlin)| | |
|[ DispatchRemote](netobject.md#dispatchremote-void)|[ AllowNapping](netobject.md#allownapping-zilch-engine)| | |
|[ Forget](netobject.md#forget-zilch-engine-docum)|[ AutomaticChannel](netobject.md#automaticchannel-zilch-en)| | |
|[ GetNetChannel](netobject.md#getnetchannel-zilch-engin)|[ DetectOutgoingChanges](netobject.md#detectoutgoingchanges-ze)| | |
|[ HasNetChannel](netobject.md#hasnetchannel-zilch-engin)|[ IsClient](netobject.md#isclient-zilch-engine-doc)| | |
|[ IsOwnedByPeer](netobject.md#isownedbypeer-zilch-engin)|[ IsClientAndMine](netobject.md#isclientandmine-zilch-eng)| | |
|[ IsOwnedByUser](netobject.md#isownedbyuser-zilch-engin)|[ IsClientButNotMine](netobject.md#isclientbutnotmine-zero)| | |
|[ Constructor](netobject.md#netobject-void)|[ IsClientOrOffline](netobject.md#isclientoroffline-zilch-e)| | |
|[ ReplicateNow](netobject.md#replicatenow-zilch-engine)|[ IsClientOrServer](netobject.md#isclientorserver-zilch-en)| | |
|[ SelectRemote](netobject.md#selectremote-zilch-engine)|[ IsMine](netobject.md#ismine-zilch-engine-docum)| | |
|[ SetNetUserOwnerDown](netobject.md#setnetuserownerdown-void)|[ IsNapping](netobject.md#isnapping-zilch-engine-do)| | |
|[ SetNetUserOwnerUp](netobject.md#setnetuserownerup-void)|[ IsNotMine](netobject.md#isnotmine-zilch-engine-do)| | |
|[ TakeNap](netobject.md#takenap-void)|[ IsNotOwnedByAUser](netobject.md#isnotownedbyauser-zilch-e)| | |
|[ WakeUp](netobject.md#wakeup-void)|[ IsOffline](netobject.md#isoffline-zilch-engine-do)| | |
| |[ IsOfflineAndMine](netobject.md#isofflineandmine-zilch-en)| | |
| |[ IsOfflineButNotMine](netobject.md#isofflinebutnotmine-zero)| | |
| |[ IsOnline](netobject.md#isonline-zilch-engine-doc)| | |
| |[ IsOwnedByAUser](netobject.md#isownedbyauser-zilch-engi)| | |
| |[ IsServer](netobject.md#isserver-zilch-engine-doc)| | |
| |[ IsServerAndMine](netobject.md#isserverandmine-zilch-eng)| | |
| |[ IsServerButNotMine](netobject.md#isserverbutnotmine-zero)| | |
| |[ IsServerOrOffline](netobject.md#isserveroroffline-zilch-e)| | |
| |[ LastChangeTimePassed](netobject.md#lastchangetimepassed-zer)| | |
| |[ LastChangeTimestamp](netobject.md#lastchangetimestamp-zero)| | |
| |[ NetObjectId](netobject.md#netobjectid-zilch-engine)| | |
| |[ NetPropertyInfos](netobject.md#netpropertyinfos-zilch-en)| | |
| |[ NetUserOwner](netobject.md#netuserowner-zilch-engine)| | |
| |[ NetUserOwnerPath](netobject.md#netuserownerpath-zilch-en)| | |
| |[ NetUserOwnerPeerId](netobject.md#netuserownerpeerid-zero)| | |
| |[ NetUserOwnerUserId](netobject.md#netuserowneruserid-zero)| | |
| |[ OfflineTimePassed](netobject.md#offlinetimepassed-zilch-e)| | |
| |[ OfflineTimestamp](netobject.md#offlinetimestamp-zilch-en)| | |
| |[ OnlineTimePassed](netobject.md#onlinetimepassed-zilch-en)| | |
| |[ OnlineTimestamp](netobject.md#onlinetimestamp-zilch-eng)| | |
| |[ Role](netobject.md#role-zilch-engine-documen)| | |


 #  Properties


---  
 #  AcceptIncomingChanges : [boolean](../nada_base_types/boolean.md)

> Controls whether or not net channels on this net object may accept incoming changes.
> ``` lang=cpp, name=Nada
> var AcceptIncomingChanges : Boolean


---  
 #  AccurateTimestampOnChange : [boolean](../nada_base_types/boolean.md)

> Controls whether or not the net object will serialize an accurate timestamp value when changed (on any net channel), or will instead accept an estimated timestamp value. (Enabling this will override the corresponding net channel type setting for all net channels added to this net object)
> ``` lang=cpp, name=Nada
> var AccurateTimestampOnChange : Boolean


---  
 #  AccurateTimestampOnOffline : [boolean](../nada_base_types/boolean.md)

> Controls whether or not the net object will serialize an accurate timestamp value when taken offline, or will instead accept an estimated timestamp value.
> ``` lang=cpp, name=Nada
> var AccurateTimestampOnOffline : Boolean


---  
 #  AccurateTimestampOnOnline : [boolean](../nada_base_types/boolean.md)

> Controls whether or not the net object will serialize an accurate timestamp value when brought online, or will instead accept an estimated timestamp value.
> ``` lang=cpp, name=Nada
> var AccurateTimestampOnOnline : Boolean


---  
 #  AllowNapping : [boolean](../nada_base_types/boolean.md)

> Controls whether or not net channels on this net object may nap (perform change detection on longer intervals) if they haven't changed in a while.
> ``` lang=cpp, name=Nada
> var AllowNapping : Boolean


---  
 #  AutomaticChannel : [netchannelconfig](netchannelconfig.md)

> Returns the automatic net channel configuration resource (assigned to net properties unless another channel is specified).
> ``` lang=cpp, name=Nada
> var AutomaticChannel : NetChannelConfig


---  
 #  DetectOutgoingChanges : [boolean](../nada_base_types/boolean.md)

> Controls whether or not net channels on this net object may detect outgoing changes.
> ``` lang=cpp, name=Nada
> var DetectOutgoingChanges : Boolean


---  
 #  IsClient : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is client, else false.
> ``` lang=cpp, name=Nada
> var IsClient : Boolean


---  
 #  IsClientAndMine : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is client and the net object is conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Nada
> var IsClientAndMine : Boolean


---  
 #  IsClientButNotMine : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is client and the net object is not conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Nada
> var IsClientButNotMine : Boolean


---  
 #  IsClientOrOffline : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is client or offline, else false.
> ``` lang=cpp, name=Nada
> var IsClientOrOffline : Boolean


---  
 #  IsClientOrServer : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is client or server, else false.
> ``` lang=cpp, name=Nada
> var IsClientOrServer : Boolean


---  
 #  IsMine : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Returns true if the net object is conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Nada
> var IsMine : Boolean


---  
 #  IsNapping : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Returns true if all net channels on this net object are napping (performing change detection on longer intervals), else false.
> ``` lang=cpp, name=Nada
> var IsNapping : Boolean


---  
 #  IsNotMine : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Returns true if the net object is not conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Nada
> var IsNotMine : Boolean


---  
 #  IsNotOwnedByAUser : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Returns true if the net object is not conceptually owned by a user, else false.
> ``` lang=cpp, name=Nada
> var IsNotOwnedByAUser : Boolean


---  
 #  IsOffline : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is offline, else false.
> ``` lang=cpp, name=Nada
> var IsOffline : Boolean


---  
 #  IsOfflineAndMine : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is offline and the net object is conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Nada
> var IsOfflineAndMine : Boolean


---  
 #  IsOfflineButNotMine : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is offline and the net object is not conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Nada
> var IsOfflineButNotMine : Boolean


---  
 #  IsOnline : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Returns true if the net object is online, else false.
> ``` lang=cpp, name=Nada
> var IsOnline : Boolean


---  
 #  IsOwnedByAUser : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Returns true if the net object is conceptually owned by a user, else false.
> ``` lang=cpp, name=Nada
> var IsOwnedByAUser : Boolean


---  
 #  IsServer : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is server, else false.
> ``` lang=cpp, name=Nada
> var IsServer : Boolean


---  
 #  IsServerAndMine : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is server and the net object is conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Nada
> var IsServerAndMine : Boolean


---  
 #  IsServerButNotMine : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is server and the net object is not conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Nada
> var IsServerButNotMine : Boolean


---  
 #  IsServerOrOffline : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is server or offline, else false.
> ``` lang=cpp, name=Nada
> var IsServerOrOffline : Boolean


---  
 #  LastChangeTimePassed : [real](../nada_base_types/real.md)

 `read-only`

> Elapsed time passed since this net object was last changed, else 0.
> ``` lang=cpp, name=Nada
> var LastChangeTimePassed : Real


---  
 #  LastChangeTimestamp : [real](../nada_base_types/real.md)

 `read-only`

> Timestamp indicating when this net object was last changed, else 0.
> ``` lang=cpp, name=Nada
> var LastChangeTimestamp : Real


---  
 #  NetObjectId : [integer](../nada_base_types/integer.md)

 `read-only`

> Returns the net object ID (set if the net object is live), else 0.
> ``` lang=cpp, name=Nada
> var NetObjectId : Integer


---  
 #  NetPropertyInfos : [netpropertyinfos](netpropertyinfos.md)

> Net property infos added through the property grid.
> ``` lang=cpp, name=Nada
> var NetPropertyInfos : NetPropertyInfos


---  
 #  NetUserOwner : [cog](cog.md)

> Returns the network user this object conceptually belongs to, else nullptr.
> ``` lang=cpp, name=Nada
> var NetUserOwner : Cog


---  
 #  NetUserOwnerPath : [cogpath](cogpath.md)

 `read-only`

> Path to the network user this object conceptually belongs to, else empty cog path.
> ``` lang=cpp, name=Nada
> var NetUserOwnerPath : CogPath


---  
 #  NetUserOwnerPeerId : [integer](../nada_base_types/integer.md)

 `read-only`

> Returns the network peer identifier of the peer who added the user this object conceptually belongs to, else 0.
> ``` lang=cpp, name=Nada
> var NetUserOwnerPeerId : Integer


---  
 #  NetUserOwnerUserId : [integer](../nada_base_types/integer.md)

 `read-only`

> Returns the network user identifier of the user this object conceptually belongs to, else 0.
> ``` lang=cpp, name=Nada
> var NetUserOwnerUserId : Integer


---  
 #  OfflineTimePassed : [real](../nada_base_types/real.md)

 `read-only`

> Elapsed time passed since this net object was taken offline, else 0.
> ``` lang=cpp, name=Nada
> var OfflineTimePassed : Real


---  
 #  OfflineTimestamp : [real](../nada_base_types/real.md)

 `read-only`

> Timestamp indicating when this net object was taken offline, else 0.
> ``` lang=cpp, name=Nada
> var OfflineTimestamp : Real


---  
 #  OnlineTimePassed : [real](../nada_base_types/real.md)

 `read-only`

> Elapsed time passed since this net object was brought online, else 0.
> ``` lang=cpp, name=Nada
> var OnlineTimePassed : Real


---  
 #  OnlineTimestamp : [real](../nada_base_types/real.md)

 `read-only`

> Timestamp indicating when this net object was brought online, else 0.
> ``` lang=cpp, name=Nada
> var OnlineTimestamp : Real


---  
 #  Role : [NetRole](../enum_reference.md#netrole)

 `read-only`

> Returns our open peer's network role (client, server, offline), else Role::Unspecified.
> ``` lang=cpp, name=Nada
> var Role : NetRole


---  
 #  Methods


---  
 #  DispatchBroadcast : Void

> Dispatches the net event on the net object for all remote peers. In Offline mode, this calls DispatchLocal only.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](../nada_base_types/string.md)| |
> |event|[event](event.md)| |
> ``` lang=cpp, name=Nada
> function DispatchBroadcast(eventId : String, event : Event)
> ``` 


---  
 #  DispatchLocal : Void

> Dispatches the net event on the net object for the local peer.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](../nada_base_types/string.md)| |
> |event|[event](event.md)| |
> ``` lang=cpp, name=Nada
> function DispatchLocal(eventId : String, event : Event)
> ``` 


---  
 #  DispatchLocalAndBroadcast : Void

> Dispatches the net event on the net object for the local peer and for all remote peers. In Offline mode, this calls DispatchLocal only.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](../nada_base_types/string.md)| |
> |event|[event](event.md)| |
> ``` lang=cpp, name=Nada
> function DispatchLocalAndBroadcast(eventId : String, event : Event)
> ``` 


---  
 #  DispatchLocalAndRemote : Void

> Dispatches the net event on the net object for the local peer and for the remote peer. In Offline mode, this calls DispatchLocal only.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](../nada_base_types/string.md)| |
> |event|[event](event.md)| |
> |netPeerId|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function DispatchLocalAndRemote(eventId : String, event : Event, netPeerId : Integer)
> ``` 


---  
 #  DispatchRemote : Void

> Dispatches the net event on the net object for the remote peer. In Offline mode, this calls DispatchLocal only.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](../nada_base_types/string.md)| |
> |event|[event](event.md)| |
> |netPeerId|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function DispatchRemote(eventId : String, event : Event, netPeerId : Integer)
> ``` 


---  
 #  Forget : [boolean](../nada_base_types/boolean.md)

> [Client] Forgets the online net object locally. [Server] Forgets the online net object locally and remotely for all relevant peers. Effectively removes the net object from the network system without destroying it. Returns true if successful, else false.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Forget() : Boolean
> ``` 


---  
 #  GetNetChannel : [netchannel](netchannel.md)

> [Client/Server] Returns the specified net channel, else nullptr.
> |Name|Type|Description|
> |---|---|---|
> |netChannelName|[string](../nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function GetNetChannel(netChannelName : String) : NetChannel
> ``` 


---  
 #  HasNetChannel : [boolean](../nada_base_types/boolean.md)

> [Client/Server] Returns true if the net object has the specified net channel, else false.
> |Name|Type|Description|
> |---|---|---|
> |netChannelName|[string](../nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function HasNetChannel(netChannelName : String) : Boolean
> ``` 


---  
 #  IsOwnedByPeer : [boolean](../nada_base_types/boolean.md)

> Returns true if the net object is conceptually owned by a user added by the specified peer, else false.
> |Name|Type|Description|
> |---|---|---|
> |netPeerId|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function IsOwnedByPeer(netPeerId : Integer) : Boolean
> ``` 


---  
 #  IsOwnedByUser : [boolean](../nada_base_types/boolean.md)

> Returns true if the net object is conceptually owned by the specified user, else false.
> |Name|Type|Description|
> |---|---|---|
> |cog|[cog](cog.md)| |
> ``` lang=cpp, name=Nada
> function IsOwnedByUser(cog : Cog) : Boolean
> ``` 


---  
 #  NetObject : Void

 `constructor`

> Constructor.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function NetObject()
> ``` 


---  
 #  ReplicateNow : [boolean](../nada_base_types/boolean.md)

> [Client/Server] Replicates all net channels' property changes immediately (only where changes are detected). Will also update nap state as configured. Returns true if changes were replicated, else false.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ReplicateNow() : Boolean
> ``` 


---  
 #  SelectRemote : [boolean](../nada_base_types/boolean.md)

> [Client/Server] Selects the remote net object on the first opposite-role peer found running in another game session instance on the engine. Will fail if the net object is not online, or not found remotely. Returns true if successful, else false.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function SelectRemote() : Boolean
> ``` 


---  
 #  SetNetUserOwnerDown : Void

> [Server/Offline] Sets the owning network user on this object and down the tree on all children recursively (pre-order traversal).
> |Name|Type|Description|
> |---|---|---|
> |cog|[cog](cog.md)| |
> ``` lang=cpp, name=Nada
> function SetNetUserOwnerDown(cog : Cog)
> ``` 


---  
 #  SetNetUserOwnerUp : Void

> [Server/Offline] Sets the owning network user on this object and up the tree on each parent recursively (pre-order traversal).
> |Name|Type|Description|
> |---|---|---|
> |cog|[cog](cog.md)| |
> ``` lang=cpp, name=Nada
> function SetNetUserOwnerUp(cog : Cog)
> ``` 


---  
 #  TakeNap : Void

> Forces all net channels on this net object to start napping immediately.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function TakeNap()
> ``` 


---  
 #  WakeUp : Void

> Forces all net channels on this net object to stop napping immediately.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function WakeUp()
> ``` 


---  
 

 
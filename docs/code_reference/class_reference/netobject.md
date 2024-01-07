 `Component` `Networking`



(NOTE) Network Object. Manages the replication of a single object on the network.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ DispatchBroadcast](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#dispatchbroadcast-void)|[ AcceptIncomingChanges](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#acceptincomingchanges-ze)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)|[netpeer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpeer.md)|
|[ DispatchLocal](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#dispatchlocal-void)|[ AccurateTimestampOnChange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#accuratetimestamponchang)| |[netspace](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netspace.md)|
|[ DispatchLocalAndBroadcast](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#dispatchlocalandbroadcas)|[ AccurateTimestampOnOffline](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#accuratetimestamponoffli)| |[netuser](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netuser.md)|
|[ DispatchLocalAndRemote](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#dispatchlocalandremote-v)|[ AccurateTimestampOnOnline](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#accuratetimestampononlin)| | |
|[ DispatchRemote](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#dispatchremote-void)|[ AllowNapping](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#allownapping-zilch-engine)| | |
|[ Forget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#forget-zilch-engine-docum)|[ AutomaticChannel](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#automaticchannel-zilch-en)| | |
|[ GetNetChannel](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#getnetchannel-zilch-engin)|[ DetectOutgoingChanges](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#detectoutgoingchanges-ze)| | |
|[ HasNetChannel](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#hasnetchannel-zilch-engin)|[ IsClient](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#isclient-zilch-engine-doc)| | |
|[ IsOwnedByPeer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#isownedbypeer-zilch-engin)|[ IsClientAndMine](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#isclientandmine-zilch-eng)| | |
|[ IsOwnedByUser](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#isownedbyuser-zilch-engin)|[ IsClientButNotMine](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#isclientbutnotmine-zero)| | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#netobject-void)|[ IsClientOrOffline](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#isclientoroffline-zilch-e)| | |
|[ ReplicateNow](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#replicatenow-zilch-engine)|[ IsClientOrServer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#isclientorserver-zilch-en)| | |
|[ SelectRemote](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#selectremote-zilch-engine)|[ IsMine](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#ismine-zilch-engine-docum)| | |
|[ SetNetUserOwnerDown](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#setnetuserownerdown-void)|[ IsNapping](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#isnapping-zilch-engine-do)| | |
|[ SetNetUserOwnerUp](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#setnetuserownerup-void)|[ IsNotMine](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#isnotmine-zilch-engine-do)| | |
|[ TakeNap](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#takenap-void)|[ IsNotOwnedByAUser](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#isnotownedbyauser-zilch-e)| | |
|[ WakeUp](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#wakeup-void)|[ IsOffline](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#isoffline-zilch-engine-do)| | |
| |[ IsOfflineAndMine](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#isofflineandmine-zilch-en)| | |
| |[ IsOfflineButNotMine](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#isofflinebutnotmine-zero)| | |
| |[ IsOnline](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#isonline-zilch-engine-doc)| | |
| |[ IsOwnedByAUser](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#isownedbyauser-zilch-engi)| | |
| |[ IsServer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#isserver-zilch-engine-doc)| | |
| |[ IsServerAndMine](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#isserverandmine-zilch-eng)| | |
| |[ IsServerButNotMine](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#isserverbutnotmine-zero)| | |
| |[ IsServerOrOffline](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#isserveroroffline-zilch-e)| | |
| |[ LastChangeTimePassed](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#lastchangetimepassed-zer)| | |
| |[ LastChangeTimestamp](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#lastchangetimestamp-zero)| | |
| |[ NetObjectId](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#netobjectid-zilch-engine)| | |
| |[ NetPropertyInfos](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#netpropertyinfos-zilch-en)| | |
| |[ NetUserOwner](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#netuserowner-zilch-engine)| | |
| |[ NetUserOwnerPath](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#netuserownerpath-zilch-en)| | |
| |[ NetUserOwnerPeerId](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#netuserownerpeerid-zero)| | |
| |[ NetUserOwnerUserId](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#netuserowneruserid-zero)| | |
| |[ OfflineTimePassed](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#offlinetimepassed-zilch-e)| | |
| |[ OfflineTimestamp](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#offlinetimestamp-zilch-en)| | |
| |[ OnlineTimePassed](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#onlinetimepassed-zilch-en)| | |
| |[ OnlineTimestamp](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#onlinetimestamp-zilch-eng)| | |
| |[ Role](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md#role-zilch-engine-documen)| | |


 #  Properties


---  
 #  AcceptIncomingChanges : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Controls whether or not net channels on this net object may accept incoming changes.
> ``` lang=cpp, name=Nada
> var AcceptIncomingChanges : Boolean


---  
 #  AccurateTimestampOnChange : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Controls whether or not the net object will serialize an accurate timestamp value when changed (on any net channel), or will instead accept an estimated timestamp value. (Enabling this will override the corresponding net channel type setting for all net channels added to this net object)
> ``` lang=cpp, name=Nada
> var AccurateTimestampOnChange : Boolean


---  
 #  AccurateTimestampOnOffline : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Controls whether or not the net object will serialize an accurate timestamp value when taken offline, or will instead accept an estimated timestamp value.
> ``` lang=cpp, name=Nada
> var AccurateTimestampOnOffline : Boolean


---  
 #  AccurateTimestampOnOnline : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Controls whether or not the net object will serialize an accurate timestamp value when brought online, or will instead accept an estimated timestamp value.
> ``` lang=cpp, name=Nada
> var AccurateTimestampOnOnline : Boolean


---  
 #  AllowNapping : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Controls whether or not net channels on this net object may nap (perform change detection on longer intervals) if they haven't changed in a while.
> ``` lang=cpp, name=Nada
> var AllowNapping : Boolean


---  
 #  AutomaticChannel : [netchannelconfig](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannelconfig.md)

> Returns the automatic net channel configuration resource (assigned to net properties unless another channel is specified).
> ``` lang=cpp, name=Nada
> var AutomaticChannel : NetChannelConfig


---  
 #  DetectOutgoingChanges : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Controls whether or not net channels on this net object may detect outgoing changes.
> ``` lang=cpp, name=Nada
> var DetectOutgoingChanges : Boolean


---  
 #  IsClient : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is client, else false.
> ``` lang=cpp, name=Nada
> var IsClient : Boolean


---  
 #  IsClientAndMine : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is client and the net object is conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Nada
> var IsClientAndMine : Boolean


---  
 #  IsClientButNotMine : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is client and the net object is not conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Nada
> var IsClientButNotMine : Boolean


---  
 #  IsClientOrOffline : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is client or offline, else false.
> ``` lang=cpp, name=Nada
> var IsClientOrOffline : Boolean


---  
 #  IsClientOrServer : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is client or server, else false.
> ``` lang=cpp, name=Nada
> var IsClientOrServer : Boolean


---  
 #  IsMine : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> Returns true if the net object is conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Nada
> var IsMine : Boolean


---  
 #  IsNapping : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> Returns true if all net channels on this net object are napping (performing change detection on longer intervals), else false.
> ``` lang=cpp, name=Nada
> var IsNapping : Boolean


---  
 #  IsNotMine : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> Returns true if the net object is not conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Nada
> var IsNotMine : Boolean


---  
 #  IsNotOwnedByAUser : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> Returns true if the net object is not conceptually owned by a user, else false.
> ``` lang=cpp, name=Nada
> var IsNotOwnedByAUser : Boolean


---  
 #  IsOffline : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is offline, else false.
> ``` lang=cpp, name=Nada
> var IsOffline : Boolean


---  
 #  IsOfflineAndMine : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is offline and the net object is conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Nada
> var IsOfflineAndMine : Boolean


---  
 #  IsOfflineButNotMine : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is offline and the net object is not conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Nada
> var IsOfflineButNotMine : Boolean


---  
 #  IsOnline : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> Returns true if the net object is online, else false.
> ``` lang=cpp, name=Nada
> var IsOnline : Boolean


---  
 #  IsOwnedByAUser : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> Returns true if the net object is conceptually owned by a user, else false.
> ``` lang=cpp, name=Nada
> var IsOwnedByAUser : Boolean


---  
 #  IsServer : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is server, else false.
> ``` lang=cpp, name=Nada
> var IsServer : Boolean


---  
 #  IsServerAndMine : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is server and the net object is conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Nada
> var IsServerAndMine : Boolean


---  
 #  IsServerButNotMine : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is server and the net object is not conceptually owned by a user added by our local peer, else false.
> ``` lang=cpp, name=Nada
> var IsServerButNotMine : Boolean


---  
 #  IsServerOrOffline : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> Returns true if our open peer's network role is server or offline, else false.
> ``` lang=cpp, name=Nada
> var IsServerOrOffline : Boolean


---  
 #  LastChangeTimePassed : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

 `read-only`

> Elapsed time passed since this net object was last changed, else 0.
> ``` lang=cpp, name=Nada
> var LastChangeTimePassed : Real


---  
 #  LastChangeTimestamp : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

 `read-only`

> Timestamp indicating when this net object was last changed, else 0.
> ``` lang=cpp, name=Nada
> var LastChangeTimestamp : Real


---  
 #  NetObjectId : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Returns the net object ID (set if the net object is live), else 0.
> ``` lang=cpp, name=Nada
> var NetObjectId : Integer


---  
 #  NetPropertyInfos : [netpropertyinfos](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpropertyinfos.md)

> Net property infos added through the property grid.
> ``` lang=cpp, name=Nada
> var NetPropertyInfos : NetPropertyInfos


---  
 #  NetUserOwner : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Returns the network user this object conceptually belongs to, else nullptr.
> ``` lang=cpp, name=Nada
> var NetUserOwner : Cog


---  
 #  NetUserOwnerPath : [cogpath](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cogpath.md)

 `read-only`

> Path to the network user this object conceptually belongs to, else empty cog path.
> ``` lang=cpp, name=Nada
> var NetUserOwnerPath : CogPath


---  
 #  NetUserOwnerPeerId : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Returns the network peer identifier of the peer who added the user this object conceptually belongs to, else 0.
> ``` lang=cpp, name=Nada
> var NetUserOwnerPeerId : Integer


---  
 #  NetUserOwnerUserId : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Returns the network user identifier of the user this object conceptually belongs to, else 0.
> ``` lang=cpp, name=Nada
> var NetUserOwnerUserId : Integer


---  
 #  OfflineTimePassed : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

 `read-only`

> Elapsed time passed since this net object was taken offline, else 0.
> ``` lang=cpp, name=Nada
> var OfflineTimePassed : Real


---  
 #  OfflineTimestamp : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

 `read-only`

> Timestamp indicating when this net object was taken offline, else 0.
> ``` lang=cpp, name=Nada
> var OfflineTimestamp : Real


---  
 #  OnlineTimePassed : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

 `read-only`

> Elapsed time passed since this net object was brought online, else 0.
> ``` lang=cpp, name=Nada
> var OnlineTimePassed : Real


---  
 #  OnlineTimestamp : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

 `read-only`

> Timestamp indicating when this net object was brought online, else 0.
> ``` lang=cpp, name=Nada
> var OnlineTimestamp : Real


---  
 #  Role : [NetRole](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#netrole)

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
> |eventId|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |event|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
> ``` lang=cpp, name=Nada
> function DispatchBroadcast(eventId : String, event : Event)
> ``` 


---  
 #  DispatchLocal : Void

> Dispatches the net event on the net object for the local peer.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |event|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
> ``` lang=cpp, name=Nada
> function DispatchLocal(eventId : String, event : Event)
> ``` 


---  
 #  DispatchLocalAndBroadcast : Void

> Dispatches the net event on the net object for the local peer and for all remote peers. In Offline mode, this calls DispatchLocal only.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |event|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
> ``` lang=cpp, name=Nada
> function DispatchLocalAndBroadcast(eventId : String, event : Event)
> ``` 


---  
 #  DispatchLocalAndRemote : Void

> Dispatches the net event on the net object for the local peer and for the remote peer. In Offline mode, this calls DispatchLocal only.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |event|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
> |netPeerId|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function DispatchLocalAndRemote(eventId : String, event : Event, netPeerId : Integer)
> ``` 


---  
 #  DispatchRemote : Void

> Dispatches the net event on the net object for the remote peer. In Offline mode, this calls DispatchLocal only.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |event|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
> |netPeerId|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function DispatchRemote(eventId : String, event : Event, netPeerId : Integer)
> ``` 


---  
 #  Forget : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> [Client] Forgets the online net object locally. [Server] Forgets the online net object locally and remotely for all relevant peers. Effectively removes the net object from the network system without destroying it. Returns true if successful, else false.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Forget() : Boolean
> ``` 


---  
 #  GetNetChannel : [netchannel](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannel.md)

> [Client/Server] Returns the specified net channel, else nullptr.
> |Name|Type|Description|
> |---|---|---|
> |netChannelName|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function GetNetChannel(netChannelName : String) : NetChannel
> ``` 


---  
 #  HasNetChannel : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> [Client/Server] Returns true if the net object has the specified net channel, else false.
> |Name|Type|Description|
> |---|---|---|
> |netChannelName|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function HasNetChannel(netChannelName : String) : Boolean
> ``` 


---  
 #  IsOwnedByPeer : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Returns true if the net object is conceptually owned by a user added by the specified peer, else false.
> |Name|Type|Description|
> |---|---|---|
> |netPeerId|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function IsOwnedByPeer(netPeerId : Integer) : Boolean
> ``` 


---  
 #  IsOwnedByUser : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Returns true if the net object is conceptually owned by the specified user, else false.
> |Name|Type|Description|
> |---|---|---|
> |cog|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
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
 #  ReplicateNow : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> [Client/Server] Replicates all net channels' property changes immediately (only where changes are detected). Will also update nap state as configured. Returns true if changes were replicated, else false.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ReplicateNow() : Boolean
> ``` 


---  
 #  SelectRemote : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

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
> |cog|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Nada
> function SetNetUserOwnerDown(cog : Cog)
> ``` 


---  
 #  SetNetUserOwnerUp : Void

> [Server/Offline] Sets the owning network user on this object and up the tree on each parent recursively (pre-order traversal).
> |Name|Type|Description|
> |---|---|---|
> |cog|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
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
 

 
 `Component` `Networking`



(NOTE) Network User. Manages the replication of a single negotiated user on the network.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddedByPeer](netuser.md#addedbypeer-zilch-engine)|[ AddedByMyPeer](netuser.md#addedbymypeer-zilch-engin)|[netobject](netobject.md)| |
|[ FindOwnedNetObjectByName](netuser.md#findownednetobjectbyname)|[ NetPeerId](netuser.md#netpeerid-zilch-engine-do)| | |
|[ FindOwnedNetObjectByNameInSpace](netuser.md#findownednetobjectbyname)|[ NetUserId](netuser.md#netuserid-zilch-engine-do)| | |
|[ Constructor](netuser.md#netuser-void)|[ OwnedNetObjectCount](netuser.md#ownednetobjectcount-zero)| | |
|[ ReleaseOwnedNetObjects](netuser.md#releaseownednetobjects-v)|[ OwnedNetObjects](netuser.md#ownednetobjects-zilch-eng)| | |


 #  Properties


---  
 #  AddedByMyPeer : [boolean](../nada_base_types/boolean.md)

 `read-only`

> 
> ```TS:Nada
> var AddedByMyPeer : Boolean


---  
 #  NetPeerId : [integer](../nada_base_types/integer.md)

 `read-only`

> Adding network peer identifier.
> ```TS:Nada
> var NetPeerId : Integer


---  
 #  NetUserId : [integer](../nada_base_types/integer.md)

 `read-only`

> Network user identifier.
> ```TS:Nada
> var NetUserId : Integer


---  
 #  OwnedNetObjectCount : [integer](../nada_base_types/integer.md)

 `read-only`

> Returns the number of net objects owned by this user in all spaces.
> ```TS:Nada
> var OwnedNetObjectCount : Integer


---  
 #  OwnedNetObjects : [coghashsetrange](coghashsetrange.md)

 `read-only`

> Returns all net objects owned by this user in all spaces.
> ```TS:Nada
> var OwnedNetObjects : CogHashSetRange


---  
 #  Methods


---  
 #  AddedByPeer : [boolean](../nada_base_types/boolean.md)

> Returns true if the user was added by the specified peer, else false.
> |Name|Type|Description|
> |---|---|---|
> |netPeerId|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function AddedByPeer(netPeerId : Integer) : Boolean
> ``` 


---  
 #  FindOwnedNetObjectByName : [cog](cog.md)

> Finds a net object with the given name owned by this user in any space, else nullptr.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function FindOwnedNetObjectByName(name : String) : Cog
> ``` 


---  
 #  FindOwnedNetObjectByNameInSpace : [cog](cog.md)

> Finds a net object with the given name owned by this user in the specified space, else nullptr.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> |space|[space](space.md)| |
> ```TS:Nada
> function FindOwnedNetObjectByNameInSpace(name : String, space : Space) : Cog
> ``` 


---  
 #  NetUser : Void

 `constructor`

> Constructor.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function NetUser()
> ``` 


---  
 #  ReleaseOwnedNetObjects : Void

> [Server/Offline] Releases ownership of all net objects owned by this user in all spaces.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ReleaseOwnedNetObjects()
> ``` 


---  
 

 
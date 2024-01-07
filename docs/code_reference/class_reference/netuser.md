 `Component` `Networking`



(NOTE) Network User. Manages the replication of a single negotiated user on the network.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddedByPeer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netuser.md#addedbypeer-zilch-engine)|[ AddedByMyPeer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netuser.md#addedbymypeer-zilch-engin)|[netobject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netobject.md)| |
|[ FindOwnedNetObjectByName](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netuser.md#findownednetobjectbyname)|[ NetPeerId](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netuser.md#netpeerid-zilch-engine-do)| | |
|[ FindOwnedNetObjectByNameInSpace](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netuser.md#findownednetobjectbyname)|[ NetUserId](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netuser.md#netuserid-zilch-engine-do)| | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netuser.md#netuser-void)|[ OwnedNetObjectCount](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netuser.md#ownednetobjectcount-zero)| | |
|[ ReleaseOwnedNetObjects](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netuser.md#releaseownednetobjects-v)|[ OwnedNetObjects](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netuser.md#ownednetobjects-zilch-eng)| | |


 #  Properties


---  
 #  AddedByMyPeer : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var AddedByMyPeer : Boolean


---  
 #  NetPeerId : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Adding network peer identifier.
> ``` lang=cpp, name=Nada
> var NetPeerId : Integer


---  
 #  NetUserId : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Network user identifier.
> ``` lang=cpp, name=Nada
> var NetUserId : Integer


---  
 #  OwnedNetObjectCount : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Returns the number of net objects owned by this user in all spaces.
> ``` lang=cpp, name=Nada
> var OwnedNetObjectCount : Integer


---  
 #  OwnedNetObjects : [coghashsetrange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/coghashsetrange.md)

 `read-only`

> Returns all net objects owned by this user in all spaces.
> ``` lang=cpp, name=Nada
> var OwnedNetObjects : CogHashSetRange


---  
 #  Methods


---  
 #  AddedByPeer : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Returns true if the user was added by the specified peer, else false.
> |Name|Type|Description|
> |---|---|---|
> |netPeerId|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function AddedByPeer(netPeerId : Integer) : Boolean
> ``` 


---  
 #  FindOwnedNetObjectByName : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Finds a net object with the given name owned by this user in any space, else nullptr.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function FindOwnedNetObjectByName(name : String) : Cog
> ``` 


---  
 #  FindOwnedNetObjectByNameInSpace : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Finds a net object with the given name owned by this user in the specified space, else nullptr.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |space|[space](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md)| |
> ``` lang=cpp, name=Nada
> function FindOwnedNetObjectByNameInSpace(name : String, space : Space) : Cog
> ``` 


---  
 #  NetUser : Void

 `constructor`

> Constructor.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function NetUser()
> ``` 


---  
 #  ReleaseOwnedNetObjects : Void

> [Server/Offline] Releases ownership of all net objects owned by this user in all spaces.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ReleaseOwnedNetObjects()
> ``` 


---  
 

 
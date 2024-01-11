 `Component` `Networking`



(NOTE) Network Space. Manages the replication of a single space on the network.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](netspace.md#netspace-void)|[ NetObjectCount](netspace.md#netobjectcount-zilch-engi)|[netobject](netobject.md)| |
| |[ NetUserCount](netspace.md#netusercount-zilch-engine)| | |


 #  Properties


---  
 #  NetObjectCount : [integer](../nada_base_types/integer.md)

 `read-only`

> Returns the number of net objects in this space (but not including the net space itself).
> ``` lang=cpp, name=Nada
> var NetObjectCount : Integer


---  
 #  NetUserCount : [integer](../nada_base_types/integer.md)

 `read-only`

> Returns the number of net users in this space.
> ``` lang=cpp, name=Nada
> var NetUserCount : Integer


---  
 #  Methods


---  
 #  NetSpace : Void

 `constructor`

> Constructor.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function NetSpace()
> ``` 


---  
 

 
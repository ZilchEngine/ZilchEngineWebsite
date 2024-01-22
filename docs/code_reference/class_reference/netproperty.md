 `Networking`



(NOTE) Network Property. Manages the replication of a single property on the network.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[LastChangeTimePassed](netproperty.md#lastchangetimepassed-zer)|[safeid32object](safeid32object.md)| |
| |[LastChangeTimestamp](netproperty.md#lastchangetimestamp-zero)| | |
| |[Name](netproperty.md#name-zilch-engine-documen)| | |
| |[NetChannel](netproperty.md#netchannel-zilch-engine-d)| | |
| |[NetPropertyType](netproperty.md#netpropertytype-zilch-eng)| | |


 #  Properties


---  
 #  LastChangeTimePassed : [real](../nada_base_types/real.md)

 `read-only`

> Elapsed time passed since this net property was last changed, else 0.
> ```TS:Nada
> var LastChangeTimePassed : Real


---  
 #  LastChangeTimestamp : [real](../nada_base_types/real.md)

 `read-only`

> Timestamp indicating when this net property was last changed, else 0.
> ```TS:Nada
> var LastChangeTimestamp : Real


---  
 #  Name : [string](../nada_base_types/string.md)

 `read-only`

> Net property name.
> ```TS:Nada
> var Name : String


---  
 #  NetChannel : [netchannel](netchannel.md)

 `read-only`

> Operating net channel.
> ```TS:Nada
> var NetChannel : NetChannel


---  
 #  NetPropertyType : [netpropertytype](netpropertytype.md)

 `read-only`

> Operating net property type.
> ```TS:Nada
> var NetPropertyType : NetPropertyType


---  
 #  Methods


---  
 

 
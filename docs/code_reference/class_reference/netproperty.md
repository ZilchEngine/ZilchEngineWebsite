 `Networking`



(NOTE) Network Property. Manages the replication of a single property on the network.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ LastChangeTimePassed](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netproperty.md#lastchangetimepassed-zer)|[safeid32object](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/safeid32object.md)| |
| |[ LastChangeTimestamp](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netproperty.md#lastchangetimestamp-zero)| | |
| |[ Name](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netproperty.md#name-zilch-engine-documen)| | |
| |[ NetChannel](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netproperty.md#netchannel-zilch-engine-d)| | |
| |[ NetPropertyType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netproperty.md#netpropertytype-zilch-eng)| | |


 #  Properties


---  
 #  LastChangeTimePassed : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

 `read-only`

> Elapsed time passed since this net property was last changed, else 0.
> ``` lang=cpp, name=Nada
> var LastChangeTimePassed : Real


---  
 #  LastChangeTimestamp : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

 `read-only`

> Timestamp indicating when this net property was last changed, else 0.
> ``` lang=cpp, name=Nada
> var LastChangeTimestamp : Real


---  
 #  Name : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

 `read-only`

> Net property name.
> ``` lang=cpp, name=Nada
> var Name : String


---  
 #  NetChannel : [netchannel](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netchannel.md)

 `read-only`

> Operating net channel.
> ``` lang=cpp, name=Nada
> var NetChannel : NetChannel


---  
 #  NetPropertyType : [netpropertytype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpropertytype.md)

 `read-only`

> Operating net property type.
> ``` lang=cpp, name=Nada
> var NetPropertyType : NetPropertyType


---  
 #  Methods


---  
 

 
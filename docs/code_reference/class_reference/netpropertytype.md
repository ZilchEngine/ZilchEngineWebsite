 `Networking`



(NOTE) Network Property Type. Configures the replication of a single property on the network.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ResetConfig](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpropertytype.md#resetconfig-void)|[ Name](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpropertytype.md#name-zilch-engine-documen)|[safeid32object](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/safeid32object.md)| |
|[ SetConfig](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpropertytype.md#setconfig-void)| | | |


 #  Properties


---  
 #  Name : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

 `read-only`

> Net property type name.
> ``` lang=cpp, name=Nada
> var Name : String


---  
 #  Methods


---  
 #  ResetConfig : Void

> Resets all configuration settings. (Cannot be modified at game runtime)
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ResetConfig()
> ``` 


---  
 #  SetConfig : Void

> Sets all configuration settings according to the specified NetPropertyConfig resource. (Cannot be modified at game runtime)
> |Name|Type|Description|
> |---|---|---|
> |netPropertyConfig|[netpropertyconfig](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/netpropertyconfig.md)| |
> ``` lang=cpp, name=Nada
> function SetConfig(netPropertyConfig : NetPropertyConfig)
> ``` 


---  
 

 
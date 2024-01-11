 `Networking`



(NOTE) Network Property Type. Configures the replication of a single property on the network.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ResetConfig](netpropertytype.md#resetconfig-void)|[ Name](netpropertytype.md#name-zilch-engine-documen)|[safeid32object](safeid32object.md)| |
|[ SetConfig](netpropertytype.md#setconfig-void)| | | |


 #  Properties


---  
 #  Name : [string](../nada_base_types/string.md)

 `read-only`

> Net property type name.
> ```TS:Nada
> var Name : String


---  
 #  Methods


---  
 #  ResetConfig : Void

> Resets all configuration settings. (Cannot be modified at game runtime)
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ResetConfig()
> ``` 


---  
 #  SetConfig : Void

> Sets all configuration settings according to the specified NetPropertyConfig resource. (Cannot be modified at game runtime)
> |Name|Type|Description|
> |---|---|---|
> |netPropertyConfig|[netpropertyconfig](netpropertyconfig.md)| |
> ```TS:Nada
> function SetConfig(netPropertyConfig : NetPropertyConfig)
> ``` 


---  
 

 
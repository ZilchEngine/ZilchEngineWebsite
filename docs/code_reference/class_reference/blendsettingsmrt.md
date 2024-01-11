 `Graphics`

(NOTE) Indexable interface for settings BlendSettings.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Get](blendsettingsmrt.md#get-zilch-engine-document)| |[threadsafereferencecounted](threadsafereferencecounted.md)| |
|[ Set](blendsettingsmrt.md#set-void)| | | |


 #  Properties


---  
 #  Methods


---  
 #  Get : [blendsettings](blendsettings.md)

> Get the current BlendSettings for a color target at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Get(index : Integer) : BlendSettings
> ``` 


---  
 #  Set : Void

> Set the BlendSettings for a color target at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> |blendSettings|[blendsettings](blendsettings.md)| |
> ``` lang=cpp, name=Nada
> function Set(index : Integer, blendSettings : BlendSettings)
> ``` 


---  
 

 
 `Graphics`

(NOTE) Interface used to define unique render settings for a base RenderGroup and its sub RenderGroups.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddSubSettings](subrendergrouppass.md#addsubsettings-void)| |[safeid32](safeid32.md)| |
|[ ExcludeSubRenderGroup](subrendergrouppass.md#excludesubrendergroup-vo)| | | |
|[ Reset](subrendergrouppass.md#reset-void)| | | |
|[ SetDefaultSettings](subrendergrouppass.md#setdefaultsettings-void)| | | |


 #  Properties


---  
 #  Methods


---  
 #  AddSubSettings : Void

> Define the settings to use for a specific RenderGroup. Given RenderGroup must be a child of the base RenderGroup, or the base itself, that this was initialized with.
> |Name|Type|Description|
> |---|---|---|
> |subSettings|[rendersettings](rendersettings.md)| |
> |subGroup|[rendergroup](rendergroup.md)| |
> |subPass|[materialblock](materialblock.md)| |
> ``` lang=cpp, name=Nada
> function AddSubSettings(subSettings : RenderSettings, subGroup : RenderGroup, subPass : MaterialBlock)
> ``` 


---  
 #  ExcludeSubRenderGroup : Void

> Explicitely exclude a RenderGroup from rendering when there are default settings. Given RenderGroup must be a child of the base RenderGroup, or the base itself, that this was initialized with.
> |Name|Type|Description|
> |---|---|---|
> |subGroup|[rendergroup](rendergroup.md)| |
> ``` lang=cpp, name=Nada
> function ExcludeSubRenderGroup(subGroup : RenderGroup)
> ``` 


---  
 #  Reset : Void

> Resets interface back to the initial creation state with a given base RenderGroup.
> |Name|Type|Description|
> |---|---|---|
> |baseRenderGroup|[rendergroup](rendergroup.md)| |
> ``` lang=cpp, name=Nada
> function Reset(baseRenderGroup : RenderGroup)
> ``` 


---  
 #  SetDefaultSettings : Void

> Settings to use for the base or all sub RenderGroups that do not have specified settings. Without defaults, the base or any sub RenderGroup without settings will not render.
> |Name|Type|Description|
> |---|---|---|
> |defaultSettings|[rendersettings](rendersettings.md)| |
> |defaultPass|[materialblock](materialblock.md)| |
> ``` lang=cpp, name=Nada
> function SetDefaultSettings(defaultSettings : RenderSettings, defaultPass : MaterialBlock)
> ``` 


---  
 

 
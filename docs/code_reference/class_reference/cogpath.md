 `Engine`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Clone](cogpath.md#clone-zilch-engine-docume)|[ Cog](cogpath.md#cog-zilch-engine-document)|Object| |
|[ Constructor](cogpath.md#cogpath-void)|[ DirectCog](cogpath.md#directcog-zilch-engine-do)| | |
|[ ComputePath](cogpath.md#computepath-zilch-engine)|[ ErrorOnDirectLinkFail](cogpath.md#errorondirectlinkfail-ze)| | |
|[ Refresh](cogpath.md#refresh-zilch-engine-docu)|[ ErrorOnPathCantCompute](cogpath.md#erroronpathcantcompute-z)| | |
|[ RefreshIfNull](cogpath.md#refreshifnull-zilch-engin)|[ ErrorOnResolveToNull](cogpath.md#erroronresolvetonull-zer)| | |
|[ Resolve](cogpath.md#resolve-zilch-engine-docu)|[ Path](cogpath.md#path-zilch-engine-documen)| | |
| |[ PathPreference0](cogpath.md#pathpreference0-zilch-eng)| | |
| |[ PathPreference1](cogpath.md#pathpreference1-zilch-eng)| | |
| |[ PathPreference2](cogpath.md#pathpreference2-zilch-eng)| | |
| |[ RelativeTo](cogpath.md#relativeto-zilch-engine-d)| | |
| |[ UpdateCogOnInitialize](cogpath.md#updatecogoninitialize-ze)| | |
| |[ UpdateCogOnPathChange](cogpath.md#updatecogonpathchange-ze)| | |
| |[ UpdatePathOnCogChange](cogpath.md#updatepathoncogchange-ze)| | |


 #  Properties


---  
 #  Cog : [cog](cog.md)

> Setting the cog manually may recompute the path if the option is set Getting the cog will attempt to resolve the cog if we don't already have one (or if the path options is set, it will always resolve)
> ``` lang=cpp, name=Nada
> var Cog : Cog


---  
 #  DirectCog : [cog](cog.md)

> Setting the cog manually may recompute the path if the option is set Getting the cog will return whatever cog we already resolved, or null (it will not attempt to resolve)
> ``` lang=cpp, name=Nada
> var DirectCog : Cog


---  
 #  ErrorOnDirectLinkFail : [boolean](../nada_base_types/boolean.md)

> Is it an exception/notification if a direct link to the object cannot be resolved?
> ``` lang=cpp, name=Nada
> var ErrorOnDirectLinkFail : Boolean


---  
 #  ErrorOnPathCantCompute : [boolean](../nada_base_types/boolean.md)

> Is it an exception/notification if the path to an object cannot be computed?
> ``` lang=cpp, name=Nada
> var ErrorOnPathCantCompute : Boolean


---  
 #  ErrorOnResolveToNull : [boolean](../nada_base_types/boolean.md)

> Is an exception thrown if you try to access the Cog when it's invalid or not found?
> ``` lang=cpp, name=Nada
> var ErrorOnResolveToNull : Boolean


---  
 #  Path : [string](../nada_base_types/string.md)

> Setting the path will invalidate the object until the next call to GetCog.
> ``` lang=cpp, name=Nada
> var Path : String


---  
 #  PathPreference0 : [CogPathPreference](../enum_reference.md#cogpathpreference)

> 
> ``` lang=cpp, name=Nada
> var PathPreference0 : CogPathPreference


---  
 #  PathPreference1 : [CogPathPreference](../enum_reference.md#cogpathpreference)

> 
> ``` lang=cpp, name=Nada
> var PathPreference1 : CogPathPreference


---  
 #  PathPreference2 : [CogPathPreference](../enum_reference.md#cogpathpreference)

> 
> ``` lang=cpp, name=Nada
> var PathPreference2 : CogPathPreference


---  
 #  RelativeTo : [cog](cog.md)

> The cog that we compute paths relative to.
> ``` lang=cpp, name=Nada
> var RelativeTo : Cog


---  
 #  UpdateCogOnInitialize : [boolean](../nada_base_types/boolean.md)

> Whether the cog path attempts to resolve an object when the object is fully initialized.
> ``` lang=cpp, name=Nada
> var UpdateCogOnInitialize : Boolean


---  
 #  UpdateCogOnPathChange : [boolean](../nada_base_types/boolean.md)

> When we set the cog path, should we try and resolve the object (this also detects parse errors)
> ``` lang=cpp, name=Nada
> var UpdateCogOnPathChange : Boolean


---  
 #  UpdatePathOnCogChange : [boolean](../nada_base_types/boolean.md)

> When we set the cog, should we try and recompute a path to the object?
> ``` lang=cpp, name=Nada
> var UpdatePathOnCogChange : Boolean


---  
 #  Methods


---  
 #  Clone : [cogpath](cogpath.md)

> Creates a new copy of a cog path (since cog paths are reference counted and shared)
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Clone() : CogPath
> ``` 


---  
 #  CogPath : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function CogPath()
> ``` 


---  
 #  CogPath : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ||[cogpath](cogpath.md)| |
> ``` lang=cpp, name=Nada
> function CogPath( : CogPath)
> ``` 


---  
 #  CogPath : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |path|[string](../nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function CogPath(path : String)
> ``` 


---  
 #  ComputePath : [string](../nada_base_types/string.md)

 `static`

> Computes a path from one object to another (or an absolute path if specified - 'from' can be null) If computing the path fails, this will return an empty string.
> |Name|Type|Description|
> |---|---|---|
> |from|[cog](cog.md)| |
> |to|[cog](cog.md)| |
> |pref|[CogPathPreference](../enum_reference.md#cogpathpreference)| |
> ``` lang=cpp, name=Nada
> function ComputePath(from : Cog, to : Cog, pref : CogPathPreference) : String
> ``` 


---  
 #  Refresh : [boolean](../nada_base_types/boolean.md)

> Returns true if the object changes, false otherwise.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Refresh() : Boolean
> ``` 


---  
 #  RefreshIfNull : [boolean](../nada_base_types/boolean.md)

> Returns true if the object changes, false otherwise.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function RefreshIfNull() : Boolean
> ``` 


---  
 #  Resolve : [cog](cog.md)

 `static`

> Resolves a cog from a path and a a relative object (or null for absolute paths) Returns null if it fails to find the cog, and will not throw an exception or assert.
> |Name|Type|Description|
> |---|---|---|
> |startFrom|[cog](cog.md)| |
> |path|[string](../nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function Resolve(startFrom : Cog, path : String) : Cog
> ``` 


---  
 

 
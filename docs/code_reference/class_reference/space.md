 `Engine`

(NOTE) A space is a near boundless, three-dimensional extent in which objects and events occur and have relative position, direction, and time. Essentially a world of objects that exist together. Used to divide objects between UI, World, Editor, and others. The two most Common spaces are the 'World' for the game world and the 'Ui' for the HUD and menus.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddObjectsFromLevel](space.md#addobjectsfromlevel-zero)|[ AllObjects](space.md#allobjects-zilch-engine-d)|[cog](cog.md)| |
|[ Create](space.md#create-zilch-engine-docum)|[ AllRootObjects](space.md#allrootobjects-zilch-engi)| | |
|[ CreateAtPosition](space.md#createatposition-zilch-en)|[ CurrentLevel](space.md#currentlevel-zilch-engine)| | |
|[ CreateLink](space.md#createlink-zilch-engine-d)|[ IsEditorMode](space.md#iseditormode-zilch-engine)| | |
|[ DestroyAll](space.md#destroyall-void)|[ ObjectCount](space.md#objectcount-zilch-engine)| | |
|[ DestroyAllFromLevel](space.md#destroyallfromlevel-void)| | | |
|[ FindAllObjectsByName](space.md#findallobjectsbyname-zer)| | | |
|[ FindFirstObjectByName](space.md#findfirstobjectbyname-ze)| | | |
|[ FindFirstRootObjectByName](space.md#findfirstrootobjectbynam)| | | |
|[ FindLastObjectByName](space.md#findlastobjectbyname-zer)| | | |
|[ FindLastRootObjectByName](space.md#findlastrootobjectbyname)| | | |
|[ FindObjectByName](space.md#findobjectbyname-zilch-en)| | | |
|[ GetModified](space.md#getmodified-zilch-engine)| | | |
|[ LoadLevel](space.md#loadlevel-void)| | | |
|[ MarkModified](space.md#markmodified-void)| | | |
|[ MarkNotModified](space.md#marknotmodified-void)| | | |
|[ ReloadLevel](space.md#reloadlevel-void)| | | |
|[ Constructor](space.md#space-void)| | | |


 #  Properties


---  
 #  AllObjects : [spacerange](spacerange.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var AllObjects : SpaceRange


---  
 #  AllRootObjects : [hierarchylistrange](hierarchylistrange.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var AllRootObjects : HierarchyListRange


---  
 #  CurrentLevel : [level](level.md)

 `read-only`

> Last level loaded.
> ``` lang=cpp, name=Nada
> var CurrentLevel : Level


---  
 #  IsEditorMode : [boolean](../nada_base_types/boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var IsEditorMode : Boolean


---  
 #  ObjectCount : [integer](../nada_base_types/integer.md)

 `read-only`

> Number of objects in the space.
> ``` lang=cpp, name=Nada
> var ObjectCount : Integer


---  
 #  Methods


---  
 #  AddObjectsFromLevel : [level](level.md)

> Add all objects from a level.
> |Name|Type|Description|
> |---|---|---|
> |levelName|[level](level.md)| |
> ``` lang=cpp, name=Nada
> function AddObjectsFromLevel(levelName : Level) : Level
> ``` 


---  
 #  Create : [cog](cog.md)

> Create an object in the space.
> |Name|Type|Description|
> |---|---|---|
> |archetype|[archetype](archetype.md)| |
> ``` lang=cpp, name=Nada
> function Create(archetype : Archetype) : Cog
> ``` 


---  
 #  CreateAtPosition : [cog](cog.md)

> Create a object at a position in the space.
> |Name|Type|Description|
> |---|---|---|
> |archetype|[archetype](archetype.md)| |
> |position|[real3](../nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function CreateAtPosition(archetype : Archetype, position : Real3) : Cog
> ``` 


---  
 #  CreateLink : [cog](cog.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |archetype|[archetype](archetype.md)| |
> |objectA|[cog](cog.md)| |
> |objectB|[cog](cog.md)| |
> ``` lang=cpp, name=Nada
> function CreateLink(archetype : Archetype, objectA : Cog, objectB : Cog) : Cog
> ``` 


---  
 #  DestroyAll : Void

> Destroy all objects in space.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function DestroyAll()
> ``` 


---  
 #  DestroyAllFromLevel : Void

> Destroy all objects created from level.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function DestroyAllFromLevel()
> ``` 


---  
 #  FindAllObjectsByName : [cognamerange](cognamerange.md)

> Find an object in the space with a given name.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function FindAllObjectsByName(name : String) : CogNameRange
> ``` 


---  
 #  FindFirstObjectByName : [cog](cog.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function FindFirstObjectByName(name : String) : Cog
> ``` 


---  
 #  FindFirstRootObjectByName : [cog](cog.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function FindFirstRootObjectByName(name : String) : Cog
> ``` 


---  
 #  FindLastObjectByName : [cog](cog.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function FindLastObjectByName(name : String) : Cog
> ``` 


---  
 #  FindLastRootObjectByName : [cog](cog.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function FindLastRootObjectByName(name : String) : Cog
> ``` 


---  
 #  FindObjectByName : [cog](cog.md)

> Find an object in the space with a given name.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function FindObjectByName(name : String) : Cog
> ``` 


---  
 #  GetModified : [boolean](../nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function GetModified() : Boolean
> ``` 


---  
 #  LoadLevel : Void

> Load new level replace the current level.
> |Name|Type|Description|
> |---|---|---|
> |level|[level](level.md)| |
> ``` lang=cpp, name=Nada
> function LoadLevel(level : Level)
> ``` 


---  
 #  MarkModified : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function MarkModified()
> ``` 


---  
 #  MarkNotModified : Void

> Clears all modifications on this Cog. Does not clear LocalModificationOverride properties.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function MarkNotModified()
> ``` 


---  
 #  ReloadLevel : Void

> Reload the current level.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ReloadLevel()
> ``` 


---  
 #  Space : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Space()
> ``` 


---  
 

 
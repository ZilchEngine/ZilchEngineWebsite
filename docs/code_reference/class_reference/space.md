 `Engine`

(NOTE) A space is a near boundless, three-dimensional extent in which objects and events occur and have relative position, direction, and time. Essentially a world of objects that exist together. Used to divide objects between UI, World, Editor, and others. The two most Common spaces are the 'World' for the game world and the 'Ui' for the HUD and menus.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddObjectsFromLevel](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md#addobjectsfromlevel-zero)|[ AllObjects](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md#allobjects-zilch-engine-d)|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
|[ Create](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md#create-zilch-engine-docum)|[ AllRootObjects](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md#allrootobjects-zilch-engi)| | |
|[ CreateAtPosition](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md#createatposition-zilch-en)|[ CurrentLevel](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md#currentlevel-zilch-engine)| | |
|[ CreateLink](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md#createlink-zilch-engine-d)|[ IsEditorMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md#iseditormode-zilch-engine)| | |
|[ DestroyAll](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md#destroyall-void)|[ ObjectCount](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md#objectcount-zilch-engine)| | |
|[ DestroyAllFromLevel](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md#destroyallfromlevel-void)| | | |
|[ FindAllObjectsByName](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md#findallobjectsbyname-zer)| | | |
|[ FindFirstObjectByName](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md#findfirstobjectbyname-ze)| | | |
|[ FindFirstRootObjectByName](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md#findfirstrootobjectbynam)| | | |
|[ FindLastObjectByName](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md#findlastobjectbyname-zer)| | | |
|[ FindLastRootObjectByName](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md#findlastrootobjectbyname)| | | |
|[ FindObjectByName](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md#findobjectbyname-zilch-en)| | | |
|[ GetModified](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md#getmodified-zilch-engine)| | | |
|[ LoadLevel](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md#loadlevel-void)| | | |
|[ MarkModified](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md#markmodified-void)| | | |
|[ MarkNotModified](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md#marknotmodified-void)| | | |
|[ ReloadLevel](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md#reloadlevel-void)| | | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md#space-void)| | | |


 #  Properties


---  
 #  AllObjects : [spacerange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spacerange.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var AllObjects : SpaceRange


---  
 #  AllRootObjects : [hierarchylistrange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/hierarchylistrange.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var AllRootObjects : HierarchyListRange


---  
 #  CurrentLevel : [level](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/level.md)

 `read-only`

> Last level loaded.
> ``` lang=cpp, name=Nada
> var CurrentLevel : Level


---  
 #  IsEditorMode : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var IsEditorMode : Boolean


---  
 #  ObjectCount : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Number of objects in the space.
> ``` lang=cpp, name=Nada
> var ObjectCount : Integer


---  
 #  Methods


---  
 #  AddObjectsFromLevel : [level](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/level.md)

> Add all objects from a level.
> |Name|Type|Description|
> |---|---|---|
> |levelName|[level](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/level.md)| |
> ``` lang=cpp, name=Nada
> function AddObjectsFromLevel(levelName : Level) : Level
> ``` 


---  
 #  Create : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Create an object in the space.
> |Name|Type|Description|
> |---|---|---|
> |archetype|[archetype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/archetype.md)| |
> ``` lang=cpp, name=Nada
> function Create(archetype : Archetype) : Cog
> ``` 


---  
 #  CreateAtPosition : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Create a object at a position in the space.
> |Name|Type|Description|
> |---|---|---|
> |archetype|[archetype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/archetype.md)| |
> |position|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function CreateAtPosition(archetype : Archetype, position : Real3) : Cog
> ``` 


---  
 #  CreateLink : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |archetype|[archetype](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/archetype.md)| |
> |objectA|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> |objectB|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
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
 #  FindAllObjectsByName : [cognamerange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cognamerange.md)

> Find an object in the space with a given name.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function FindAllObjectsByName(name : String) : CogNameRange
> ``` 


---  
 #  FindFirstObjectByName : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function FindFirstObjectByName(name : String) : Cog
> ``` 


---  
 #  FindFirstRootObjectByName : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function FindFirstRootObjectByName(name : String) : Cog
> ``` 


---  
 #  FindLastObjectByName : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function FindLastObjectByName(name : String) : Cog
> ``` 


---  
 #  FindLastRootObjectByName : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function FindLastRootObjectByName(name : String) : Cog
> ``` 


---  
 #  FindObjectByName : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Find an object in the space with a given name.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function FindObjectByName(name : String) : Cog
> ``` 


---  
 #  GetModified : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

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
> |level|[level](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/level.md)| |
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
 

 
 `Engine`

(NOTE) The GameSession manages all spaces and data for a a game.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ CreateNamedSpace](gamesession.md#createnamedspace-zilch-en)|[ AllSpaces](gamesession.md#allspaces-zilch-engine-do)|[cog](cog.md)| |
|[ CreateSpace](gamesession.md#createspace-zilch-engine)|[ Focused](gamesession.md#focused-zilch-engine-docu)| | |
|[ FindAllSpacesByName](gamesession.md#findallspacesbyname-zero)|[ FullScreen](gamesession.md#fullscreen-zilch-engine-d)| | |
|[ FindSpaceByName](gamesession.md#findspacebyname-zilch-eng)|[ Paused](gamesession.md#paused-zilch-engine-docum)| | |
|[ Constructor](gamesession.md#gamesession-void)|[ Resolution](gamesession.md#resolution-zilch-engine-d)| | |
|[ IsEditorMode](gamesession.md#iseditormode-zilch-engine)| | | |
|[ Pause](gamesession.md#pause-void)| | | |
|[ Quit](gamesession.md#quit-void)| | | |
|[ RequestQuit](gamesession.md#requestquit-void)| | | |
|[ Start](gamesession.md#start-void)| | | |


 #  Properties


---  
 #  AllSpaces : [spacemapvaluerange](spacemapvaluerange.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var AllSpaces : SpaceMapValueRange


---  
 #  Focused : [boolean](../nada_base_types/boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Focused : Boolean


---  
 #  FullScreen : [boolean](../nada_base_types/boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var FullScreen : Boolean


---  
 #  Paused : [boolean](../nada_base_types/boolean.md)

> Controls if the game session is paused which prevents updates to all spaces owned by this game.
> ``` lang=cpp, name=Nada
> var Paused : Boolean


---  
 #  Resolution : [real2](../nada_base_types/real2.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Resolution : Real2


---  
 #  Methods


---  
 #  CreateNamedSpace : [space](space.md)

> Create a space from an archetype with the given name.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> |archetype|[archetype](archetype.md)| |
> ``` lang=cpp, name=Nada
> function CreateNamedSpace(name : String, archetype : Archetype) : Space
> ``` 


---  
 #  CreateSpace : [space](space.md)

> Create a space in the game. Use the archetype's name.
> |Name|Type|Description|
> |---|---|---|
> |archetype|[archetype](archetype.md)| |
> ``` lang=cpp, name=Nada
> function CreateSpace(archetype : Archetype) : Space
> ``` 


---  
 #  FindAllSpacesByName : [spacemapvaluerange](spacemapvaluerange.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function FindAllSpacesByName(name : String) : SpaceMapValueRange
> ``` 


---  
 #  FindSpaceByName : [space](space.md)

> Find a named space.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function FindSpaceByName(name : String) : Space
> ``` 


---  
 #  GameSession : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function GameSession()
> ``` 


---  
 #  IsEditorMode : [boolean](../nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function IsEditorMode() : Boolean
> ``` 


---  
 #  Pause : Void

> Pauses the game session which prevents updates to all spaces owned by this game.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Pause()
> ``` 


---  
 #  Quit : Void

> Quit the game and exit the engine if not in editor.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Quit()
> ``` 


---  
 #  RequestQuit : Void

> Request to quit sending out the GameRequestQuit event.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function RequestQuit()
> ``` 


---  
 #  Start : Void

> Start the game.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Start()
> ``` 


---  
 

 
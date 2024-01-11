 `Editor`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddResource](editor.md#addresource-void)|[ Actions](editor.md#actions-zilch-engine-docu)|[multidock](multidock.md)|[editormain](editormain.md)|
|[ AddResourceType](editor.md#addresourcetype-void)|[ EditGameSession](editor.md#editgamesession-zilch-eng)| | |
|[ CreateDockableWindow](editor.md#createdockablewindow-voi)|[ EditLevel](editor.md#editlevel-zilch-engine-do)| | |
|[ DisplayGameSession](editor.md#displaygamesession-void)|[ EditSpace](editor.md#editspace-zilch-engine-do)| | |
|[ EditGameSpaces](editor.md#editgamespaces-void)|[ OperationQueue](editor.md#operationqueue-zilch-engi)| | |
|[ EditResource](editor.md#editresource-void)|[ ProjectCog](editor.md#projectcog-zilch-engine-d)| | |
|[ ExecuteCommand](editor.md#executecommand-void)|[ Selection](editor.md#selection-zilch-engine-do)| | |
|[ PauseGame](editor.md#pausegame-void)| | | |
|[ PlayGame](editor.md#playgame-zilch-engine-doc)| | | |
|[ PlayNewGame](editor.md#playnewgame-zilch-engine)| | | |
|[ PlaySingleGame](editor.md#playsinglegame-zilch-engi)| | | |
|[ SelectPrimary](editor.md#selectprimary-void)| | | |
|[ SelectTool](editor.md#selecttool-void)| | | |
|[ SetFocus](editor.md#setfocus-void)| | | |
|[ SetGamePaused](editor.md#setgamepaused-void)| | | |
|[ SetMainPropertyViewObject](editor.md#setmainpropertyviewobjec)| | | |
|[ StepGame](editor.md#stepgame-void)| | | |
|[ StopGame](editor.md#stopgame-void)| | | |
|[ ToggleGamePaused](editor.md#togglegamepaused-void)| | | |
|[ ZoomOnGame](editor.md#zoomongame-void)| | | |


 #  Properties


---  
 #  Actions : [actions](actions.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Actions : Actions


---  
 #  EditGameSession : [gamesession](gamesession.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var EditGameSession : GameSession


---  
 #  EditLevel : [level](level.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var EditLevel : Level


---  
 #  EditSpace : [space](space.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var EditSpace : Space


---  
 #  OperationQueue : [operationqueue](operationqueue.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var OperationQueue : OperationQueue


---  
 #  ProjectCog : [cog](cog.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var ProjectCog : Cog


---  
 #  Selection : [metaselection](metaselection.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Selection : MetaSelection


---  
 #  Methods


---  
 #  AddResource : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function AddResource()
> ``` 


---  
 #  AddResourceType : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[boundtype](../nada_base_types/boundtype.md)| |
> |p1|[string](../nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function AddResourceType(p0 : BoundType, p1 : String)
> ``` 


---  
 #  CreateDockableWindow : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[string](../nada_base_types/string.md)| |
> |p1|[cameraviewport](cameraviewport.md)| |
> |p2|[real2](../nada_base_types/real2.md)| |
> |p3|[boolean](../nada_base_types/boolean.md)| |
> |p4|[DockArea](../enum_reference.md#dockarea)| |
> ``` lang=cpp, name=Nada
> function CreateDockableWindow(p0 : String, p1 : CameraViewport, p2 : Real2, p3 : Boolean, p4 : DockArea)
> ``` 


---  
 #  DisplayGameSession : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[string](../nada_base_types/string.md)| |
> |p1|[gamesession](gamesession.md)| |
> ``` lang=cpp, name=Nada
> function DisplayGameSession(p0 : String, p1 : GameSession)
> ``` 


---  
 #  EditGameSpaces : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function EditGameSpaces()
> ``` 


---  
 #  EditResource : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|Resource| |
> ``` lang=cpp, name=Nada
> function EditResource(p0 : Resource)
> ``` 


---  
 #  ExecuteCommand : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[string](../nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function ExecuteCommand(p0 : String)
> ``` 


---  
 #  PauseGame : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function PauseGame()
> ``` 


---  
 #  PlayGame : [gamesession](gamesession.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[PlayGameOptions](../enum_reference.md#playgameoptions)| |
> |p1|[boolean](../nada_base_types/boolean.md)| |
> |p2|[boolean](../nada_base_types/boolean.md)| |
> ``` lang=cpp, name=Nada
> function PlayGame(p0 : PlayGameOptions, p1 : Boolean, p2 : Boolean) : GameSession
> ``` 


---  
 #  PlayNewGame : [gamesession](gamesession.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function PlayNewGame() : GameSession
> ``` 


---  
 #  PlaySingleGame : [gamesession](gamesession.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function PlaySingleGame() : GameSession
> ``` 


---  
 #  SelectPrimary : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[anyhandle](../nada_base_types/anyhandle.md)| |
> ``` lang=cpp, name=Nada
> function SelectPrimary(p0 : AnyHandle)
> ``` 


---  
 #  SelectTool : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[string](../nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function SelectTool(p0 : String)
> ``` 


---  
 #  SetFocus : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[space](space.md)| |
> ``` lang=cpp, name=Nada
> function SetFocus(p0 : Space)
> ``` 


---  
 #  SetGamePaused : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[boolean](../nada_base_types/boolean.md)| |
> ``` lang=cpp, name=Nada
> function SetGamePaused(p0 : Boolean)
> ``` 


---  
 #  SetMainPropertyViewObject : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|Object| |
> ``` lang=cpp, name=Nada
> function SetMainPropertyViewObject(p0 : Object)
> ``` 


---  
 #  StepGame : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function StepGame()
> ``` 


---  
 #  StopGame : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function StopGame()
> ``` 


---  
 #  ToggleGamePaused : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ToggleGamePaused()
> ``` 


---  
 #  ZoomOnGame : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[gamesession](gamesession.md)| |
> ``` lang=cpp, name=Nada
> function ZoomOnGame(p0 : GameSession)
> ``` 


---  
 

 
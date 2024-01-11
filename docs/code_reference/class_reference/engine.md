 `Engine`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ CrashEngine](engine.md#crashengine-void)|[ GameSessions](engine.md#gamesessions-zilch-engine)|[eventobject](eventobject.md)| |
|[ CreateGameSession](engine.md#creategamesession-zilch-e)| | | |
|[ CreateGameSessionFromArchetype](engine.md#creategamesessionfromarc)| | | |
|[ DebugBreak](engine.md#debugbreak-void)| | | |
|[ GetCurrentInputDevice](engine.md#getcurrentinputdevice-ze)| | | |
|[ RebuildArchetypes](engine.md#rebuildarchetypes-void)| | | |
|[ Terminate](engine.md#terminate-void)| | | |


 #  Properties


---  
 #  GameSessions : [gamesessionrange](gamesessionrange.md)

 `read-only`

> 
> ```TS:Nada
> var GameSessions : GameSessionRange


---  
 #  Methods


---  
 #  CrashEngine : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function CrashEngine()
> ``` 


---  
 #  CreateGameSession : [gamesession](gamesession.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function CreateGameSession() : GameSession
> ``` 


---  
 #  CreateGameSessionFromArchetype : [gamesession](gamesession.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[archetype](archetype.md)| |
> ```TS:Nada
> function CreateGameSessionFromArchetype(p0 : Archetype) : GameSession
> ``` 


---  
 #  DebugBreak : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function DebugBreak()
> ``` 


---  
 #  GetCurrentInputDevice : [InputDevice](../enum_reference.md#inputdevice)

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function GetCurrentInputDevice() : InputDevice
> ``` 


---  
 #  RebuildArchetypes : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[archetype](archetype.md)| |
> ```TS:Nada
> function RebuildArchetypes(p0 : Archetype)
> ``` 


---  
 #  Terminate : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Terminate()
> ``` 


---  
 

 
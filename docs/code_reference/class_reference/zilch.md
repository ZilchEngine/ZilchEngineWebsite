 `Gameplay`

(NOTE) Global functionality exposed to Nada script. Bound as "Zilch" to script (e.g. Zilch.Keyboard) ZilchStatic was used to avoid the conflict with namespace Zilch).

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Connect](zilch.md#connect-void)|[Audio](zilch.md#audio-zilch-engine-docume)| | |
|[Disconnect](zilch.md#disconnect-void)|[Editor](zilch.md#editor-zilch-engine-docum)| | |
|[DisconnectAll](zilch.md#disconnectall-void)|[Engine](zilch.md#engine-zilch-engine-docum)| | |
| |[Environment](zilch.md#environment-zilch-engine)| | |
| |[Gamepads](zilch.md#gamepads-zilch-engine-doc)| | |
| |[Joysticks](zilch.md#joysticks-zilch-engine-do)| | |
| |[Keyboard](zilch.md#keyboard-zilch-engine-doc)| | |
| |[Mouse](zilch.md#mouse-zilch-engine-docume)| | |
| |[ObjectStore](zilch.md#objectstore-zilch-engine)| | |
| |[OsShell](zilch.md#osshell-zilch-engine-docu)| | |
| |[ResourceSystem](zilch.md#resourcesystem-zilch-engi)| | |


 #  Properties


---  
 #  Audio : [audio](audio.md)

 `read-only` `static`

> 
> ```TS
> var Audio : Audio


---  
 #  Editor : [editor](editor.md)

 `read-only` `static`

> 
> ```TS
> var Editor : Editor


---  
 #  Engine : [engine](engine.md)

 `read-only` `static`

> 
> ```TS
> var Engine : Engine


---  
 #  Environment : [environment](environment.md)

 `read-only` `static`

> 
> ```TS
> var Environment : Environment


---  
 #  Gamepads : [gamepads](gamepads.md)

 `read-only` `static`

> 
> ```TS
> var Gamepads : Gamepads


---  
 #  Joysticks : [joysticks](joysticks.md)

 `read-only` `static`

> 
> ```TS
> var Joysticks : Joysticks


---  
 #  Keyboard : [keyboard](keyboard.md)

 `read-only` `static`

> 
> ```TS
> var Keyboard : Keyboard


---  
 #  Mouse : [mouse](mouse.md)

 `read-only` `static`

> 
> ```TS
> var Mouse : Mouse


---  
 #  ObjectStore : [objectstore](objectstore.md)

 `read-only` `static`

> 
> ```TS
> var ObjectStore : ObjectStore


---  
 #  OsShell : [osshell](osshell.md)

 `read-only` `static`

> 
> ```TS
> var OsShell : OsShell


---  
 #  ResourceSystem : [resourcesystem](resourcesystem.md)

 `read-only` `static`

> 
> ```TS
> var ResourceSystem : ResourceSystem


---  
 #  Methods


---  
 #  Connect : Void

 `static`

> Connection invokes the given delegate when sender dispatches the specified event.
> |Name|Type|Description|
> |---|---|---|
> |sender|Object| |
> |eventId|[string](../nada_base_types/string.md)| |
> |receiverDelegate|delegate()| |
> ```TS
> function Connect(sender : Object, eventId : String, receiverDelegate : delegate())
> ``` 


---  
 #  Disconnect : Void

 `static`

> Removes specified event connection, if connection delegate was a component method then receiver object is just the component.
> |Name|Type|Description|
> |---|---|---|
> |sender|Object| |
> |eventId|[string](../nada_base_types/string.md)| |
> |receiver|Object| |
> ```TS
> function Disconnect(sender : Object, eventId : String, receiver : Object)
> ``` 


---  
 #  DisconnectAll : Void

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ||Object| |
> ||Object| |
> ```TS
> function DisconnectAll( : Object,  : Object)
> ``` 


---  
 

 
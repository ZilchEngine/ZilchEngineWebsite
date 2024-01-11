 `Gameplay`

(NOTE) Global functionality exposed to Nada script. Bound as "Zilch" to script (e.g. Zilch.Keyboard) ZilchStatic was used to avoid the conflict with namespace Zilch).

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Connect](zero.md#connect-void)|[ Audio](zero.md#audio-zilch-engine-docume)| | |
|[ Disconnect](zero.md#disconnect-void)|[ Editor](zero.md#editor-zilch-engine-docum)| | |
|[ DisconnectAll](zero.md#disconnectall-void)|[ Engine](zero.md#engine-zilch-engine-docum)| | |
| |[ Environment](zero.md#environment-zilch-engine)| | |
| |[ Gamepads](zero.md#gamepads-zilch-engine-doc)| | |
| |[ Joysticks](zero.md#joysticks-zilch-engine-do)| | |
| |[ Keyboard](zero.md#keyboard-zilch-engine-doc)| | |
| |[ Mouse](zero.md#mouse-zilch-engine-docume)| | |
| |[ ObjectStore](zero.md#objectstore-zilch-engine)| | |
| |[ OsShell](zero.md#osshell-zilch-engine-docu)| | |
| |[ ResourceSystem](zero.md#resourcesystem-zilch-engi)| | |


 #  Properties


---  
 #  Audio : [audio](audio.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var Audio : Audio


---  
 #  Editor : [editor](editor.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var Editor : Editor


---  
 #  Engine : [engine](engine.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var Engine : Engine


---  
 #  Environment : [environment](environment.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var Environment : Environment


---  
 #  Gamepads : [gamepads](gamepads.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var Gamepads : Gamepads


---  
 #  Joysticks : [joysticks](joysticks.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var Joysticks : Joysticks


---  
 #  Keyboard : [keyboard](keyboard.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var Keyboard : Keyboard


---  
 #  Mouse : [mouse](mouse.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var Mouse : Mouse


---  
 #  ObjectStore : [objectstore](objectstore.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var ObjectStore : ObjectStore


---  
 #  OsShell : [osshell](osshell.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var OsShell : OsShell


---  
 #  ResourceSystem : [resourcesystem](resourcesystem.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
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
> ``` lang=cpp, name=Nada
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
> ``` lang=cpp, name=Nada
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
> ``` lang=cpp, name=Nada
> function DisconnectAll( : Object,  : Object)
> ``` 


---  
 

 
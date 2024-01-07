 `Gameplay`

(NOTE) Global functionality exposed to Nada script. Bound as "Zilch" to script (e.g. Zilch.Keyboard) ZilchStatic was used to avoid the conflict with namespace Zilch).

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Connect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/zero.md#connect-void)|[ Audio](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/zero.md#audio-zilch-engine-docume)| | |
|[ Disconnect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/zero.md#disconnect-void)|[ Editor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/zero.md#editor-zilch-engine-docum)| | |
|[ DisconnectAll](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/zero.md#disconnectall-void)|[ Engine](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/zero.md#engine-zilch-engine-docum)| | |
| |[ Environment](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/zero.md#environment-zilch-engine)| | |
| |[ Gamepads](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/zero.md#gamepads-zilch-engine-doc)| | |
| |[ Joysticks](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/zero.md#joysticks-zilch-engine-do)| | |
| |[ Keyboard](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/zero.md#keyboard-zilch-engine-doc)| | |
| |[ Mouse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/zero.md#mouse-zilch-engine-docume)| | |
| |[ ObjectStore](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/zero.md#objectstore-zilch-engine)| | |
| |[ OsShell](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/zero.md#osshell-zilch-engine-docu)| | |
| |[ ResourceSystem](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/zero.md#resourcesystem-zilch-engi)| | |


 #  Properties


---  
 #  Audio : [audio](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/audio.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var Audio : Audio


---  
 #  Editor : [editor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/editor.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var Editor : Editor


---  
 #  Engine : [engine](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/engine.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var Engine : Engine


---  
 #  Environment : [environment](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/environment.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var Environment : Environment


---  
 #  Gamepads : [gamepads](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gamepads.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var Gamepads : Gamepads


---  
 #  Joysticks : [joysticks](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/joysticks.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var Joysticks : Joysticks


---  
 #  Keyboard : [keyboard](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/keyboard.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var Keyboard : Keyboard


---  
 #  Mouse : [mouse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mouse.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var Mouse : Mouse


---  
 #  ObjectStore : [objectstore](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objectstore.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var ObjectStore : ObjectStore


---  
 #  OsShell : [osshell](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/osshell.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var OsShell : OsShell


---  
 #  ResourceSystem : [resourcesystem](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/resourcesystem.md)

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
> |eventId|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
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
> |eventId|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
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
 

 
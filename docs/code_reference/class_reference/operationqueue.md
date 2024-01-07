 `Engine`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ BeginBatch](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/operationqueue.md#beginbatch-void)|[ ActiveBatchName](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/operationqueue.md#activebatchname-zilch-eng)|[referencecountedeventobject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/referencecountedeventobject.md)| |
|[ ClearAll](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/operationqueue.md#clearall-void)|[ Commands](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/operationqueue.md#commands-zilch-engine-doc)| | |
|[ ClearRedo](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/operationqueue.md#clearredo-void)|[ RedoCommands](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/operationqueue.md#redocommands-zilch-engine)| | |
|[ ClearUndo](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/operationqueue.md#clearundo-void)| | | |
|[ DestroyObject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/operationqueue.md#destroyobject-void)| | | |
|[ EndBatch](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/operationqueue.md#endbatch-void)| | | |
|[ IsListeningForSideEffects](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/operationqueue.md#islisteningforsideeffect)| | | |
|[ MarkPropertyAsModified](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/operationqueue.md#markpropertyasmodified-v)| | | |
|[ ObjectCreated](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/operationqueue.md#objectcreated-void)| | | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/operationqueue.md#operationqueue-void)| | | |
|[ PopSubPropertyContext](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/operationqueue.md#popsubpropertycontext-vo)| | | |
|[ QueueRegisteredSideEffects](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/operationqueue.md#queueregisteredsideeffec)| | | |
|[ Redo](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/operationqueue.md#redo-void)| | | |
|[ RegisterSideEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/operationqueue.md#registersideeffect-void)| | | |
|[ SaveObjectState](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/operationqueue.md#saveobjectstate-void)| | | |
|[ StartListeningForSideEffects](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/operationqueue.md#startlisteningforsideeff)| | | |
|[ Undo](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/operationqueue.md#undo-void)| | | |


 #  Properties


---  
 #  ActiveBatchName : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> 
> ``` lang=cpp, name=Nada
> var ActiveBatchName : String


---  
 #  Commands : [operationlistrange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/operationlistrange.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Commands : OperationListRange


---  
 #  RedoCommands : [operationlistrange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/operationlistrange.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var RedoCommands : OperationListRange


---  
 #  Methods


---  
 #  BeginBatch : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function BeginBatch()
> ``` 


---  
 #  BeginBatch : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function BeginBatch(p0 : String)
> ``` 


---  
 #  ClearAll : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ClearAll()
> ``` 


---  
 #  ClearRedo : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ClearRedo()
> ``` 


---  
 #  ClearUndo : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ClearUndo()
> ``` 


---  
 #  DestroyObject : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Nada
> function DestroyObject(p0 : Cog)
> ``` 


---  
 #  EndBatch : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function EndBatch()
> ``` 


---  
 #  IsListeningForSideEffects : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function IsListeningForSideEffects() : Boolean
> ``` 


---  
 #  MarkPropertyAsModified : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)| |
> |p1|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function MarkPropertyAsModified(p0 : Component, p1 : String)
> ``` 


---  
 #  ObjectCreated : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Nada
> function ObjectCreated(p0 : Cog)
> ``` 


---  
 #  OperationQueue : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function OperationQueue()
> ``` 


---  
 #  PopSubPropertyContext : Void

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function PopSubPropertyContext()
> ``` 


---  
 #  QueueRegisteredSideEffects : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function QueueRegisteredSideEffects()
> ``` 


---  
 #  Redo : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Redo()
> ``` 


---  
 #  Redo : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[operation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/operation.md)| |
> ``` lang=cpp, name=Nada
> function Redo(p0 : Operation) : Boolean
> ``` 


---  
 #  RegisterSideEffect : Void

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[anyhandle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/anyhandle.md)| |
> |p1|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |p2|T| |
> ``` lang=cpp, name=Nada
> function RegisterSideEffect(p0 : AnyHandle, p1 : String, p2 : T)
> ``` 


---  
 #  SaveObjectState : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Nada
> function SaveObjectState(p0 : Cog)
> ``` 


---  
 #  StartListeningForSideEffects : Void

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function StartListeningForSideEffects()
> ``` 


---  
 #  Undo : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Undo()
> ``` 


---  
 #  Undo : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[operation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/operation.md)| |
> ``` lang=cpp, name=Nada
> function Undo(p0 : Operation) : Boolean
> ``` 


---  
 

 
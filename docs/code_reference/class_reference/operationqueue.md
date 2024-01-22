 `Engine`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[BeginBatch](operationqueue.md#beginbatch-void)|[ActiveBatchName](operationqueue.md#activebatchname-zilch-eng)|[referencecountedeventobject](referencecountedeventobject.md)| |
|[ClearAll](operationqueue.md#clearall-void)|[Commands](operationqueue.md#commands-zilch-engine-doc)| | |
|[ClearRedo](operationqueue.md#clearredo-void)|[RedoCommands](operationqueue.md#redocommands-zilch-engine)| | |
|[ClearUndo](operationqueue.md#clearundo-void)| | | |
|[DestroyObject](operationqueue.md#destroyobject-void)| | | |
|[EndBatch](operationqueue.md#endbatch-void)| | | |
|[IsListeningForSideEffects](operationqueue.md#islisteningforsideeffect)| | | |
|[MarkPropertyAsModified](operationqueue.md#markpropertyasmodified-v)| | | |
|[ObjectCreated](operationqueue.md#objectcreated-void)| | | |
|[Constructor](operationqueue.md#operationqueue-void)| | | |
|[PopSubPropertyContext](operationqueue.md#popsubpropertycontext-vo)| | | |
|[QueueRegisteredSideEffects](operationqueue.md#queueregisteredsideeffec)| | | |
|[Redo](operationqueue.md#redo-void)| | | |
|[RegisterSideEffect](operationqueue.md#registersideeffect-void)| | | |
|[SaveObjectState](operationqueue.md#saveobjectstate-void)| | | |
|[StartListeningForSideEffects](operationqueue.md#startlisteningforsideeff)| | | |
|[Undo](operationqueue.md#undo-void)| | | |


 #  Properties


---  
 #  ActiveBatchName : [string](../nada_base_types/string.md)

> 
> ```TS:Nada
> var ActiveBatchName : String


---  
 #  Commands : [operationlistrange](operationlistrange.md)

 `read-only`

> 
> ```TS:Nada
> var Commands : OperationListRange


---  
 #  RedoCommands : [operationlistrange](operationlistrange.md)

 `read-only`

> 
> ```TS:Nada
> var RedoCommands : OperationListRange


---  
 #  Methods


---  
 #  BeginBatch : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function BeginBatch()
> ``` 


---  
 #  BeginBatch : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function BeginBatch(p0 : String)
> ``` 


---  
 #  ClearAll : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ClearAll()
> ``` 


---  
 #  ClearRedo : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ClearRedo()
> ``` 


---  
 #  ClearUndo : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ClearUndo()
> ``` 


---  
 #  DestroyObject : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[cog](cog.md)| |
> ```TS:Nada
> function DestroyObject(p0 : Cog)
> ``` 


---  
 #  EndBatch : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function EndBatch()
> ``` 


---  
 #  IsListeningForSideEffects : [boolean](../nada_base_types/boolean.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function IsListeningForSideEffects() : Boolean
> ``` 


---  
 #  MarkPropertyAsModified : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[component](component.md)| |
> |p1|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function MarkPropertyAsModified(p0 : Component, p1 : String)
> ``` 


---  
 #  ObjectCreated : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[cog](cog.md)| |
> ```TS:Nada
> function ObjectCreated(p0 : Cog)
> ``` 


---  
 #  OperationQueue : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function OperationQueue()
> ``` 


---  
 #  PopSubPropertyContext : Void

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function PopSubPropertyContext()
> ``` 


---  
 #  QueueRegisteredSideEffects : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function QueueRegisteredSideEffects()
> ``` 


---  
 #  Redo : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Redo()
> ``` 


---  
 #  Redo : [boolean](../nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[operation](operation.md)| |
> ```TS:Nada
> function Redo(p0 : Operation) : Boolean
> ``` 


---  
 #  RegisterSideEffect : Void

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[anyhandle](../nada_base_types/anyhandle.md)| |
> |p1|[string](../nada_base_types/string.md)| |
> |p2|T| |
> ```TS:Nada
> function RegisterSideEffect(p0 : AnyHandle, p1 : String, p2 : T)
> ``` 


---  
 #  SaveObjectState : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[cog](cog.md)| |
> ```TS:Nada
> function SaveObjectState(p0 : Cog)
> ``` 


---  
 #  StartListeningForSideEffects : Void

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function StartListeningForSideEffects()
> ``` 


---  
 #  Undo : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Undo()
> ``` 


---  
 #  Undo : [boolean](../nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[operation](operation.md)| |
> ```TS:Nada
> function Undo(p0 : Operation) : Boolean
> ``` 


---  
 

 
 `Component` `Editor`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddObject](objecttransformgizmo.md#addobject-void)|[ Basis](objecttransformgizmo.md#basis-zilch-engine-docume)|[component](component.md)|[objectrotategizmo](objectrotategizmo.md)|
|[ ClearObjects](objecttransformgizmo.md#clearobjects-void)|[ ObjectCount](objecttransformgizmo.md#objectcount-zilch-engine)| |[objectscalegizmo](objectscalegizmo.md)|
|[ GetObjectAtIndex](objecttransformgizmo.md#getobjectatindex-zilch-en)|[ Pivot](objecttransformgizmo.md#pivot-zilch-engine-docume)| |[objecttranslategizmo](objecttranslategizmo.md)|
|[ Constructor](objecttransformgizmo.md#objecttransformgizmo-voi)| | | |
|[ RemoveObject](objecttransformgizmo.md#removeobject-void)| | | |
|[ SetOperationQueue](objecttransformgizmo.md#setoperationqueue-void)| | | |
|[ ToggleCoordinateMode](objecttransformgizmo.md#togglecoordinatemode-voi)| | | |


 #  Properties


---  
 #  Basis : [GizmoBasis](../enum_reference.md#gizmobasis)

> Setters / Getters.
> ``` lang=cpp, name=Nada
> var Basis : GizmoBasis


---  
 #  ObjectCount : [integer](../nada_base_types/integer.md)

 `read-only`

> Object getters.
> ``` lang=cpp, name=Nada
> var ObjectCount : Integer


---  
 #  Pivot : [GizmoPivot](../enum_reference.md#gizmopivot)

> 
> ``` lang=cpp, name=Nada
> var Pivot : GizmoPivot


---  
 #  Methods


---  
 #  AddObject : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ||[anyhandle](../nada_base_types/anyhandle.md)| |
> ||[boolean](../nada_base_types/boolean.md)| |
> ``` lang=cpp, name=Nada
> function AddObject( : AnyHandle,  : Boolean)
> ``` 


---  
 #  ClearObjects : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ClearObjects()
> ``` 


---  
 #  GetObjectAtIndex : [anyhandle](../nada_base_types/anyhandle.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function GetObjectAtIndex(index : Integer) : AnyHandle
> ``` 


---  
 #  ObjectTransformGizmo : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ObjectTransformGizmo()
> ``` 


---  
 #  RemoveObject : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ||[anyhandle](../nada_base_types/anyhandle.md)| |
> ||[boolean](../nada_base_types/boolean.md)| |
> ``` lang=cpp, name=Nada
> function RemoveObject( : AnyHandle,  : Boolean)
> ``` 


---  
 #  SetOperationQueue : Void

> If set, this Gizmo will add operations for all modifications to cogs.
> |Name|Type|Description|
> |---|---|---|
> |opQueue|[operationqueue](operationqueue.md)| |
> ``` lang=cpp, name=Nada
> function SetOperationQueue(opQueue : OperationQueue)
> ``` 


---  
 #  ToggleCoordinateMode : Void

> Toggle between local / world.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ToggleCoordinateMode()
> ``` 


---  
 

 
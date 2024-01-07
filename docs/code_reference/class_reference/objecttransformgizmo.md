 `Component` `Editor`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddObject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objecttransformgizmo.md#addobject-void)|[ Basis](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objecttransformgizmo.md#basis-zilch-engine-docume)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)|[objectrotategizmo](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objectrotategizmo.md)|
|[ ClearObjects](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objecttransformgizmo.md#clearobjects-void)|[ ObjectCount](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objecttransformgizmo.md#objectcount-zilch-engine)| |[objectscalegizmo](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objectscalegizmo.md)|
|[ GetObjectAtIndex](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objecttransformgizmo.md#getobjectatindex-zilch-en)|[ Pivot](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objecttransformgizmo.md#pivot-zilch-engine-docume)| |[objecttranslategizmo](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objecttranslategizmo.md)|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objecttransformgizmo.md#objecttransformgizmo-voi)| | | |
|[ RemoveObject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objecttransformgizmo.md#removeobject-void)| | | |
|[ SetOperationQueue](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objecttransformgizmo.md#setoperationqueue-void)| | | |
|[ ToggleCoordinateMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objecttransformgizmo.md#togglecoordinatemode-voi)| | | |


 #  Properties


---  
 #  Basis : [GizmoBasis](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#gizmobasis)

> Setters / Getters.
> ``` lang=cpp, name=Nada
> var Basis : GizmoBasis


---  
 #  ObjectCount : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Object getters.
> ``` lang=cpp, name=Nada
> var ObjectCount : Integer


---  
 #  Pivot : [GizmoPivot](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#gizmopivot)

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
> ||[anyhandle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/anyhandle.md)| |
> ||[boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)| |
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
 #  GetObjectAtIndex : [anyhandle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/anyhandle.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
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
> ||[anyhandle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/anyhandle.md)| |
> ||[boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)| |
> ``` lang=cpp, name=Nada
> function RemoveObject( : AnyHandle,  : Boolean)
> ``` 


---  
 #  SetOperationQueue : Void

> If set, this Gizmo will add operations for all modifications to cogs.
> |Name|Type|Description|
> |---|---|---|
> |opQueue|[operationqueue](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/operationqueue.md)| |
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
 

 
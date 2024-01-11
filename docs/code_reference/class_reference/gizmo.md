 `Component` `Editor`



(NOTE) Registers itself with the GizmoSpace. This allows GizmoSpace to keep track of which Gizmo the mouse is over, as well as send other input events directly to Gizmos.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](gizmo.md#gizmo-void)|[ Active](gizmo.md#active-zilch-engine-docum)|[component](component.md)| |
| |[ EditingObject](gizmo.md#editingobject-zilch-engin)| | |
| |[ ForwardEventsToChildren](gizmo.md#forwardeventstochildren)| | |
| |[ MouseOver](gizmo.md#mouseover-zilch-engine-do)| | |


 #  Properties


---  
 #  Active : [boolean](../nada_base_types/boolean.md)

> If set to false, it will not receive input events.
> ```TS:Nada
> var Active : Boolean


---  
 #  EditingObject : [cog](cog.md)

 `read-only`

> Needed?
> ```TS:Nada
> var EditingObject : Cog


---  
 #  ForwardEventsToChildren : [boolean](../nada_base_types/boolean.md)

> You may want to manually forward the input events to specific children.
> ```TS:Nada
> var ForwardEventsToChildren : Boolean


---  
 #  MouseOver : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Whether or not the mouse is currently over the gizmo.
> ```TS:Nada
> var MouseOver : Boolean


---  
 #  Methods


---  
 #  Gizmo : Void

 `constructor`

> Constructor.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Gizmo()
> ``` 


---  
 

 
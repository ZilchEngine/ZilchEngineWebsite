 `Component` `Physics`



(NOTE) Regions are used to make PhysicsEffects affect a region of space. Any effects attached to a Cog with a Region will apply to all objects in contact with this region.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ DispatchEvent](region.md#dispatchevent-void)|[ WakeUpOnEffectChange](region.md#wakeuponeffectchange-zer)|[component](component.md)| |
|[ Constructor](region.md#region-void)| | | |


 #  Properties


---  
 #  WakeUpOnEffectChange : [boolean](../nada_base_types/boolean.md)

> Determines if all objects in the region should be woken up when an effect is changed. Used to make sure that changes in effects will be applied to an object event if it is asleep.
> ```TS:Nada
> var WakeUpOnEffectChange : Boolean


---  
 #  Methods


---  
 #  DispatchEvent : Void

> Dispatches an event to all objects in this region.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](../nada_base_types/string.md)| |
> |toSend|[event](event.md)| |
> ```TS:Nada
> function DispatchEvent(eventId : String, toSend : Event)
> ``` 


---  
 #  Region : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Region()
> ``` 


---  
 

 
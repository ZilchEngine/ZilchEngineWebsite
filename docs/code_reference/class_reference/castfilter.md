 `Physics`

(NOTE) Filter for casting operations in physics. Allows basic filtering such as static or dynamic objects, advanced filters such as collision groups, and custom filters via an event callback.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](castfilter.md#castfilter-void)|[CallbackEventName](castfilter.md#callbackeventname-zilch-e)|[basecastfilter](basecastfilter.md)| |
| |[CallbackObject](castfilter.md#callbackobject-object)| | |
| |[CollisionGroup](castfilter.md#collisiongroup-zilch-engi)| | |
| |[IgnoreCog](castfilter.md#ignorecog-zilch-engine-do)| | |


 #  Properties


---  
 #  CallbackEventName : [string](../nada_base_types/string.md)

> The name of the event to invoke on the callback object.
> ```TS:Nada
> var CallbackEventName : String


---  
 #  CallbackObject : Object

> An object to invoke a callback on (via the callback name) to see if an object in a cast should be skipped.
> ```TS:Nada
> var CallbackObject : Object


---  
 #  CollisionGroup : [collisiongroup](collisiongroup.md)

> Should this cast behave like it belongs to a collision group? Uses the current space's CollisionTable for filtering logic.
> ```TS:Nada
> var CollisionGroup : CollisionGroup


---  
 #  IgnoreCog : [cog](cog.md)

> A cog to ignore during casts.
> ```TS:Nada
> var IgnoreCog : Cog


---  
 #  Methods


---  
 #  CastFilter : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function CastFilter()
> ``` 


---  
 #  CastFilter : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ||[castfilter](castfilter.md)| |
> ```TS:Nada
> function CastFilter( : CastFilter)
> ``` 


---  
 

 
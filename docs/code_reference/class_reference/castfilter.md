 `Physics`

(NOTE) Filter for casting operations in physics. Allows basic filtering such as static or dynamic objects, advanced filters such as collision groups, and custom filters via an event callback.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castfilter.md#castfilter-void)|[ CallbackEventName](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castfilter.md#callbackeventname-zilch-e)|[basecastfilter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/basecastfilter.md)| |
| |[ CallbackObject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castfilter.md#callbackobject-object)| | |
| |[ CollisionGroup](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castfilter.md#collisiongroup-zilch-engi)| | |
| |[ IgnoreCog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castfilter.md#ignorecog-zilch-engine-do)| | |


 #  Properties


---  
 #  CallbackEventName : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> The name of the event to invoke on the callback object.
> ``` lang=cpp, name=Nada
> var CallbackEventName : String


---  
 #  CallbackObject : Object

> An object to invoke a callback on (via the callback name) to see if an object in a cast should be skipped.
> ``` lang=cpp, name=Nada
> var CallbackObject : Object


---  
 #  CollisionGroup : [collisiongroup](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisiongroup.md)

> Should this cast behave like it belongs to a collision group? Uses the current space's CollisionTable for filtering logic.
> ``` lang=cpp, name=Nada
> var CollisionGroup : CollisionGroup


---  
 #  IgnoreCog : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> A cog to ignore during casts.
> ``` lang=cpp, name=Nada
> var IgnoreCog : Cog


---  
 #  Methods


---  
 #  CastFilter : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function CastFilter()
> ``` 


---  
 #  CastFilter : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ||[castfilter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castfilter.md)| |
> ``` lang=cpp, name=Nada
> function CastFilter( : CastFilter)
> ``` 


---  
 

 
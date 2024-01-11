 `Physics`

(NOTE) Used to specify which collision group events should be sent out for a CollisionFilter. Allows customizing who gets events (in the filter pair) and what event name is sent out.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ BlockType](collisionfilterblock.md#blocktype-zilch-engine-do)|[safeid32object](safeid32object.md)|[collisionendblock](collisionendblock.md)|
| |[ EventOverride](collisionfilterblock.md#eventoverride-zilch-engin)| |[collisionpersistedblock](collisionpersistedblock.md)|
| |[ SendEventsToA](collisionfilterblock.md#sendeventstoa-zilch-engin)| |[collisionstartblock](collisionstartblock.md)|
| |[ SendEventsToB](collisionfilterblock.md#sendeventstob-zilch-engin)| |[presolveblock](presolveblock.md)|
| |[ SendEventsToSpace](collisionfilterblock.md#sendeventstospace-zilch-e)| | |


 #  Properties


---  
 #  BlockType : [CollisionFilterBlockType](../enum_reference.md#collisionfilterblocktype)

 `read-only`

> What type of collision filter block is this?
> ``` lang=cpp, name=Nada
> var BlockType : CollisionFilterBlockType


---  
 #  EventOverride : [string](../nada_base_types/string.md)

> What event name to send out when this block triggers. If left empty the default name will be used (e.g. GroupCollisionStarted).
> ``` lang=cpp, name=Nada
> var EventOverride : String


---  
 #  SendEventsToA : [boolean](../nada_base_types/boolean.md)

> Does the first object in the filter get this event type sent to it?
> ``` lang=cpp, name=Nada
> var SendEventsToA : Boolean


---  
 #  SendEventsToB : [boolean](../nada_base_types/boolean.md)

> Does the second object in the filter get this event type sent to it?
> ``` lang=cpp, name=Nada
> var SendEventsToB : Boolean


---  
 #  SendEventsToSpace : [boolean](../nada_base_types/boolean.md)

> Does the active space of the objects get this event type sent to it?
> ``` lang=cpp, name=Nada
> var SendEventsToSpace : Boolean


---  
 #  Methods


---  
 

 
 `Physics`

(NOTE) Used to specify which collision group events should be sent out for a CollisionFilter. Allows customizing who gets events (in the filter pair) and what event name is sent out.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ BlockType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisionfilterblock.md#blocktype-zilch-engine-do)|[safeid32object](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/safeid32object.md)|[collisionendblock](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisionendblock.md)|
| |[ EventOverride](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisionfilterblock.md#eventoverride-zilch-engin)| |[collisionpersistedblock](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisionpersistedblock.md)|
| |[ SendEventsToA](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisionfilterblock.md#sendeventstoa-zilch-engin)| |[collisionstartblock](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisionstartblock.md)|
| |[ SendEventsToB](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisionfilterblock.md#sendeventstob-zilch-engin)| |[presolveblock](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/presolveblock.md)|
| |[ SendEventsToSpace](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisionfilterblock.md#sendeventstospace-zilch-e)| | |


 #  Properties


---  
 #  BlockType : [CollisionFilterBlockType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#collisionfilterblocktype)

 `read-only`

> What type of collision filter block is this?
> ``` lang=cpp, name=Nada
> var BlockType : CollisionFilterBlockType


---  
 #  EventOverride : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> What event name to send out when this block triggers. If left empty the default name will be used (e.g. GroupCollisionStarted).
> ``` lang=cpp, name=Nada
> var EventOverride : String


---  
 #  SendEventsToA : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Does the first object in the filter get this event type sent to it?
> ``` lang=cpp, name=Nada
> var SendEventsToA : Boolean


---  
 #  SendEventsToB : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Does the second object in the filter get this event type sent to it?
> ``` lang=cpp, name=Nada
> var SendEventsToB : Boolean


---  
 #  SendEventsToSpace : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Does the active space of the objects get this event type sent to it?
> ``` lang=cpp, name=Nada
> var SendEventsToSpace : Boolean


---  
 #  Methods


---  
 

 
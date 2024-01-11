 `Event` `Physics`



(NOTE) Sent by CustomJoint before solving constraints. Used to configure constraints before the physics system begins solving.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ Dt](customjointevent.md#dt-zilch-engine-documenta)|[event](event.md)| |
| |[ Owner](customjointevent.md#owner-zilch-engine-docume)| | |


 #  Properties


---  
 #  Dt : [real](../nada_base_types/real.md)

> The current frame's delta time. Use to setup the constraint if necessary.
> ``` lang=cpp, name=Nada
> var Dt : Real


---  
 #  Owner : [customjoint](customjoint.md)

> The joint that sent this event.
> ``` lang=cpp, name=Nada
> var Owner : CustomJoint


---  
 #  Methods


---  
 

 
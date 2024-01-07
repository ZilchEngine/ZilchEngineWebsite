 `Event` `Physics`



(NOTE) Sent by CustomJoint before solving constraints. Used to configure constraints before the physics system begins solving.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ Dt](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customjointevent.md#dt-zilch-engine-documenta)|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
| |[ Owner](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customjointevent.md#owner-zilch-engine-docume)| | |


 #  Properties


---  
 #  Dt : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The current frame's delta time. Use to setup the constraint if necessary.
> ``` lang=cpp, name=Nada
> var Dt : Real


---  
 #  Owner : [customjoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customjoint.md)

> The joint that sent this event.
> ``` lang=cpp, name=Nada
> var Owner : CustomJoint


---  
 #  Methods


---  
 

 
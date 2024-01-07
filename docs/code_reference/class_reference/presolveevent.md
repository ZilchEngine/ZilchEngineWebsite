 `Event` `Physics`



(NOTE) Event sent out when a CollisionFilter contains a PreSolveBlock. This event is sent out after collision detection but before collision resolution. This can be used to alter the state of the two objects in a collision before they're resolved (e.g. turn one from static to dynamic). Warning: Do not delete objects or do any other significant changes as this may destabilize the system.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ Friction](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/presolveevent.md#friction-zilch-engine-doc)|[basecollisionevent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/basecollisionevent.md)| |
| |[ Restitution](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/presolveevent.md#restitution-zilch-engine)| | |


 #  Properties


---  
 #  Friction : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The friction to use for solving this pair. Allows custom overriding for this pair.
> ``` lang=cpp, name=Nada
> var Friction : Real


---  
 #  Restitution : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The restitution to use for solving this pair. Allows custom overriding for this pair.
> ``` lang=cpp, name=Nada
> var Restitution : Real


---  
 #  Methods


---  
 

 
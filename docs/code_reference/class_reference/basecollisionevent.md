 `Event` `Physics`



(NOTE) Common interface for all collision events. Contains shared methods to access contact information for a collision.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ ContactPointCount](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/basecollisionevent.md#contactpointcount-zilch-e)|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)|[collisionevent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisionevent.md)|
| |[ ContactPoints](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/basecollisionevent.md#contactpoints-zilch-engin)| |[collisiongroupevent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisiongroupevent.md)|
| |[ IsGhost](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/basecollisionevent.md#isghost-zilch-engine-docu)| |[presolveevent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/presolveevent.md)|
| |[ Object](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/basecollisionevent.md#object-zilch-engine-docum)| | |
| |[ OtherObject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/basecollisionevent.md#otherobject-zilch-engine)| | |


 #  Properties


---  
 #  ContactPointCount : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> The number of contact points in this collision.
> ``` lang=cpp, name=Nada
> var ContactPointCount : Integer


---  
 #  ContactPoints : [contactpointrange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contactpointrange.md)

 `read-only`

> A range for iterating through all contact points.
> ``` lang=cpp, name=Nada
> var ContactPoints : ContactPointRange


---  
 #  IsGhost : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> If this was a ghost collision (detected but not resolved).
> ``` lang=cpp, name=Nada
> var IsGhost : Boolean


---  
 #  Object : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

 `read-only`

> The object that this event was sent to.
> ``` lang=cpp, name=Nada
> var Object : Cog


---  
 #  OtherObject : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

 `read-only`

> The other object in this collision.
> ``` lang=cpp, name=Nada
> var OtherObject : Cog


---  
 #  Methods


---  
 

 
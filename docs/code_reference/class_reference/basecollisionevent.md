 `Event` `Physics`



(NOTE) Common interface for all collision events. Contains shared methods to access contact information for a collision.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ContactPointCount](basecollisionevent.md#contactpointcount-zilch-e)|[event](event.md)|[collisionevent](collisionevent.md)|
| |[ContactPoints](basecollisionevent.md#contactpoints-zilch-engin)| |[collisiongroupevent](collisiongroupevent.md)|
| |[IsGhost](basecollisionevent.md#isghost-zilch-engine-docu)| |[presolveevent](presolveevent.md)|
| |[Object](basecollisionevent.md#object-zilch-engine-docum)| | |
| |[OtherObject](basecollisionevent.md#otherobject-zilch-engine)| | |


 #  Properties


---  
 #  ContactPointCount : [integer](../nada_base_types/integer.md)

 `read-only`

> The number of contact points in this collision.
> ```TS:Nada
> var ContactPointCount : Integer


---  
 #  ContactPoints : [contactpointrange](contactpointrange.md)

 `read-only`

> A range for iterating through all contact points.
> ```TS:Nada
> var ContactPoints : ContactPointRange


---  
 #  IsGhost : [boolean](../nada_base_types/boolean.md)

 `read-only`

> If this was a ghost collision (detected but not resolved).
> ```TS:Nada
> var IsGhost : Boolean


---  
 #  Object : [cog](cog.md)

 `read-only`

> The object that this event was sent to.
> ```TS:Nada
> var Object : Cog


---  
 #  OtherObject : [cog](cog.md)

 `read-only`

> The other object in this collision.
> ```TS:Nada
> var OtherObject : Cog


---  
 #  Methods


---  
 

 
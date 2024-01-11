 `Physics`

(NOTE) A bi-directional graph edge between a collider and a contact. Exposes some internals to Contact which currently can't be exposed.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](contactgraphedge.md#contactgraphedge-void)|[ ContactPointCount](contactgraphedge.md#contactpointcount-zilch-e)|BaseConstraintGraphEdge<Physics::Contact,Physics::ContactEdge>| |
| |[ ContactPoints](contactgraphedge.md#contactpoints-zilch-engin)| | |
| |[ FirstPoint](contactgraphedge.md#firstpoint-zilch-engine-d)| | |
| |[ IsGhost](contactgraphedge.md#isghost-zilch-engine-docu)| | |
| |[ Object](contactgraphedge.md#object-zilch-engine-docum)| | |
| |[ OtherObject](contactgraphedge.md#otherobject-zilch-engine)| | |


 #  Properties


---  
 #  ContactPointCount : [integer](../nada_base_types/integer.md)

 `read-only`

> How many points of contact were in this collision.
> ```TS:Nada
> var ContactPointCount : Integer


---  
 #  ContactPoints : [contactpointrange](contactpointrange.md)

 `read-only`

> Returns a range of all contact points in the collision.
> ```TS:Nada
> var ContactPoints : ContactPointRange


---  
 #  FirstPoint : [contactpoint](contactpoint.md)

 `read-only`

> Convenience function to return the first ContactPoint. Some logic only cares about one point of information. In a more general case all points should be iterated over.
> ```TS:Nada
> var FirstPoint : ContactPoint


---  
 #  IsGhost : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Was this a ghost collision?
> ```TS:Nada
> var IsGhost : Boolean


---  
 #  Object : [cog](cog.md)

 `read-only`

> 
> ```TS:Nada
> var Object : Cog


---  
 #  OtherObject : [cog](cog.md)

 `read-only`

> 
> ```TS:Nada
> var OtherObject : Cog


---  
 #  Methods


---  
 #  ContactGraphEdge : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ContactGraphEdge()
> ``` 


---  
 #  ContactGraphEdge : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ||[contactgraphedge](contactgraphedge.md)| |
> ```TS:Nada
> function ContactGraphEdge( : ContactGraphEdge)
> ``` 


---  
 

 
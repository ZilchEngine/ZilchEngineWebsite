 `Physics`

(NOTE) A bi-directional graph edge between a collider and a contact. Exposes some internals to Contact which currently can't be exposed.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contactgraphedge.md#contactgraphedge-void)|[ ContactPointCount](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contactgraphedge.md#contactpointcount-zilch-e)|BaseConstraintGraphEdge<Physics::Contact,Physics::ContactEdge>| |
| |[ ContactPoints](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contactgraphedge.md#contactpoints-zilch-engin)| | |
| |[ FirstPoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contactgraphedge.md#firstpoint-zilch-engine-d)| | |
| |[ IsGhost](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contactgraphedge.md#isghost-zilch-engine-docu)| | |
| |[ Object](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contactgraphedge.md#object-zilch-engine-docum)| | |
| |[ OtherObject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contactgraphedge.md#otherobject-zilch-engine)| | |


 #  Properties


---  
 #  ContactPointCount : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> How many points of contact were in this collision.
> ``` lang=cpp, name=Nada
> var ContactPointCount : Integer


---  
 #  ContactPoints : [contactpointrange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contactpointrange.md)

 `read-only`

> Returns a range of all contact points in the collision.
> ``` lang=cpp, name=Nada
> var ContactPoints : ContactPointRange


---  
 #  FirstPoint : [contactpoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contactpoint.md)

 `read-only`

> Convenience function to return the first ContactPoint. Some logic only cares about one point of information. In a more general case all points should be iterated over.
> ``` lang=cpp, name=Nada
> var FirstPoint : ContactPoint


---  
 #  IsGhost : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> Was this a ghost collision?
> ``` lang=cpp, name=Nada
> var IsGhost : Boolean


---  
 #  Object : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Object : Cog


---  
 #  OtherObject : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var OtherObject : Cog


---  
 #  Methods


---  
 #  ContactGraphEdge : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ContactGraphEdge()
> ``` 


---  
 #  ContactGraphEdge : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ||[contactgraphedge](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contactgraphedge.md)| |
> ``` lang=cpp, name=Nada
> function ContactGraphEdge( : ContactGraphEdge)
> ``` 


---  
 

 
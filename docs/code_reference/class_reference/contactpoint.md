 `Physics`



(NOTE) Information about one point of contact in a collision. This is useful for evaluating info about the collision after it happened such as where the objects hit. WARNING: Do not hold onto this after an event is sent out.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contactpoint.md#contactpoint-void)|[ ComplexImpulse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contactpoint.md#compleximpulse-zilch-engi)| | |
| |[ FrictionImpulse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contactpoint.md#frictionimpulse-zilch-eng)| | |
| |[ LocalPoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contactpoint.md#localpoint-zilch-engine-d)| | |
| |[ NormalImpulse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contactpoint.md#normalimpulse-zilch-engin)| | |
| |[ OtherLocalPoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contactpoint.md#otherlocalpoint-zilch-eng)| | |
| |[ Penetration](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contactpoint.md#penetration-zilch-engine)| | |
| |[ RelativeVelocity](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contactpoint.md#relativevelocity-zilch-en)| | |
| |[ WorldNormalTowardsOther](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contactpoint.md#worldnormaltowardsother)| | |
| |[ WorldPoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contactpoint.md#worldpoint-zilch-engine-d)| | |


 #  Properties


---  
 #  ComplexImpulse : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

 `read-only`

> The total impulse this object applied (only for more complicated logic). The impulse is a Vector3 of the values (normal, friction1, friction2).
> ``` lang=cpp, name=Nada
> var ComplexImpulse : Real3


---  
 #  FrictionImpulse : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

 `read-only`

> The total friction impulse that this object applied.
> ``` lang=cpp, name=Nada
> var FrictionImpulse : Real


---  
 #  LocalPoint : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

 `read-only`

> The point in local space of myself in this collision.
> ``` lang=cpp, name=Nada
> var LocalPoint : Real3


---  
 #  NormalImpulse : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

 `read-only`

> The total impulse that this object applied in the direction of the normal.
> ``` lang=cpp, name=Nada
> var NormalImpulse : Real


---  
 #  OtherLocalPoint : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

 `read-only`

> The point in local space of the other object in this collision.
> ``` lang=cpp, name=Nada
> var OtherLocalPoint : Real3


---  
 #  Penetration : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

 `read-only`

> The penetration of this contact point in the direction of the normal. Note: penetration is always positive and is not flipped for object A or object B.
> ``` lang=cpp, name=Nada
> var Penetration : Real


---  
 #  RelativeVelocity : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

 `read-only`

> The relative velocity of this point in the direction of the normal. The relative point velocity is defined as Dot(p1 - p0, n) where p1 and p0 are the velocities of the contact points in the collision of myself and the other object respectively. This value can be used to see how fast the objects are now separating. Also, in pre-collision this value can be used to approximate the impulse of the collision since the impulse values will not have been calculated yet in pre-collision.
> ``` lang=cpp, name=Nada
> var RelativeVelocity : Real


---  
 #  WorldNormalTowardsOther : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

 `read-only`

> The world space normal that points from myself towards the other object.
> ``` lang=cpp, name=Nada
> var WorldNormalTowardsOther : Real3


---  
 #  WorldPoint : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

 `read-only`

> The point in world space of this contact point.
> ``` lang=cpp, name=Nada
> var WorldPoint : Real3


---  
 #  Methods


---  
 #  ContactPoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ContactPoint()
> ``` 


---  
 #  ContactPoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ||[contactpoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contactpoint.md)| |
> ``` lang=cpp, name=Nada
> function ContactPoint( : ContactPoint)
> ``` 


---  
 

 
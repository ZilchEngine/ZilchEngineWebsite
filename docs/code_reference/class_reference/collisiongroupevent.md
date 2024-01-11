 `Event` `Physics`



(NOTE) An event sent out when specified by a CollisionFilter in a CollisionTable. Used to hook up events based upon certain CollisionGroup types colliding.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ FirstPoint](collisiongroupevent.md#firstpoint-zilch-engine-d)|[basecollisionevent](basecollisionevent.md)| |
| |[ TypeAName](collisiongroupevent.md#typeaname-zilch-engine-do)| | |
| |[ TypeBName](collisiongroupevent.md#typebname-zilch-engine-do)| | |


 #  Properties


---  
 #  FirstPoint : [contactpoint](contactpoint.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var FirstPoint : ContactPoint


---  
 #  TypeAName : [string](../nada_base_types/string.md)

 `read-only`

> Returns the CollisionGroup name of object A.
> ``` lang=cpp, name=Nada
> var TypeAName : String


---  
 #  TypeBName : [string](../nada_base_types/string.md)

 `read-only`

> Returns the CollisionGroup name of object B.
> ``` lang=cpp, name=Nada
> var TypeBName : String


---  
 #  Methods


---  
 

 
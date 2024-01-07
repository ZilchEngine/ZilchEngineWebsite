 `Event` `Physics`



(NOTE) An event sent out when specified by a CollisionFilter in a CollisionTable. Used to hook up events based upon certain CollisionGroup types colliding.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ FirstPoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisiongroupevent.md#firstpoint-zilch-engine-d)|[basecollisionevent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/basecollisionevent.md)| |
| |[ TypeAName](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisiongroupevent.md#typeaname-zilch-engine-do)| | |
| |[ TypeBName](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisiongroupevent.md#typebname-zilch-engine-do)| | |


 #  Properties


---  
 #  FirstPoint : [contactpoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contactpoint.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var FirstPoint : ContactPoint


---  
 #  TypeAName : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

 `read-only`

> Returns the CollisionGroup name of object A.
> ``` lang=cpp, name=Nada
> var TypeAName : String


---  
 #  TypeBName : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

 `read-only`

> Returns the CollisionGroup name of object B.
> ``` lang=cpp, name=Nada
> var TypeBName : String


---  
 #  Methods


---  
 

 
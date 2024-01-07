 `Event` `Physics`



(NOTE) Allows a user to filter out an object during any cast in physics.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ FilterState](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castfilterevent.md#filterstate-zilch-engine)|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
| |[ Object](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castfilterevent.md#object-zilch-engine-docum)| | |


 #  Properties


---  
 #  FilterState : [CastFilterState](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#castfilterstate)

> When filtering should we accept or reject this cog? Alternatively we can let the default cast filter logic run.
> ``` lang=cpp, name=Nada
> var FilterState : CastFilterState


---  
 #  Object : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

 `read-only`

> The object being tested in this cast.
> ``` lang=cpp, name=Nada
> var Object : Cog


---  
 #  Methods


---  
 

 
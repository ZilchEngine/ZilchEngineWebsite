 `Component` `Physics`



(NOTE) Joints connect two objects together with one or more constraints. A constraint is a mathematical rule that restricts object movement, typically defined in terms of the position and velocities of the objects involved.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetCog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/joint.md#getcog-zilch-engine-docum)|[ Active](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/joint.md#active-zilch-engine-docum)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)|[customjoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customjoint.md)|
|[ GetOtherObject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/joint.md#getotherobject-zilch-engi)|[ AutoSnaps](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/joint.md#autosnaps-zilch-engine-do)| |[fixedanglejoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/fixedanglejoint.md)|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/joint.md#joint-void)|[ CollideConnected](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/joint.md#collideconnected-zilch-en)| |[gearjoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gearjoint.md)|
| |[ MaxImpulse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/joint.md#maximpulse-zilch-engine-d)| |[linearaxisjoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/linearaxisjoint.md)|
| |[ SendsEvents](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/joint.md#sendsevents-zilch-engine)| |[manipulatorjoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/manipulatorjoint.md)|
| | | |[phygunjoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/phygunjoint.md)|
| | | |[positionjoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/positionjoint.md)|
| | | |[prismaticjoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/prismaticjoint.md)|
| | | |[prismaticjoint2d](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/prismaticjoint2d.md)|
| | | |[pulleyjoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/pulleyjoint.md)|
| | | |[relativevelocityjoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/relativevelocityjoint.md)|
| | | |[revolutejoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/revolutejoint.md)|
| | | |[revolutejoint2d](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/revolutejoint2d.md)|
| | | |[stickjoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/stickjoint.md)|
| | | |[universaljoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/universaljoint.md)|
| | | |[uprightjoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uprightjoint.md)|
| | | |[weldjoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/weldjoint.md)|
| | | |[wheeljoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/wheeljoint.md)|
| | | |[wheeljoint2d](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/wheeljoint2d.md)|


 #  Properties


---  
 #  Active : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Determines if this joint is currently active. Used for runtime enabling/disabling of joints.
> ``` lang=cpp, name=Nada
> var Active : Boolean


---  
 #  AutoSnaps : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Determines if this joint will automatically delete itself if any of its constraints reach the max impulse value. This will still send an event if it snaps.
> ``` lang=cpp, name=Nada
> var AutoSnaps : Boolean


---  
 #  CollideConnected : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Determines if the two objects connected by this joint can collide. If any joint between this pair does not collide, then the pair does not collide. All joints have to be set to true in order to have the objects collide.
> ``` lang=cpp, name=Nada
> var CollideConnected : Boolean


---  
 #  MaxImpulse : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The maximum impulse (instantaneous force) that this joint can apply to correct itself.
> ``` lang=cpp, name=Nada
> var MaxImpulse : Real


---  
 #  SendsEvents : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Determines if this joint will send any events. Used for a small efficiency boost and for reducing the number of events.
> ``` lang=cpp, name=Nada
> var SendsEvents : Boolean


---  
 #  Methods


---  
 #  GetCog : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> Returns the cog associated with an index. Index of 0 is ObjectA, index 1 is ObjectB. Used to write more streamline functions where you index into the objects in a loop.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function GetCog(index : Integer) : Cog
> ``` 


---  
 #  GetOtherObject : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> If the passed in object is ObjectA, returns ObjectB. Provides easier logic for traversing across joints.
> |Name|Type|Description|
> |---|---|---|
> |cog|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Nada
> function GetOtherObject(cog : Cog) : Cog
> ``` 


---  
 #  Joint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Joint()
> ``` 


---  
 

 
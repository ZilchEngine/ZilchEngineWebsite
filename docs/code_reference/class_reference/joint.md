 `Component` `Physics`



(NOTE) Joints connect two objects together with one or more constraints. A constraint is a mathematical rule that restricts object movement, typically defined in terms of the position and velocities of the objects involved.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetCog](joint.md#getcog-zilch-engine-docum)|[ Active](joint.md#active-zilch-engine-docum)|[component](component.md)|[customjoint](customjoint.md)|
|[ GetOtherObject](joint.md#getotherobject-zilch-engi)|[ AutoSnaps](joint.md#autosnaps-zilch-engine-do)| |[fixedanglejoint](fixedanglejoint.md)|
|[ Constructor](joint.md#joint-void)|[ CollideConnected](joint.md#collideconnected-zilch-en)| |[gearjoint](gearjoint.md)|
| |[ MaxImpulse](joint.md#maximpulse-zilch-engine-d)| |[linearaxisjoint](linearaxisjoint.md)|
| |[ SendsEvents](joint.md#sendsevents-zilch-engine)| |[manipulatorjoint](manipulatorjoint.md)|
| | | |[phygunjoint](phygunjoint.md)|
| | | |[positionjoint](positionjoint.md)|
| | | |[prismaticjoint](prismaticjoint.md)|
| | | |[prismaticjoint2d](prismaticjoint2d.md)|
| | | |[pulleyjoint](pulleyjoint.md)|
| | | |[relativevelocityjoint](relativevelocityjoint.md)|
| | | |[revolutejoint](revolutejoint.md)|
| | | |[revolutejoint2d](revolutejoint2d.md)|
| | | |[stickjoint](stickjoint.md)|
| | | |[universaljoint](universaljoint.md)|
| | | |[uprightjoint](uprightjoint.md)|
| | | |[weldjoint](weldjoint.md)|
| | | |[wheeljoint](wheeljoint.md)|
| | | |[wheeljoint2d](wheeljoint2d.md)|


 #  Properties


---  
 #  Active : [boolean](../nada_base_types/boolean.md)

> Determines if this joint is currently active. Used for runtime enabling/disabling of joints.
> ```TS:Nada
> var Active : Boolean


---  
 #  AutoSnaps : [boolean](../nada_base_types/boolean.md)

> Determines if this joint will automatically delete itself if any of its constraints reach the max impulse value. This will still send an event if it snaps.
> ```TS:Nada
> var AutoSnaps : Boolean


---  
 #  CollideConnected : [boolean](../nada_base_types/boolean.md)

> Determines if the two objects connected by this joint can collide. If any joint between this pair does not collide, then the pair does not collide. All joints have to be set to true in order to have the objects collide.
> ```TS:Nada
> var CollideConnected : Boolean


---  
 #  MaxImpulse : [real](../nada_base_types/real.md)

> The maximum impulse (instantaneous force) that this joint can apply to correct itself.
> ```TS:Nada
> var MaxImpulse : Real


---  
 #  SendsEvents : [boolean](../nada_base_types/boolean.md)

> Determines if this joint will send any events. Used for a small efficiency boost and for reducing the number of events.
> ```TS:Nada
> var SendsEvents : Boolean


---  
 #  Methods


---  
 #  GetCog : [cog](cog.md)

> Returns the cog associated with an index. Index of 0 is ObjectA, index 1 is ObjectB. Used to write more streamline functions where you index into the objects in a loop.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function GetCog(index : Integer) : Cog
> ``` 


---  
 #  GetOtherObject : [cog](cog.md)

> If the passed in object is ObjectA, returns ObjectB. Provides easier logic for traversing across joints.
> |Name|Type|Description|
> |---|---|---|
> |cog|[cog](cog.md)| |
> ```TS:Nada
> function GetOtherObject(cog : Cog) : Cog
> ``` 


---  
 #  Joint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Joint()
> ``` 


---  
 

 
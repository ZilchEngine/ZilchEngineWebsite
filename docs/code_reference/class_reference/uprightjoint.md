 `Component` `Physics`



(NOTE) A joint to keep an object upright. Locks two axes of the objects together but allows free rotation on the plane defined by that axis. This constraint is useful for keeping any object upright. This could also be used to auto correct an object slowly by lowering the max impulse value of the constraint.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](uprightjoint.md#uprightjoint-void)|[LocalAxisA](uprightjoint.md#localaxisa-zilch-engine-d)|[joint](joint.md)| |
| |[LocalAxisB](uprightjoint.md#localaxisb-zilch-engine-d)| | |
| |[WorldAxis](uprightjoint.md#worldaxis-zilch-engine-do)| | |


 #  Properties


---  
 #  LocalAxisA : [real3](../nada_base_types/real3.md)

> The locally defined axis on object A . 
> ```TS:Nada
> var LocalAxisA : Real3


---  
 #  LocalAxisB : [real3](../nada_base_types/real3.md)

> The locally defined axis on object B . 
> ```TS:Nada
> var LocalAxisB : Real3


---  
 #  WorldAxis : [real3](../nada_base_types/real3.md)

> The axis in world space that is being rotated about . 
> ```TS:Nada
> var WorldAxis : Real3


---  
 #  Methods


---  
 #  UprightJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function UprightJoint()
> ``` 


---  
 

 
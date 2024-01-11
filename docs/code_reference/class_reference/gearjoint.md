 `Component` `Physics`



(NOTE) A gear connects two joints on two objects together. Either joint can be a prismatic or a revolute. A gear ratio is used to bind the two joints together. Limits, motors, and springs should not be used on this.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](gearjoint.md#gearjoint-void)|[ Constant](gearjoint.md#constant-zilch-engine-doc)|[joint](joint.md)| |
| |[ JointA](gearjoint.md#jointa-zilch-engine-docum)| | |
| |[ JointAPath](gearjoint.md#jointapath-zilch-engine-d)| | |
| |[ JointB](gearjoint.md#jointb-zilch-engine-docum)| | |
| |[ JointBPath](gearjoint.md#jointbpath-zilch-engine-d)| | |
| |[ Ratio](gearjoint.md#ratio-zilch-engine-docume)| | |


 #  Properties


---  
 #  Constant : [real](../nada_base_types/real.md)

> The initial offset of the gear ratio.
> ``` lang=cpp, name=Nada
> var Constant : Real


---  
 #  JointA : [cog](cog.md)

> The joint connected to ObjectA that the gear operates on.
> ``` lang=cpp, name=Nada
> var JointA : Cog


---  
 #  JointAPath : [cogpath](cogpath.md)

> The joint connected to ObjectA that the gear operates on.
> ``` lang=cpp, name=Nada
> var JointAPath : CogPath


---  
 #  JointB : [cog](cog.md)

> The joint connected to ObjectB that the gear operates on.
> ``` lang=cpp, name=Nada
> var JointB : Cog


---  
 #  JointBPath : [cogpath](cogpath.md)

> The joint connected to ObjectB that the gear operates on.
> ``` lang=cpp, name=Nada
> var JointBPath : CogPath


---  
 #  Ratio : [real](../nada_base_types/real.md)

> The gear ratio that the two constraints are bound with.
> ``` lang=cpp, name=Nada
> var Ratio : Real


---  
 #  Methods


---  
 #  GearJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function GearJoint()
> ``` 


---  
 

 
 `Component` `Physics`



(NOTE) A gear connects two joints on two objects together. Either joint can be a prismatic or a revolute. A gear ratio is used to bind the two joints together. Limits, motors, and springs should not be used on this.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gearjoint.md#gearjoint-void)|[ Constant](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gearjoint.md#constant-zilch-engine-doc)|[joint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/joint.md)| |
| |[ JointA](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gearjoint.md#jointa-zilch-engine-docum)| | |
| |[ JointAPath](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gearjoint.md#jointapath-zilch-engine-d)| | |
| |[ JointB](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gearjoint.md#jointb-zilch-engine-docum)| | |
| |[ JointBPath](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gearjoint.md#jointbpath-zilch-engine-d)| | |
| |[ Ratio](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gearjoint.md#ratio-zilch-engine-docume)| | |


 #  Properties


---  
 #  Constant : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The initial offset of the gear ratio.
> ``` lang=cpp, name=Nada
> var Constant : Real


---  
 #  JointA : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> The joint connected to ObjectA that the gear operates on.
> ``` lang=cpp, name=Nada
> var JointA : Cog


---  
 #  JointAPath : [cogpath](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cogpath.md)

> The joint connected to ObjectA that the gear operates on.
> ``` lang=cpp, name=Nada
> var JointAPath : CogPath


---  
 #  JointB : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> The joint connected to ObjectB that the gear operates on.
> ``` lang=cpp, name=Nada
> var JointB : Cog


---  
 #  JointBPath : [cogpath](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cogpath.md)

> The joint connected to ObjectB that the gear operates on.
> ``` lang=cpp, name=Nada
> var JointBPath : CogPath


---  
 #  Ratio : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

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
 

 
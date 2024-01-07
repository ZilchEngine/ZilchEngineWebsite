 `Component` `Physics`



(NOTE) A PulleyJoint turns two StickJoints into a pulley via a pulley ratio. A PulleyJoint connects the two free objects of two different stick joints. These two objects will then be bound to move together via the formula "length0 + ratio * length1 = 0". Limits, motors and springs should not be used on a pulley.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/pulleyjoint.md#pulleyjoint-void)|[ JointA](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/pulleyjoint.md#jointa-zilch-engine-docum)|[joint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/joint.md)| |
| |[ JointAPath](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/pulleyjoint.md#jointapath-zilch-engine-d)| | |
| |[ JointB](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/pulleyjoint.md#jointb-zilch-engine-docum)| | |
| |[ JointBPath](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/pulleyjoint.md#jointbpath-zilch-engine-d)| | |
| |[ Ratio](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/pulleyjoint.md#ratio-zilch-engine-docume)| | |


 #  Properties


---  
 #  JointA : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> The joint connected to ObjectA that the pulley operates on.
> ``` lang=cpp, name=Nada
> var JointA : Cog


---  
 #  JointAPath : [cogpath](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cogpath.md)

> The joint connected to ObjectA that the pulley operates on.
> ``` lang=cpp, name=Nada
> var JointAPath : CogPath


---  
 #  JointB : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> The joint connected to ObjectB that the pulley operates on.
> ``` lang=cpp, name=Nada
> var JointB : Cog


---  
 #  JointBPath : [cogpath](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cogpath.md)

> The joint connected to ObjectB that the pulley operates on.
> ``` lang=cpp, name=Nada
> var JointBPath : CogPath


---  
 #  Ratio : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The ratio between the two stick joints. The ratio is used in the formula "length0 + ratio * length1 = 0".
> ``` lang=cpp, name=Nada
> var Ratio : Real


---  
 #  Methods


---  
 #  PulleyJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function PulleyJoint()
> ``` 


---  
 

 
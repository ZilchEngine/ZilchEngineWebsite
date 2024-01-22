 `Component` `Physics`



(NOTE) A PulleyJoint turns two StickJoints into a pulley via a pulley ratio. A PulleyJoint connects the two free objects of two different stick joints. These two objects will then be bound to move together via the formula "length0 + ratio * length1 = 0". Limits, motors and springs should not be used on a pulley.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](pulleyjoint.md#pulleyjoint-void)|[JointA](pulleyjoint.md#jointa-zilch-engine-docum)|[joint](joint.md)| |
| |[JointAPath](pulleyjoint.md#jointapath-zilch-engine-d)| | |
| |[JointB](pulleyjoint.md#jointb-zilch-engine-docum)| | |
| |[JointBPath](pulleyjoint.md#jointbpath-zilch-engine-d)| | |
| |[Ratio](pulleyjoint.md#ratio-zilch-engine-docume)| | |


 #  Properties


---  
 #  JointA : [cog](cog.md)

> The joint connected to ObjectA that the pulley operates on.
> ```TS:Nada
> var JointA : Cog


---  
 #  JointAPath : [cogpath](cogpath.md)

> The joint connected to ObjectA that the pulley operates on.
> ```TS:Nada
> var JointAPath : CogPath


---  
 #  JointB : [cog](cog.md)

> The joint connected to ObjectB that the pulley operates on.
> ```TS:Nada
> var JointB : Cog


---  
 #  JointBPath : [cogpath](cogpath.md)

> The joint connected to ObjectB that the pulley operates on.
> ```TS:Nada
> var JointBPath : CogPath


---  
 #  Ratio : [real](../nada_base_types/real.md)

> The ratio between the two stick joints. The ratio is used in the formula "length0 + ratio * length1 = 0".
> ```TS:Nada
> var Ratio : Real


---  
 #  Methods


---  
 #  PulleyJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function PulleyJoint()
> ``` 


---  
 

 
 `Component` `Physics`



(NOTE) A revolute joint is used to create a wheel or a hinge. A revolute joint bring the two locally defined axes together and allows free rotation only on that axis. This axis is also where the motor is applied. The two axes that are orthogonal to the motor axis have their rotation locked (objects rotate together unless on the motor axis). Add on definitions: Limit: A limit will provide a min/max angle on the motor axis. Zilch is defined by the location of the primary axis on the FrameOfreference object. Motor: A motor will drive the objects about the motor axis. Spring: A spring will make the motor axis springy at the limits.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](revolutejoint.md#revolutejoint-void)|[FrameOfReference](revolutejoint.md#frameofreference-zilch-en)|[joint](joint.md)| |
|[SetWorldFrame](revolutejoint.md#setworldframe-void)|[LocalBasisA](revolutejoint.md#localbasisa-zilch-engine)| | |
|[SetWorldPoints](revolutejoint.md#setworldpoints-void)|[LocalBasisB](revolutejoint.md#localbasisb-zilch-engine)| | |
| |[LocalPointA](revolutejoint.md#localpointa-zilch-engine)| | |
| |[LocalPointB](revolutejoint.md#localpointb-zilch-engine)| | |
| |[WorldBasis](revolutejoint.md#worldbasis-zilch-engine-d)| | |
| |[WorldPointA](revolutejoint.md#worldpointa-zilch-engine)| | |
| |[WorldPointB](revolutejoint.md#worldpointb-zilch-engine)| | |


 #  Properties


---  
 #  FrameOfReference : [JointFrameOfReference](../enum_reference.md#jointframeofreference)

> Should the default basis of the constraint be object A or B? This determines which object's world axis is used when constructing the basis for the constraint. In the case of a dynamic and static object, the static object is generally the better choice. As a general rule of thumb, it should be the heavier/most important object.
> ```TS:Nada
> var FrameOfReference : JointFrameOfReference


---  
 #  LocalBasisA : [quaternion](../nada_base_types/quaternion.md)

> The local space reference frame of object A . This frame is transformed to world space and then aligned with object B s frame . 
> ```TS:Nada
> var LocalBasisA : Quaternion


---  
 #  LocalBasisB : [quaternion](../nada_base_types/quaternion.md)

> The local space reference frame of object B . This frame is transformed to world space and then aligned with object A s frame . 
> ```TS:Nada
> var LocalBasisB : Quaternion


---  
 #  LocalPointA : [real3](../nada_base_types/real3.md)

> The local point of the anchor on object A . 
> ```TS:Nada
> var LocalPointA : Real3


---  
 #  LocalPointB : [real3](../nada_base_types/real3.md)

> The local point of the anchor on object B . 
> ```TS:Nada
> var LocalPointB : Real3


---  
 #  WorldBasis : [quaternion](../nada_base_types/quaternion.md)

> The basis of the joint in world-space. This basis will come object specified by FrameOfReference. The basis is constructed such that the x-axis is the primary axis while the z-axis is the hinge axis.
> ```TS:Nada
> var WorldBasis : Quaternion


---  
 #  WorldPointA : [real3](../nada_base_types/real3.md)

> The position of the anchor on object A given a position in world space 
> ```TS:Nada
> var WorldPointA : Real3


---  
 #  WorldPointB : [real3](../nada_base_types/real3.md)

> The position of the anchor on object B given a position in world space 
> ```TS:Nada
> var WorldPointB : Real3


---  
 #  Methods


---  
 #  RevoluteJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function RevoluteJoint()
> ``` 


---  
 #  SetWorldFrame : Void

> Legacy. Used to set the entire frame in world space for this joint. The x and y axes are used as a basis for limiting the joint. The x axis is at angle 0 and the y axis is at angle 90. The z axis is the axis of rotational freedom.
> |Name|Type|Description|
> |---|---|---|
> |rot|[quaternion](../nada_base_types/quaternion.md)| |
> ```TS:Nada
> function SetWorldFrame(rot : Quaternion)
> ``` 


---  
 #  SetWorldPoints : Void

> Sets the position of the anchor on object A and B given a position in world space 
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function SetWorldPoints(point : Real3)
> ``` 


---  
 

 
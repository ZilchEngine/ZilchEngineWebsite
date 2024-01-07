 `Component` `Physics`



(NOTE) Legacy. A linear axis joint is used to keep an object locked on a plane that is defined by a normal. This was made to help make a dynamic character controller. Instead of locking translation along a plane, the constraint can be turned off with a motor attached to it which will drive movement in the direction of the plane normal. This can then be thought of as a "move in direction" constraint.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/linearaxisjoint.md#linearaxisjoint-void)|[ WorldAxis](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/linearaxisjoint.md#worldaxis-zilch-engine-do)|[joint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/joint.md)| |


 #  Properties


---  
 #  WorldAxis : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The axis in world space that is constrained.
> ``` lang=cpp, name=Nada
> var WorldAxis : Real3


---  
 #  Methods


---  
 #  LinearAxisJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function LinearAxisJoint()
> ``` 


---  
 

 
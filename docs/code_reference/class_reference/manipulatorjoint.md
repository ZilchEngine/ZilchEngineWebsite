 `Component` `Physics`



(NOTE) Legacy. A position joint that is designed to manipulate one object. The only difference between this and the position joint is that the manipulator always draws itself, draws differently, and configures the max impulse differently.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/manipulatorjoint.md#manipulatorjoint-void)|[ LocalPoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/manipulatorjoint.md#localpoint-zilch-engine-d)|[joint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/joint.md)| |
| |[ TargetPoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/manipulatorjoint.md#targetpoint-zilch-engine)| | |
| |[ WorldPoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/manipulatorjoint.md#worldpoint-zilch-engine-d)| | |


 #  Properties


---  
 #  LocalPoint : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The local space point on the object that the joint is connected to.
> ``` lang=cpp, name=Nada
> var LocalPoint : Real3


---  
 #  TargetPoint : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The point in world space that the object's point is being moved towards.
> ``` lang=cpp, name=Nada
> var TargetPoint : Real3


---  
 #  WorldPoint : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The world space point on the object that the joint is connected to.
> ``` lang=cpp, name=Nada
> var WorldPoint : Real3


---  
 #  Methods


---  
 #  ManipulatorJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ManipulatorJoint()
> ``` 


---  
 

 
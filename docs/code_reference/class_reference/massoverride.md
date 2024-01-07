 `Component` `Physics`



(NOTE) Takes a snap shot of the current mass and inertia and overrides the object's mass so it can be resized while keeping it's old mass.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/massoverride.md#massoverride-void)|[ Active](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/massoverride.md#active-zilch-engine-docum)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)| |
|[ RecomputeMass](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/massoverride.md#recomputemass-void)|[ AutoComputeCenterOfMass](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/massoverride.md#autocomputecenterofmass)| | |
| |[ AutoComputeInertia](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/massoverride.md#autocomputeinertia-zero)| | |
| |[ InverseMass](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/massoverride.md#inversemass-zilch-engine)| | |
| |[ LocalCenterOfMass](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/massoverride.md#localcenterofmass-zilch-e)| | |
| |[ LocalInverseInertiaTensor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/massoverride.md#localinverseinertiatenso)| | |
| |[ Mass](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/massoverride.md#mass-zilch-engine-documen)| | |


 #  Properties


---  
 #  Active : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Determines whether the RigidBody on this Cog will use the cached or actual mass and inertia.
> ``` lang=cpp, name=Nada
> var Active : Boolean


---  
 #  AutoComputeCenterOfMass : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Should the center of mass be auto computed or overwritten (via script).
> ``` lang=cpp, name=Nada
> var AutoComputeCenterOfMass : Boolean


---  
 #  AutoComputeInertia : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Should the inertia tensor be auto computed or overwritten (via script).
> ``` lang=cpp, name=Nada
> var AutoComputeInertia : Boolean


---  
 #  InverseMass : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The cached inverse mass of this object.
> ``` lang=cpp, name=Nada
> var InverseMass : Real


---  
 #  LocalCenterOfMass : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The center of mass in local space to override with. When set, the center of mass will be locked to this value until AutoComputeCenterOfMass is set to true.
> ``` lang=cpp, name=Nada
> var LocalCenterOfMass : Real3


---  
 #  LocalInverseInertiaTensor : [real3x3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3x3.md)

> The inverse inertia tensor this object is saved with.
> ``` lang=cpp, name=Nada
> var LocalInverseInertiaTensor : Real3x3


---  
 #  Mass : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Overrides the mass of this body. Inertia is updated as a ratio of the new mass to the old mass.
> ``` lang=cpp, name=Nada
> var Mass : Real


---  
 #  Methods


---  
 #  MassOverride : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function MassOverride()
> ``` 


---  
 #  RecomputeMass : Void

> Takes a new snapshot of the current mass and inertia.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function RecomputeMass()
> ``` 


---  
 

 
 `Component` `Physics`



(NOTE) Takes a snap shot of the current mass and inertia and overrides the object's mass so it can be resized while keeping it's old mass.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](massoverride.md#massoverride-void)|[Active](massoverride.md#active-zilch-engine-docum)|[component](component.md)| |
|[RecomputeMass](massoverride.md#recomputemass-void)|[AutoComputeCenterOfMass](massoverride.md#autocomputecenterofmass)| | |
| |[AutoComputeInertia](massoverride.md#autocomputeinertia-zero)| | |
| |[InverseMass](massoverride.md#inversemass-zilch-engine)| | |
| |[LocalCenterOfMass](massoverride.md#localcenterofmass-zilch-e)| | |
| |[LocalInverseInertiaTensor](massoverride.md#localinverseinertiatenso)| | |
| |[Mass](massoverride.md#mass-zilch-engine-documen)| | |


 #  Properties


---  
 #  Active : [boolean](../nada_base_types/boolean.md)

> Determines whether the RigidBody on this Cog will use the cached or actual mass and inertia.
> ```TS:Nada
> var Active : Boolean


---  
 #  AutoComputeCenterOfMass : [boolean](../nada_base_types/boolean.md)

> Should the center of mass be auto computed or overwritten (via script).
> ```TS:Nada
> var AutoComputeCenterOfMass : Boolean


---  
 #  AutoComputeInertia : [boolean](../nada_base_types/boolean.md)

> Should the inertia tensor be auto computed or overwritten (via script).
> ```TS:Nada
> var AutoComputeInertia : Boolean


---  
 #  InverseMass : [real](../nada_base_types/real.md)

> The cached inverse mass of this object.
> ```TS:Nada
> var InverseMass : Real


---  
 #  LocalCenterOfMass : [real3](../nada_base_types/real3.md)

> The center of mass in local space to override with. When set, the center of mass will be locked to this value until AutoComputeCenterOfMass is set to true.
> ```TS:Nada
> var LocalCenterOfMass : Real3


---  
 #  LocalInverseInertiaTensor : [real3x3](../nada_base_types/real3x3.md)

> The inverse inertia tensor this object is saved with.
> ```TS:Nada
> var LocalInverseInertiaTensor : Real3x3


---  
 #  Mass : [real](../nada_base_types/real.md)

> Overrides the mass of this body. Inertia is updated as a ratio of the new mass to the old mass.
> ```TS:Nada
> var Mass : Real


---  
 #  Methods


---  
 #  MassOverride : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function MassOverride()
> ``` 


---  
 #  RecomputeMass : Void

> Takes a new snapshot of the current mass and inertia.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function RecomputeMass()
> ``` 


---  
 

 
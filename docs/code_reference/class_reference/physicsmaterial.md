 `Resource` `Physics`



(NOTE) Describes material properties of a collider mainly used during collision resolution.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[CreateRuntime](physicsmaterial.md#createruntime-zilch-engin)|[Density](physicsmaterial.md#density-zilch-engine-docu)|[dataresource](dataresource.md)| |
|[Constructor](physicsmaterial.md#physicsmaterial-void)|[Friction](physicsmaterial.md#friction-zilch-engine-doc)| | |
|[RuntimeClone](physicsmaterial.md#runtimeclone-zilch-engine)|[FrictionImportance](physicsmaterial.md#frictionimportance-zero)| | |
|[UpdateAndNotifyIfModified](physicsmaterial.md#updateandnotifyifmodifie)|[HighPriority](physicsmaterial.md#highpriority-zilch-engine)| | |
| |[Restitution](physicsmaterial.md#restitution-zilch-engine)| | |
| |[RestitutionImportance](physicsmaterial.md#restitutionimportance-ze)| | |


 #  Properties


---  
 #  Density : [real](../nada_base_types/real.md)

> Density is used to determine the mass of an object. Mass is computed as density * volume. Density can be set to exactly 0 to produce a massless object, however this should only be done with children objects to add collision without affecting mass.
> ```TS:Nada
> var Density : Real


---  
 #  Friction : [real](../nada_base_types/real.md)

> How slippery or rough the object is. When friction is 0 the object will be slippery. As friction increases, sliding objects will stop quicker. The friction of two object's are combined with the formula sqrt(a * b).
> ```TS:Nada
> var Friction : Real


---  
 #  FrictionImportance : [real](../nada_base_types/real.md)

> Determines which object's friction should be used. If object A's friction importance value is larger than object B's then object A's friction will be used. If both importance values are the same then the default combination logic will be used (see the description of Friction for details).
> ```TS:Nada
> var FrictionImportance : Real


---  
 #  HighPriority : [boolean](../nada_base_types/boolean.md)

> Deprecated. Use RestitutionImportance instead.
> ```TS:Nada
> var HighPriority : Boolean


---  
 #  Restitution : [real](../nada_base_types/real.md)

> How much an object will bounce during a collision. Values should be in the range [0,1] where 0 is an inelastic collision and 1 is a fully elastic collision. Restitution is computed as the max of the two objects. Note: due to solving constraints with baumgarte, energy will not be perfectly conserved with a restitution 1.
> ```TS:Nada
> var Restitution : Real


---  
 #  RestitutionImportance : [real](../nada_base_types/real.md)

> Determines which object's restitution should be used. If object A's restitution importance value is larger than object B's then object A's restitution will be used. If both importance values are the same then the default combination logic will be used (see the description of Restitution for details).
> ```TS:Nada
> var RestitutionImportance : Real


---  
 #  Methods


---  
 #  CreateRuntime : [physicsmaterial](physicsmaterial.md)

 `static`

> Creates a PhysicsMaterial for run-time modifications.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function CreateRuntime() : PhysicsMaterial
> ``` 


---  
 #  PhysicsMaterial : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function PhysicsMaterial()
> ``` 


---  
 #  RuntimeClone : [physicsmaterial](physicsmaterial.md)

> Creates a clone of this material for run-time modifications.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function RuntimeClone() : PhysicsMaterial
> ``` 


---  
 #  UpdateAndNotifyIfModified : Void

> After modifying this resource, notify anyone using it to update now instead of at the next physics update.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function UpdateAndNotifyIfModified()
> ``` 


---  
 

 
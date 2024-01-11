 `Physics`

(NOTE) Used to filter objects during cast operations.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ IgnoreChildren](basecastfilter.md#ignorechildren-zilch-engi)| |[castfilter](castfilter.md)|
| |[ IgnoreDynamic](basecastfilter.md#ignoredynamic-zilch-engin)| | |
| |[ IgnoreGhost](basecastfilter.md#ignoreghost-zilch-engine)| | |
| |[ IgnoreKinematic](basecastfilter.md#ignorekinematic-zilch-eng)| | |
| |[ IgnoreStatic](basecastfilter.md#ignorestatic-zilch-engine)| | |


 #  Properties


---  
 #  IgnoreChildren : [boolean](../nada_base_types/boolean.md)

> This flag is currently only used for SweepCollider tests on PhysicsSpace. This is used to ignore all objects that are a child of the Collider that is being swept.
> ```TS:Nada
> var IgnoreChildren : Boolean


---  
 #  IgnoreDynamic : [boolean](../nada_base_types/boolean.md)

> Should Colliders with RigidBodies marked Dynamic be ignored during casts?
> ```TS:Nada
> var IgnoreDynamic : Boolean


---  
 #  IgnoreGhost : [boolean](../nada_base_types/boolean.md)

> Should Colliders marked Ghost be ignored during casts?
> ```TS:Nada
> var IgnoreGhost : Boolean


---  
 #  IgnoreKinematic : [boolean](../nada_base_types/boolean.md)

> Should Colliders with RigidBodies marked Kinematic be ignored during casts?
> ```TS:Nada
> var IgnoreKinematic : Boolean


---  
 #  IgnoreStatic : [boolean](../nada_base_types/boolean.md)

> Should Colliders with RigidBodies marked Static be ignored during casts? Note: Collider's with no RigidBody are treated as static.
> ```TS:Nada
> var IgnoreStatic : Boolean


---  
 #  Methods


---  
 

 
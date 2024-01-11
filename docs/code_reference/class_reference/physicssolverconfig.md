 `Resource` `Physics`



(NOTE) Defines various configuration values used by physics to solve constraints. This resource defines a tiered set of properties that can be overridden global or per constraint type.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](physicssolverconfig.md#physicssolverconfig-void)|[ PositionCorrectionType](physicssolverconfig.md#positioncorrectiontype-z)|[dataresource](dataresource.md)| |
| |[ PositionIterationCount](physicssolverconfig.md#positioniterationcount-z)| | |
| |[ SolverIterationCount](physicssolverconfig.md#solveriterationcount-zer)| | |
| |[ VelocityRestitutionThreshold](physicssolverconfig.md#velocityrestitutionthres)| | |


 #  Properties


---  
 #  PositionCorrectionType : [PhysicsSolverPositionCorrection](../enum_reference.md#physicssolverpositioncorrection)

> What method should be used to fix errors in joints. Baumgarte fixes errors by adding extra velocity but results in a more spongy behavior. Post Stabilization fixes errors by directly modifying position but can behave worse in unsolvable configurations.
> ``` lang=cpp, name=Nada
> var PositionCorrectionType : PhysicsSolverPositionCorrection


---  
 #  PositionIterationCount : [integer](../nada_base_types/integer.md)

> The number of iterations used for position correction (if position correction is used).
> ``` lang=cpp, name=Nada
> var PositionIterationCount : Integer


---  
 #  SolverIterationCount : [integer](../nada_base_types/integer.md)

> The number of iterations used in the constraint solver. Affects how stiff joints will be.
> ``` lang=cpp, name=Nada
> var SolverIterationCount : Integer


---  
 #  VelocityRestitutionThreshold : [real](../nada_base_types/real.md)

> To prevent numerical issues, restitution is only applied if the relative velocity between the two objects is above this value.
> ``` lang=cpp, name=Nada
> var VelocityRestitutionThreshold : Real


---  
 #  Methods


---  
 #  PhysicsSolverConfig : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function PhysicsSolverConfig()
> ``` 


---  
 

 
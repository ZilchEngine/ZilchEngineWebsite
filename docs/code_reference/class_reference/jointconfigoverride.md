 `Component` `Physics`



(NOTE) Overrides a joint's configuration values of slop, linear/angular Baumgarte, and linear/angular error correction. Slop is the amount of error allowed before position correction takes effect. Baumgarte is used to correct error with a penalty impulse. Baumgarte is split into linear and angular portions because of stability. Error correction is only used when the joint is solved with post stabilization.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](jointconfigoverride.md#jointconfigoverride-void)|[AngularBaumgarte](jointconfigoverride.md#angularbaumgarte-zilch-en)|[component](component.md)| |
| |[AngularErrorCorrection](jointconfigoverride.md#angularerrorcorrection-z)| | |
| |[LinearBaumgarte](jointconfigoverride.md#linearbaumgarte-zilch-eng)| | |
| |[LinearErrorCorrection](jointconfigoverride.md#linearerrorcorrection-ze)| | |
| |[PositionCorrectionType](jointconfigoverride.md#positioncorrectiontype-z)| | |
| |[Slop](jointconfigoverride.md#slop-zilch-engine-documen)| | |


 #  Properties


---  
 #  AngularBaumgarte : [real](../nada_base_types/real.md)

> The exponential constant for correcting angular error with a penalty impulse.
> ```TS:Nada
> var AngularBaumgarte : Real


---  
 #  AngularErrorCorrection : [real](../nada_base_types/real.md)

> The max amount of error that can be corrected by the angular portion of any constraint in one frame (only for PostStabilization).
> ```TS:Nada
> var AngularErrorCorrection : Real


---  
 #  LinearBaumgarte : [real](../nada_base_types/real.md)

> The exponential constant for correcting linear error with a penalty impulse.
> ```TS:Nada
> var LinearBaumgarte : Real


---  
 #  LinearErrorCorrection : [real](../nada_base_types/real.md)

> The max amount of error that can be corrected by the linear portion of any constraint in one frame (only for PostStabilization).
> ```TS:Nada
> var LinearErrorCorrection : Real


---  
 #  PositionCorrectionType : [ConstraintPositionCorrection](../enum_reference.md#constraintpositioncorrection)

> The kind of position correction that this joint should use.
> ```TS:Nada
> var PositionCorrectionType : ConstraintPositionCorrection


---  
 #  Slop : [real](../nada_base_types/real.md)

> The amount of error allowed before position correction takes effect.
> ```TS:Nada
> var Slop : Real


---  
 #  Methods


---  
 #  JointConfigOverride : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function JointConfigOverride()
> ``` 


---  
 

 
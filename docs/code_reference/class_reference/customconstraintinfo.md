 `Physics`

(NOTE) Information to represent a constraint to be solved. The main information that needs to be set here is the Jacobian and error. A constraint will enforce that the relative velocities along the Jacobian are equal to zero (ignoring error correction or motors).

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ComputeMotor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customconstraintinfo.md#computemotor-void)|[ Active](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customconstraintinfo.md#active-zilch-engine-docum)|[referencecountedeventobject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/referencecountedeventobject.md)| |
|[ ComputeSpring](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customconstraintinfo.md#computespring-void)|[ Angular0](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customconstraintinfo.md#angular0-zilch-engine-doc)| | |
|[ DetachFromOwner](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customconstraintinfo.md#detachfromowner-void)|[ Angular1](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customconstraintinfo.md#angular1-zilch-engine-doc)| | |
|[ IsOwned](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customconstraintinfo.md#isowned-zilch-engine-docu)|[ Baumgarte](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customconstraintinfo.md#baumgarte-zilch-engine-do)| | |
|[ SetErrorAndBias](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customconstraintinfo.md#seterrorandbias-void)|[ Bias](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customconstraintinfo.md#bias-zilch-engine-documen)| | |
|[ SetJacobian](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customconstraintinfo.md#setjacobian-void)|[ EffectiveMass](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customconstraintinfo.md#effectivemass-zilch-engin)| | |
| |[ Error](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customconstraintinfo.md#error-zilch-engine-docume)| | |
| |[ Gamma](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customconstraintinfo.md#gamma-zilch-engine-docume)| | |
| |[ Impulse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customconstraintinfo.md#impulse-zilch-engine-docu)| | |
| |[ Linear0](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customconstraintinfo.md#linear0-zilch-engine-docu)| | |
| |[ Linear1](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customconstraintinfo.md#linear1-zilch-engine-docu)| | |
| |[ MaxImpulse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customconstraintinfo.md#maximpulse-zilch-engine-d)| | |
| |[ MinImpulse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customconstraintinfo.md#minimpulse-zilch-engine-d)| | |
| |[ Owner](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customconstraintinfo.md#owner-zilch-engine-docume)| | |
| |[ SolvePosition](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customconstraintinfo.md#solveposition-zilch-engin)| | |


 #  Properties


---  
 #  Active : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Is this constraint currently active?
> ``` lang=cpp, name=Nada
> var Active : Boolean


---  
 #  Angular0 : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Angular portion of objectA's Jacobian.
> ``` lang=cpp, name=Nada
> var Angular0 : Real3


---  
 #  Angular1 : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Angular portion of objectB's Jacobian.
> ``` lang=cpp, name=Nada
> var Angular1 : Real3


---  
 #  Baumgarte : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The baumgarte term used to correct error. This should typically be set in initialization (per constraint) and then left alone. Default value is 5.
> ``` lang=cpp, name=Nada
> var Baumgarte : Real


---  
 #  Bias : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The bias is used to apply energy into the system. Typically, bias is combined with Error and Baumgarte to fix error. Bias is also used for motors and springs to drive the constraint.
> ``` lang=cpp, name=Nada
> var Bias : Real


---  
 #  EffectiveMass : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The effective mass of the constraint. This is typically set by calling SetJacobian.
> ``` lang=cpp, name=Nada
> var EffectiveMass : Real


---  
 #  Error : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The error of the constraint. This should typically be set via the SetError function.
> ``` lang=cpp, name=Nada
> var Error : Real


---  
 #  Gamma : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Gamma is used to soften constraints. This should typically never be manually set. Instead, it is set when configuring the constraint to act like a spring.
> ``` lang=cpp, name=Nada
> var Gamma : Real


---  
 #  Impulse : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The total accumulated impulse of this constraint. If you want to not use warm-starting then clear this value every frame.
> ``` lang=cpp, name=Nada
> var Impulse : Real


---  
 #  Linear0 : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Linear portion of objectA's Jacobian.
> ``` lang=cpp, name=Nada
> var Linear0 : Real3


---  
 #  Linear1 : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Linear portion of objectB's Jacobian.
> ``` lang=cpp, name=Nada
> var Linear1 : Real3


---  
 #  MaxImpulse : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The max impulse magnitude allowed for the constraint.
> ``` lang=cpp, name=Nada
> var MaxImpulse : Real


---  
 #  MinImpulse : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The min impulse magnitude allowed for the constraint.
> ``` lang=cpp, name=Nada
> var MinImpulse : Real


---  
 #  Owner : [customjoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customjoint.md)

 `read-only`

> What joint currently owns this constraint.
> ``` lang=cpp, name=Nada
> var Owner : CustomJoint


---  
 #  SolvePosition : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Should this constraint solve position directly or use baumgarte correction? Toggling SolvePosition should be done before setting any other values (ideally in initialization). Setting a constraint to be a motor or a spring will turn off position correction as an error bias must be used to solve those scenarios.
> ``` lang=cpp, name=Nada
> var SolvePosition : Boolean


---  
 #  Methods


---  
 #  ComputeMotor : Void

> Sets this constraint as a motor (i.e. a constraint that drives movement along the Jacobian direction at a certain speed). The motor has a min and max impulse value that can be solved (typically -value, +value). If you set this as a motor, you should do so last. Motors should typically be their own constraint unlike springs.
> |Name|Type|Description|
> |---|---|---|
> |targetSpeed|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |minImpulse|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |maxImpulse|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function ComputeMotor(targetSpeed : Real, minImpulse : Real, maxImpulse : Real)
> ``` 


---  
 #  ComputeSpring : Void

> Given the currently set mass and error, fix the constraint to be soft (i.e. solve the constraint like a spring). The spring fixes the constraint using the given frequency (oscillations per second) and damping ratio (0 is no damping, 1 is critical damping).
> |Name|Type|Description|
> |---|---|---|
> |frequencyHz|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |dampRatio|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function ComputeSpring(frequencyHz : Real, dampRatio : Real)
> ``` 


---  
 #  DetachFromOwner : Void

> Remove this constraint from whatever joint owns it. This is equivalent to "this.Owner.RemoveConstraint(this)".
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function DetachFromOwner()
> ``` 


---  
 #  IsOwned : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Is this constraint currently owned by a joint? (Equivalent to "this.Owner != null").
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function IsOwned() : Boolean
> ``` 


---  
 #  SetErrorAndBias : Void

> Set the position error of the constraint. This also sets the bias of the constraint (used to actually correct the error). If you want to set this constraint as a motor you should not call this function (or call it first). If you want to set this as a spring then make sure you call this first.
> |Name|Type|Description|
> |---|---|---|
> |error|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function SetErrorAndBias(error : Real)
> ``` 


---  
 #  SetJacobian : Void

> Set the Jacobian of this constraint (and the effective mass).
> |Name|Type|Description|
> |---|---|---|
> |linear0|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |angular0|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |linear1|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |angular1|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function SetJacobian(linear0 : Real3, angular0 : Real3, linear1 : Real3, angular1 : Real3)
> ``` 


---  
 

 
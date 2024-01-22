 `Component` `Physics`



(NOTE) Defines motor properties for a joint. Used to add energy to a joint. A motor defines a desired speed to move at as well as a max impulse that can be applied to reach that speed in a timestep. See each joint for a description of how it reacts to a motor.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](jointmotor.md#jointmotor-void)|[Active](jointmotor.md#active-zilch-engine-docum)|[component](component.md)| |
| |[AtomIds](jointmotor.md#atomids-zilch-engine-docu)| | |
| |[MaxImpulse](jointmotor.md#maximpulse-zilch-engine-d)| | |
| |[Reverse](jointmotor.md#reverse-zilch-engine-docu)| | |
| |[Speed](jointmotor.md#speed-zilch-engine-docume)| | |


 #  Properties


---  
 #  Active : [boolean](../nada_base_types/boolean.md)

> Determines if this motor is currently active.
> ```TS:Nada
> var Active : Boolean


---  
 #  AtomIds : [integer](../nada_base_types/integer.md)

> Signifies what atoms on the joint this affects. For internal use.
> ```TS:Nada
> var AtomIds : Integer


---  
 #  MaxImpulse : [real](../nada_base_types/real.md)

> The maximum impulse that the motor can apply each frame to reach the target speed.
> ```TS:Nada
> var MaxImpulse : Real


---  
 #  Reverse : [boolean](../nada_base_types/boolean.md)

> Determines if this motor should move in reverse. This is a convenient way to reverse a motor without having to negate the speed.
> ```TS:Nada
> var Reverse : Boolean


---  
 #  Speed : [real](../nada_base_types/real.md)

> The desired speed for this motor.
> ```TS:Nada
> var Speed : Real


---  
 #  Methods


---  
 #  JointMotor : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function JointMotor()
> ``` 


---  
 

 
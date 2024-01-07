 `Component` `Physics`



(NOTE) Defines motor properties for a joint. Used to add energy to a joint. A motor defines a desired speed to move at as well as a max impulse that can be applied to reach that speed in a timestep. See each joint for a description of how it reacts to a motor.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointmotor.md#jointmotor-void)|[ Active](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointmotor.md#active-zilch-engine-docum)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)| |
| |[ AtomIds](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointmotor.md#atomids-zilch-engine-docu)| | |
| |[ MaxImpulse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointmotor.md#maximpulse-zilch-engine-d)| | |
| |[ Reverse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointmotor.md#reverse-zilch-engine-docu)| | |
| |[ Speed](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointmotor.md#speed-zilch-engine-docume)| | |


 #  Properties


---  
 #  Active : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Determines if this motor is currently active.
> ``` lang=cpp, name=Nada
> var Active : Boolean


---  
 #  AtomIds : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> Signifies what atoms on the joint this affects. For internal use.
> ``` lang=cpp, name=Nada
> var AtomIds : Integer


---  
 #  MaxImpulse : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The maximum impulse that the motor can apply each frame to reach the target speed.
> ``` lang=cpp, name=Nada
> var MaxImpulse : Real


---  
 #  Reverse : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Determines if this motor should move in reverse. This is a convenient way to reverse a motor without having to negate the speed.
> ``` lang=cpp, name=Nada
> var Reverse : Boolean


---  
 #  Speed : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The desired speed for this motor.
> ``` lang=cpp, name=Nada
> var Speed : Real


---  
 #  Methods


---  
 #  JointMotor : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function JointMotor()
> ``` 


---  
 

 
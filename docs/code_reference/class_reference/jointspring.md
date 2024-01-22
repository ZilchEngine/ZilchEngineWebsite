 `Component` `Physics`



(NOTE) Defines spring properties for a joint. Used to make a joint soft and therefore behave spring-like. A joint spring has a frequency in hertz at which to oscillate as well as a damping ratio. The ratio should vary from 0 to 1 where 0 is no damping and 1 is critical damping. See each joint for a description of how it reacts to a spring.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](jointspring.md#jointspring-void)|[Active](jointspring.md#active-zilch-engine-docum)|[component](component.md)| |
| |[AtomIds](jointspring.md#atomids-zilch-engine-docu)| | |
| |[DampingRatio](jointspring.md#dampingratio-zilch-engine)| | |
| |[FrequencyHz](jointspring.md#frequencyhz-zilch-engine)| | |


 #  Properties


---  
 #  Active : [boolean](../nada_base_types/boolean.md)

> Determines if this spring is active.
> ```TS:Nada
> var Active : Boolean


---  
 #  AtomIds : [integer](../nada_base_types/integer.md)

> Signifies what atoms on the joint this affects. For internal use.
> ```TS:Nada
> var AtomIds : Integer


---  
 #  DampingRatio : [real](../nada_base_types/real.md)

> The damping ratio of this spring. The value should range from 0 to 1 where 0 is no damping and 1 is critical damping.
> ```TS:Nada
> var DampingRatio : Real


---  
 #  FrequencyHz : [real](../nada_base_types/real.md)

> The oscillation frequency of the spring in Hertz (cycles per second).
> ```TS:Nada
> var FrequencyHz : Real


---  
 #  Methods


---  
 #  JointSpring : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function JointSpring()
> ``` 


---  
 

 
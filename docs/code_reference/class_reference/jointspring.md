 `Component` `Physics`



(NOTE) Defines spring properties for a joint. Used to make a joint soft and therefore behave spring-like. A joint spring has a frequency in hertz at which to oscillate as well as a damping ratio. The ratio should vary from 0 to 1 where 0 is no damping and 1 is critical damping. See each joint for a description of how it reacts to a spring.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointspring.md#jointspring-void)|[ Active](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointspring.md#active-zilch-engine-docum)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)| |
| |[ AtomIds](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointspring.md#atomids-zilch-engine-docu)| | |
| |[ DampingRatio](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointspring.md#dampingratio-zilch-engine)| | |
| |[ FrequencyHz](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointspring.md#frequencyhz-zilch-engine)| | |


 #  Properties


---  
 #  Active : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Determines if this spring is active.
> ``` lang=cpp, name=Nada
> var Active : Boolean


---  
 #  AtomIds : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> Signifies what atoms on the joint this affects. For internal use.
> ``` lang=cpp, name=Nada
> var AtomIds : Integer


---  
 #  DampingRatio : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The damping ratio of this spring. The value should range from 0 to 1 where 0 is no damping and 1 is critical damping.
> ``` lang=cpp, name=Nada
> var DampingRatio : Real


---  
 #  FrequencyHz : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The oscillation frequency of the spring in Hertz (cycles per second).
> ``` lang=cpp, name=Nada
> var FrequencyHz : Real


---  
 #  Methods


---  
 #  JointSpring : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function JointSpring()
> ``` 


---  
 

 
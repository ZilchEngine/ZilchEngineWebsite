 `Component` `Physics`



(NOTE) Defines limit properties for a joint. Used to add a min/max bounds to a joint. When the joint is in between the min/max bounds, the "limited" portion will be ignored (The stick will not solve when it is in between the bounds, making it a rope). See each joint for a description of how it reacts to a limit.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointlimit.md#jointlimit-void)|[ Active](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointlimit.md#active-zilch-engine-docum)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)| |
| |[ AtomIds](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointlimit.md#atomids-zilch-engine-docu)| | |
| |[ LowerLimit](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointlimit.md#lowerlimit-zilch-engine-d)| | |
| |[ UpperLimit](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointlimit.md#upperlimit-zilch-engine-d)| | |


 #  Properties


---  
 #  Active : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Determines if this limit is currently active.
> ``` lang=cpp, name=Nada
> var Active : Boolean


---  
 #  AtomIds : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> Signifies what atoms on the joint this affects. For internal use.
> ``` lang=cpp, name=Nada
> var AtomIds : Integer


---  
 #  LowerLimit : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The lower bound for this limit.
> ``` lang=cpp, name=Nada
> var LowerLimit : Real


---  
 #  UpperLimit : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The upper bound for this limit.
> ``` lang=cpp, name=Nada
> var UpperLimit : Real


---  
 #  Methods


---  
 #  JointLimit : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function JointLimit()
> ``` 


---  
 

 
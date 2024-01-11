 `Component` `Physics`



(NOTE) Defines limit properties for a joint. Used to add a min/max bounds to a joint. When the joint is in between the min/max bounds, the "limited" portion will be ignored (The stick will not solve when it is in between the bounds, making it a rope). See each joint for a description of how it reacts to a limit.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](jointlimit.md#jointlimit-void)|[ Active](jointlimit.md#active-zilch-engine-docum)|[component](component.md)| |
| |[ AtomIds](jointlimit.md#atomids-zilch-engine-docu)| | |
| |[ LowerLimit](jointlimit.md#lowerlimit-zilch-engine-d)| | |
| |[ UpperLimit](jointlimit.md#upperlimit-zilch-engine-d)| | |


 #  Properties


---  
 #  Active : [boolean](../nada_base_types/boolean.md)

> Determines if this limit is currently active.
> ```TS:Nada
> var Active : Boolean


---  
 #  AtomIds : [integer](../nada_base_types/integer.md)

> Signifies what atoms on the joint this affects. For internal use.
> ```TS:Nada
> var AtomIds : Integer


---  
 #  LowerLimit : [real](../nada_base_types/real.md)

> The lower bound for this limit.
> ```TS:Nada
> var LowerLimit : Real


---  
 #  UpperLimit : [real](../nada_base_types/real.md)

> The upper bound for this limit.
> ```TS:Nada
> var UpperLimit : Real


---  
 #  Methods


---  
 #  JointLimit : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function JointLimit()
> ``` 


---  
 

 
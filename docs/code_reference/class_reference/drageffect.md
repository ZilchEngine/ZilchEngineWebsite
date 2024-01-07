 `Component` `Physics`



(NOTE) Applies drag or damping forces to slow down an object's linear and angular velocity. Drag is computed as a simple linear approximation of the drag force. Damping is a linear approximation of a drag acceleration. This means that damping affects all objects the same (mass independent).

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/drageffect.md#drageffect-void)|[ AngularDamping](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/drageffect.md#angulardamping-zilch-engi)|[physicseffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicseffect.md)| |
| |[ AngularDrag](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/drageffect.md#angulardrag-zilch-engine)| | |
| |[ LinearDamping](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/drageffect.md#lineardamping-zilch-engin)| | |
| |[ LinearDrag](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/drageffect.md#lineardrag-zilch-engine-d)| | |


 #  Properties


---  
 #  AngularDamping : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Angular damping coefficient for applying an angular drag acceleration (accel = -kw). Note: this affects objects the same regardless of mass.
> ``` lang=cpp, name=Nada
> var AngularDamping : Real


---  
 #  AngularDrag : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The angular drag coefficient for applying an angular drag force (T = -kw).
> ``` lang=cpp, name=Nada
> var AngularDrag : Real


---  
 #  LinearDamping : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Linear damping coefficient for applying a linear drag acceleration (accel = -bv). Note: this affects objects the same regardless of mass.
> ``` lang=cpp, name=Nada
> var LinearDamping : Real


---  
 #  LinearDrag : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The linear drag coefficient for applying a linear drag force (F = -bv).
> ``` lang=cpp, name=Nada
> var LinearDrag : Real


---  
 #  Methods


---  
 #  DragEffect : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function DragEffect()
> ``` 


---  
 

 
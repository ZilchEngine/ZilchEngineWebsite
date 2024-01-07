 `Component` `Physics`



(NOTE) Controls an object's movement using joints. This allows creating a physics based character controller that reacts to physics (joints, forces, collisions, etc...). The motor controls relative velocity with respect to a target object frame.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/dynamicmotor.md#dynamicmotor-void)|[ Active](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/dynamicmotor.md#active-zilch-engine-docum)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)| |
|[ MoveInDirection](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/dynamicmotor.md#moveindirection-void)|[ MaxMoveImpulse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/dynamicmotor.md#maxmoveimpulse-zilch-engi)| | |
|[ SetReferenceFrameToObject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/dynamicmotor.md#setreferenceframetoobjec)| | | |
|[ SetReferenceFrameToWorld](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/dynamicmotor.md#setreferenceframetoworld)| | | |


 #  Properties


---  
 #  Active : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Should physics restrict the movement of this object?
> ``` lang=cpp, name=Nada
> var Active : Boolean


---  
 #  MaxMoveImpulse : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> What is the max impulse allowed for controlling movement.
> ``` lang=cpp, name=Nada
> var MaxMoveImpulse : Real


---  
 #  Methods


---  
 #  DynamicMotor : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function DynamicMotor()
> ``` 


---  
 #  MoveInDirection : Void

> Attempts to move the body in the given direction.
> |Name|Type|Description|
> |---|---|---|
> |direction|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |up|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function MoveInDirection(direction : Real3, up : Real3)
> ``` 


---  
 #  SetReferenceFrameToObject : Void

> Compute the relative velocity with respect to a target object. Used to control movement on moving platforms.
> |Name|Type|Description|
> |---|---|---|
> |object|[cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| |
> ``` lang=cpp, name=Nada
> function SetReferenceFrameToObject(object : Cog)
> ``` 


---  
 #  SetReferenceFrameToWorld : Void

> Compute relative velocity with respect to the world. Used to signify that an absolute world speed is desired.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function SetReferenceFrameToWorld()
> ``` 


---  
 

 
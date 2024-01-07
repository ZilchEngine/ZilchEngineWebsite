 `Component` `Physics`



(NOTE) A customizable joint that can be configured in script. The user can create constraints belonging to this joint and set the required values to solve them. Some basic constraint understanding is required. To compute constraints you should listen to Events.ComputeCustomJointInfo.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddConstraint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customjoint.md#addconstraint-void)|[ ConstraintCount](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customjoint.md#constraintcount-zilch-eng)|[joint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/joint.md)| |
|[ ClearConstraints](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customjoint.md#clearconstraints-void)| | | |
|[ CreateConstraint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customjoint.md#createconstraint-zilch-en)| | | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customjoint.md#customjoint-void)| | | |
|[ GetConstraint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customjoint.md#getconstraint-zilch-engin)| | | |
|[ RemoveConstraint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customjoint.md#removeconstraint-void)| | | |


 #  Properties


---  
 #  ConstraintCount : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Returns how many constraints this joint owns.
> ``` lang=cpp, name=Nada
> var ConstraintCount : Integer


---  
 #  Methods


---  
 #  AddConstraint : Void

> Add a constraint to this joint. This will assert if a joint already owns this constraint.
> |Name|Type|Description|
> |---|---|---|
> |constraint|[customconstraintinfo](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customconstraintinfo.md)| |
> ``` lang=cpp, name=Nada
> function AddConstraint(constraint : CustomConstraintInfo)
> ``` 


---  
 #  ClearConstraints : Void

> Clear all constraints from this joint (so none will solve).
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ClearConstraints()
> ``` 


---  
 #  CreateConstraint : [customconstraintinfo](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customconstraintinfo.md)

> Create a constraint that is attached to this joint.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function CreateConstraint() : CustomConstraintInfo
> ``` 


---  
 #  CustomJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function CustomJoint()
> ``` 


---  
 #  GetConstraint : [customconstraintinfo](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customconstraintinfo.md)

> Returns the constraint at the given index. Will assert if the index is outside the constraint count range.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function GetConstraint(index : Integer) : CustomConstraintInfo
> ``` 


---  
 #  RemoveConstraint : Void

> If the given constraint belongs to this joint then remove it from the constraints to solve.
> |Name|Type|Description|
> |---|---|---|
> |constraint|[customconstraintinfo](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customconstraintinfo.md)| |
> ``` lang=cpp, name=Nada
> function RemoveConstraint(constraint : CustomConstraintInfo)
> ``` 


---  
 

 
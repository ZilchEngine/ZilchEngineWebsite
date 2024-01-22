 `Component` `Physics`



(NOTE) A customizable joint that can be configured in script. The user can create constraints belonging to this joint and set the required values to solve them. Some basic constraint understanding is required. To compute constraints you should listen to Events.ComputeCustomJointInfo.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[AddConstraint](customjoint.md#addconstraint-void)|[ConstraintCount](customjoint.md#constraintcount-zilch-eng)|[joint](joint.md)| |
|[ClearConstraints](customjoint.md#clearconstraints-void)| | | |
|[CreateConstraint](customjoint.md#createconstraint-zilch-en)| | | |
|[Constructor](customjoint.md#customjoint-void)| | | |
|[GetConstraint](customjoint.md#getconstraint-zilch-engin)| | | |
|[RemoveConstraint](customjoint.md#removeconstraint-void)| | | |


 #  Properties


---  
 #  ConstraintCount : [integer](../nada_base_types/integer.md)

 `read-only`

> Returns how many constraints this joint owns.
> ```TS:Nada
> var ConstraintCount : Integer


---  
 #  Methods


---  
 #  AddConstraint : Void

> Add a constraint to this joint. This will assert if a joint already owns this constraint.
> |Name|Type|Description|
> |---|---|---|
> |constraint|[customconstraintinfo](customconstraintinfo.md)| |
> ```TS:Nada
> function AddConstraint(constraint : CustomConstraintInfo)
> ``` 


---  
 #  ClearConstraints : Void

> Clear all constraints from this joint (so none will solve).
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ClearConstraints()
> ``` 


---  
 #  CreateConstraint : [customconstraintinfo](customconstraintinfo.md)

> Create a constraint that is attached to this joint.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function CreateConstraint() : CustomConstraintInfo
> ``` 


---  
 #  CustomJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function CustomJoint()
> ``` 


---  
 #  GetConstraint : [customconstraintinfo](customconstraintinfo.md)

> Returns the constraint at the given index. Will assert if the index is outside the constraint count range.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function GetConstraint(index : Integer) : CustomConstraintInfo
> ``` 


---  
 #  RemoveConstraint : Void

> If the given constraint belongs to this joint then remove it from the constraints to solve.
> |Name|Type|Description|
> |---|---|---|
> |constraint|[customconstraintinfo](customconstraintinfo.md)| |
> ```TS:Nada
> function RemoveConstraint(constraint : CustomConstraintInfo)
> ``` 


---  
 

 
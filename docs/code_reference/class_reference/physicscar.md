 `Component` `Physics`



(NOTE) A controller for a high speed physics based car. The car is controlled with a steer, gas, and brake scalar. The car will raycast wheel positions to try to keep the wheels on the ground and then apply friction and normal forces to propel the car.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ NumberOfWheelsInContact](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicscar.md#numberofwheelsincontact)|[ Active](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicscar.md#active-zilch-engine-docum)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)| |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicscar.md#physicscar-void)|[ AntiLockBrakes](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicscar.md#antilockbrakes-zilch-engi)| | |
| |[ Brake](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicscar.md#brake-zilch-engine-docume)| | |
| |[ DebugDraw](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicscar.md#debugdraw-zilch-engine-do)| | |
| |[ Gas](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicscar.md#gas-zilch-engine-document)| | |
| |[ GripScalar](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicscar.md#gripscalar-zilch-engine-d)| | |
| |[ MaxSpeed](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicscar.md#maxspeed-zilch-engine-doc)| | |
| |[ MaxTorque](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicscar.md#maxtorque-zilch-engine-do)| | |
| |[ Steer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicscar.md#steer-zilch-engine-docume)| | |
| |[ TorqueGovernor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicscar.md#torquegovernor-zilch-engi)| | |
| |[ WheelCogs](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicscar.md#wheelcogs-zilch-engine-do)| | |
| |[ WheelFrictionFrontRollCoef](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicscar.md#wheelfrictionfrontrollco)| | |
| |[ WheelFrictionSideRollCoef](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicscar.md#wheelfrictionsiderollcoe)| | |


 #  Properties


---  
 #  Active : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Whether or not the car will run any logic at all. If this is false wheels will not work, they will not behave as springs, drive, or anything else.
> ``` lang=cpp, name=Nada
> var Active : Boolean


---  
 #  AntiLockBrakes : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Prevents the car from entering dynamic friction when applying brakes. If the brake would start to skid, the brake force is clamped to the max amount that will not slip.
> ``` lang=cpp, name=Nada
> var AntiLockBrakes : Boolean


---  
 #  Brake : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> How much the brake is being pressed [0,1] where 1 is full brake.
> ``` lang=cpp, name=Nada
> var Brake : Real


---  
 #  DebugDraw : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Whether or not the car should debug draw.
> ``` lang=cpp, name=Nada
> var DebugDraw : Boolean


---  
 #  Gas : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> How much the gas is being pressed [-1,1] where -1 is full reverse.
> ``` lang=cpp, name=Nada
> var Gas : Real


---  
 #  GripScalar : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Artificially increases the grip of the car (where 2 is twice the grip). The total grip scalar is computed as CarGripScalar * WheelGripScalar so the total car can be easily tweaked while allowing individual wheel tweaks.
> ``` lang=cpp, name=Nada
> var GripScalar : Real


---  
 #  MaxSpeed : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The desired maximum speed of the car. Similar to a speed governor.
> ``` lang=cpp, name=Nada
> var MaxSpeed : Real


---  
 #  MaxTorque : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The maximum torque the engine can apply to try to reach the max speed.
> ``` lang=cpp, name=Nada
> var MaxTorque : Real


---  
 #  Steer : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> How much the wheel is being steered. This is measured in radians about this object's y-axis.
> ``` lang=cpp, name=Nada
> var Steer : Real


---  
 #  TorqueGovernor : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Governs the max torque that the engine can apply. This is used to keep the wheels from spinning out (slipping) when too high of a torque is applied. If the tires would slip, the engine will apply the maximum torque for the tires to not slip.
> ``` lang=cpp, name=Nada
> var TorqueGovernor : Boolean


---  
 #  WheelCogs : [carwheelarray](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/carwheelarray.md)

 `read-only`

> Read-only array of wheels belonging to this car.
> ``` lang=cpp, name=Nada
> var WheelCogs : CarWheelArray


---  
 #  WheelFrictionFrontRollCoef : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Coefficient used to apply the forward friction force closer to the car's center of mass. 1 applies the force at the wheel position, 0 applies the force at the point along the contact normal closest to the center of mass.
> ``` lang=cpp, name=Nada
> var WheelFrictionFrontRollCoef : Real


---  
 #  WheelFrictionSideRollCoef : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Coefficient used to apply the side friction force closer to the car's center of mass. 1 applies the force at the wheel position, 0 applies the force at the point along the contact normal closest to the center of mass.
> ``` lang=cpp, name=Nada
> var WheelFrictionSideRollCoef : Real


---  
 #  Methods


---  
 #  NumberOfWheelsInContact : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> The number of wheels currently in contact with an object.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function NumberOfWheelsInContact() : Integer
> ``` 


---  
 #  PhysicsCar : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function PhysicsCar()
> ``` 


---  
 

 
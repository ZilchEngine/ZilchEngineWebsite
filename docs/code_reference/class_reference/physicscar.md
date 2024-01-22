 `Component` `Physics`



(NOTE) A controller for a high speed physics based car. The car is controlled with a steer, gas, and brake scalar. The car will raycast wheel positions to try to keep the wheels on the ground and then apply friction and normal forces to propel the car.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[NumberOfWheelsInContact](physicscar.md#numberofwheelsincontact)|[Active](physicscar.md#active-zilch-engine-docum)|[component](component.md)| |
|[Constructor](physicscar.md#physicscar-void)|[AntiLockBrakes](physicscar.md#antilockbrakes-zilch-engi)| | |
| |[Brake](physicscar.md#brake-zilch-engine-docume)| | |
| |[DebugDraw](physicscar.md#debugdraw-zilch-engine-do)| | |
| |[Gas](physicscar.md#gas-zilch-engine-document)| | |
| |[GripScalar](physicscar.md#gripscalar-zilch-engine-d)| | |
| |[MaxSpeed](physicscar.md#maxspeed-zilch-engine-doc)| | |
| |[MaxTorque](physicscar.md#maxtorque-zilch-engine-do)| | |
| |[Steer](physicscar.md#steer-zilch-engine-docume)| | |
| |[TorqueGovernor](physicscar.md#torquegovernor-zilch-engi)| | |
| |[WheelCogs](physicscar.md#wheelcogs-zilch-engine-do)| | |
| |[WheelFrictionFrontRollCoef](physicscar.md#wheelfrictionfrontrollco)| | |
| |[WheelFrictionSideRollCoef](physicscar.md#wheelfrictionsiderollcoe)| | |


 #  Properties


---  
 #  Active : [boolean](../nada_base_types/boolean.md)

> Whether or not the car will run any logic at all. If this is false wheels will not work, they will not behave as springs, drive, or anything else.
> ```TS:Nada
> var Active : Boolean


---  
 #  AntiLockBrakes : [boolean](../nada_base_types/boolean.md)

> Prevents the car from entering dynamic friction when applying brakes. If the brake would start to skid, the brake force is clamped to the max amount that will not slip.
> ```TS:Nada
> var AntiLockBrakes : Boolean


---  
 #  Brake : [real](../nada_base_types/real.md)

> How much the brake is being pressed [0,1] where 1 is full brake.
> ```TS:Nada
> var Brake : Real


---  
 #  DebugDraw : [boolean](../nada_base_types/boolean.md)

> Whether or not the car should debug draw.
> ```TS:Nada
> var DebugDraw : Boolean


---  
 #  Gas : [real](../nada_base_types/real.md)

> How much the gas is being pressed [-1,1] where -1 is full reverse.
> ```TS:Nada
> var Gas : Real


---  
 #  GripScalar : [real](../nada_base_types/real.md)

> Artificially increases the grip of the car (where 2 is twice the grip). The total grip scalar is computed as CarGripScalar * WheelGripScalar so the total car can be easily tweaked while allowing individual wheel tweaks.
> ```TS:Nada
> var GripScalar : Real


---  
 #  MaxSpeed : [real](../nada_base_types/real.md)

> The desired maximum speed of the car. Similar to a speed governor.
> ```TS:Nada
> var MaxSpeed : Real


---  
 #  MaxTorque : [real](../nada_base_types/real.md)

> The maximum torque the engine can apply to try to reach the max speed.
> ```TS:Nada
> var MaxTorque : Real


---  
 #  Steer : [real](../nada_base_types/real.md)

> How much the wheel is being steered. This is measured in radians about this object's y-axis.
> ```TS:Nada
> var Steer : Real


---  
 #  TorqueGovernor : [boolean](../nada_base_types/boolean.md)

> Governs the max torque that the engine can apply. This is used to keep the wheels from spinning out (slipping) when too high of a torque is applied. If the tires would slip, the engine will apply the maximum torque for the tires to not slip.
> ```TS:Nada
> var TorqueGovernor : Boolean


---  
 #  WheelCogs : [carwheelarray](carwheelarray.md)

 `read-only`

> Read-only array of wheels belonging to this car.
> ```TS:Nada
> var WheelCogs : CarWheelArray


---  
 #  WheelFrictionFrontRollCoef : [real](../nada_base_types/real.md)

> Coefficient used to apply the forward friction force closer to the car's center of mass. 1 applies the force at the wheel position, 0 applies the force at the point along the contact normal closest to the center of mass.
> ```TS:Nada
> var WheelFrictionFrontRollCoef : Real


---  
 #  WheelFrictionSideRollCoef : [real](../nada_base_types/real.md)

> Coefficient used to apply the side friction force closer to the car's center of mass. 1 applies the force at the wheel position, 0 applies the force at the point along the contact normal closest to the center of mass.
> ```TS:Nada
> var WheelFrictionSideRollCoef : Real


---  
 #  Methods


---  
 #  NumberOfWheelsInContact : [integer](../nada_base_types/integer.md)

> The number of wheels currently in contact with an object.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function NumberOfWheelsInContact() : Integer
> ``` 


---  
 #  PhysicsCar : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function PhysicsCar()
> ``` 


---  
 

 
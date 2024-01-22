 `Component` `Physics`



(NOTE) A wheel for a high speed physics based car. Each wheel contains properties to describe how to interact with the world (eg. spring forces, friction, etc...).

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](physicscarwheel.md#physicscarwheel-void)|[Active](physicscarwheel.md#active-zilch-engine-docum)|[component](component.md)| |
| |[ContactedObject](physicscarwheel.md#contactedobject-zilch-eng)| | |
| |[ContactNormal](physicscarwheel.md#contactnormal-zilch-engin)| | |
| |[ContactPoint](physicscarwheel.md#contactpoint-zilch-engine)| | |
| |[DampingCompressionRatio](physicscarwheel.md#dampingcompressionratio)| | |
| |[DampingRelaxationRatio](physicscarwheel.md#dampingrelaxationratio-z)| | |
| |[DriveFactor](physicscarwheel.md#drivefactor-zilch-engine)| | |
| |[ForwardDynamicFriction](physicscarwheel.md#forwarddynamicfriction-z)| | |
| |[ForwardImpulse](physicscarwheel.md#forwardimpulse-zilch-engi)| | |
| |[ForwardStaticFriction](physicscarwheel.md#forwardstaticfriction-ze)| | |
| |[FrequencyHz](physicscarwheel.md#frequencyhz-zilch-engine)| | |
| |[Grip](physicscarwheel.md#grip-zilch-engine-documen)| | |
| |[GripScalar](physicscarwheel.md#gripscalar-zilch-engine-d)| | |
| |[Is2DWheel](physicscarwheel.md#is2dwheel-zilch-engine-do)| | |
| |[IsDriveWheel](physicscarwheel.md#isdrivewheel-zilch-engine)| | |
| |[IsInContact](physicscarwheel.md#isincontact-zilch-engine)| | |
| |[IsSliding](physicscarwheel.md#issliding-zilch-engine-do)| | |
| |[MaxBrakeStrength](physicscarwheel.md#maxbrakestrength-zilch-en)| | |
| |[MaxSpringCompressionDistance](physicscarwheel.md#maxspringcompressiondist)| | |
| |[MaxSpringForce](physicscarwheel.md#maxspringforce-zilch-engi)| | |
| |[MaxSpringRelaxationDistance](physicscarwheel.md#maxspringrelaxationdista)| | |
| |[NormalImpulse](physicscarwheel.md#normalimpulse-zilch-engin)| | |
| |[PhysicsCarPath](physicscarwheel.md#physicscarpath-zilch-engi)| | |
| |[PreRotation](physicscarwheel.md#prerotation-zilch-engine)| | |
| |[Radius](physicscarwheel.md#radius-zilch-engine-docum)| | |
| |[Rotation](physicscarwheel.md#rotation-zilch-engine-doc)| | |
| |[RotationalVelocity](physicscarwheel.md#rotationalvelocity-zero)| | |
| |[SideDynamicFriction](physicscarwheel.md#sidedynamicfriction-zero)| | |
| |[SideImpulse](physicscarwheel.md#sideimpulse-zilch-engine)| | |
| |[SideStaticFriction](physicscarwheel.md#sidestaticfriction-zero)| | |
| |[SpringLength](physicscarwheel.md#springlength-zilch-engine)| | |
| |[SpringMaxLength](physicscarwheel.md#springmaxlength-zilch-eng)| | |
| |[SpringMinLength](physicscarwheel.md#springminlength-zilch-eng)| | |
| |[SpringRestLength](physicscarwheel.md#springrestlength-zilch-en)| | |
| |[SpringStartLength](physicscarwheel.md#springstartlength-zilch-e)| | |
| |[SteerFactor](physicscarwheel.md#steerfactor-zilch-engine)| | |
| |[WheelLocalStartPosition](physicscarwheel.md#wheellocalstartposition)| | |
| |[WorldAngularVelocity](physicscarwheel.md#worldangularvelocity-zer)| | |
| |[WorldAxleAxis](physicscarwheel.md#worldaxleaxis-zilch-engin)| | |
| |[WorldForwardAxis](physicscarwheel.md#worldforwardaxis-zilch-en)| | |
| |[WorldLinearVelocity](physicscarwheel.md#worldlinearvelocity-zero)| | |
| |[WorldSpringAxis](physicscarwheel.md#worldspringaxis-zilch-eng)| | |
| |[WorldWheelBasis](physicscarwheel.md#worldwheelbasis-zilch-eng)| | |


 #  Properties


---  
 #  Active : [boolean](../nada_base_types/boolean.md)

> Should this wheel calculate forces for the current PhysicsCar.
> ```TS:Nada
> var Active : Boolean


---  
 #  ContactedObject : [cog](cog.md)

 `read-only`

> The object that this wheel is currently in contact with.
> ```TS:Nada
> var ContactedObject : Cog


---  
 #  ContactNormal : [real3](../nada_base_types/real3.md)

 `read-only`

> The normal of the surface where the wheel is currently in contact. Will be the zero vector if there is no contact.
> ```TS:Nada
> var ContactNormal : Real3


---  
 #  ContactPoint : [real3](../nada_base_types/real3.md)

 `read-only`

> The point in world space where the wheel is currently in contact. Will be the zero vector if there is no contact.
> ```TS:Nada
> var ContactPoint : Real3


---  
 #  DampingCompressionRatio : [real](../nada_base_types/real.md)

> The damping ratio when the spring is compressing (0: no damping, 1 critical damping)
> ```TS:Nada
> var DampingCompressionRatio : Real


---  
 #  DampingRelaxationRatio : [real](../nada_base_types/real.md)

> The damping ratio when the spring is relaxing (0: no damping, 1 critical damping)
> ```TS:Nada
> var DampingRelaxationRatio : Real


---  
 #  DriveFactor : [real](../nada_base_types/real.md)

> Used to alter the direction this wheel turns when the motor receives power. Typically set to 1 or -1. Useful to cause a wheel to temporarily rotate backwards without having to change its basis.
> ```TS:Nada
> var DriveFactor : Real


---  
 #  ForwardDynamicFriction : [real](../nada_base_types/real.md)

> Determines the force applied in the forward direction when the wheel is in dynamic friction and therefore slipping. (i.e. force = muK * Fnormal)
> ```TS:Nada
> var ForwardDynamicFriction : Real


---  
 #  ForwardImpulse : [real](../nada_base_types/real.md)

 `read-only`

> The forward impulse (drive force) being exerted by the wheel.
> ```TS:Nada
> var ForwardImpulse : Real


---  
 #  ForwardStaticFriction : [real](../nada_base_types/real.md)

> Used with Coulomb's friction to determine when the wheel will start slipping in the forward direction. (i.e. the friction is bound by muS * Fnormal).
> ```TS:Nada
> var ForwardStaticFriction : Real


---  
 #  FrequencyHz : [real](../nada_base_types/real.md)

> The frequency at which the spring of this wheel oscillates per second.
> ```TS:Nada
> var FrequencyHz : Real


---  
 #  Grip : [real](../nada_base_types/real.md)

 `read-only`

> A coefficient from 0 to 1 that represents how much grip the wheel has.
> ```TS:Nada
> var Grip : Real


---  
 #  GripScalar : [real](../nada_base_types/real.md)

> Artificially increases the grip of the car (where 2 is twice the grip). The total grip scalar is computed as CarGripScalar * WheelGripScalar so the total car can be easily tweaked while allowing individual wheel tweaks.
> ```TS:Nada
> var GripScalar : Real


---  
 #  Is2DWheel : [boolean](../nada_base_types/boolean.md)

> Does this wheel only operate in 2D? Ignores the side friction axis.
> ```TS:Nada
> var Is2DWheel : Boolean


---  
 #  IsDriveWheel : [boolean](../nada_base_types/boolean.md)

> Drive wheels turn when the car body has gas pressed.
> ```TS:Nada
> var IsDriveWheel : Boolean


---  
 #  IsInContact : [boolean](../nada_base_types/boolean.md)

 `read-only`

> If the wheel is currently in contact with an object.
> ```TS:Nada
> var IsInContact : Boolean


---  
 #  IsSliding : [boolean](../nada_base_types/boolean.md)

 `read-only`

> If the wheel is currently sliding. This means that the wheel is slipping from spinning too fast (using dynamic friction instead of static).
> ```TS:Nada
> var IsSliding : Boolean


---  
 #  MaxBrakeStrength : [real](../nada_base_types/real.md)

> The max force that this wheel can exert to break.
> ```TS:Nada
> var MaxBrakeStrength : Real


---  
 #  MaxSpringCompressionDistance : [real](../nada_base_types/real.md)

> The max distance that a spring can compress in one frame.
> ```TS:Nada
> var MaxSpringCompressionDistance : Real


---  
 #  MaxSpringForce : [real](../nada_base_types/real.md)

> The maximum force that the wheel's spring can exert.
> ```TS:Nada
> var MaxSpringForce : Real


---  
 #  MaxSpringRelaxationDistance : [real](../nada_base_types/real.md)

> The max distance that a spring can relax in one frame.
> ```TS:Nada
> var MaxSpringRelaxationDistance : Real


---  
 #  NormalImpulse : [real](../nada_base_types/real.md)

 `read-only`

> The normal impulse (spring force) being exerted by the wheel.
> ```TS:Nada
> var NormalImpulse : Real


---  
 #  PhysicsCarPath : [cogpath](cogpath.md)

> The path to the car that this is a wheel for.
> ```TS:Nada
> var PhysicsCarPath : CogPath


---  
 #  PreRotation : [quaternion](../nada_base_types/quaternion.md)

> Used to rotate the wheel before taking into account it's transform. Typically used to rotate a cylinder to align with a model.
> ```TS:Nada
> var PreRotation : Quaternion


---  
 #  Radius : [real](../nada_base_types/real.md)

> The radius of the wheel.
> ```TS:Nada
> var Radius : Real


---  
 #  Rotation : [real](../nada_base_types/real.md)

 `read-only`

> The current rotation of the wheel in radians about it's axle.
> ```TS:Nada
> var Rotation : Real


---  
 #  RotationalVelocity : [real](../nada_base_types/real.md)

 `read-only`

> The current rotational velocity of the wheel about it's axle.
> ```TS:Nada
> var RotationalVelocity : Real


---  
 #  SideDynamicFriction : [real](../nada_base_types/real.md)

> Same as ForwardDynamicFriction, but in the side direction. See SideStaticFriction for a why these are separated.
> ```TS:Nada
> var SideDynamicFriction : Real


---  
 #  SideImpulse : [real](../nada_base_types/real.md)

 `read-only`

> The side impulse (side friction) being exerted by the wheel.
> ```TS:Nada
> var SideImpulse : Real


---  
 #  SideStaticFriction : [real](../nada_base_types/real.md)

> Same as ForwardStaticFriction, but in the side direction. Forward and side friction are separated since the forward direction is rolling friction and the side direction is sliding friction.
> ```TS:Nada
> var SideStaticFriction : Real


---  
 #  SpringLength : [real](../nada_base_types/real.md)

 `read-only`

> The current length of the spring.
> ```TS:Nada
> var SpringLength : Real


---  
 #  SpringMaxLength : [real](../nada_base_types/real.md)

> The maximum length of the spring of the wheel. If the wheel hits something further away than this length (plus the wheel radius) then that object will be ignored.
> ```TS:Nada
> var SpringMaxLength : Real


---  
 #  SpringMinLength : [real](../nada_base_types/real.md)

> The minimum length of the spring of the wheel. If a wheel cast hits an object at a time before min but after start then the wheel will still collide with this object but the spring forces and visuals will be at the min spring length. This is useful for putting the starting raycast position inside of the object so as to avoid tunneling but still having the wheel only visually display where it should.
> ```TS:Nada
> var SpringMinLength : Real


---  
 #  SpringRestLength : [real](../nada_base_types/real.md)

> The rest length of the spring.
> ```TS:Nada
> var SpringRestLength : Real


---  
 #  SpringStartLength : [real](../nada_base_types/real.md)

> The t value to start the raycast at. This t value is 0 at the wheel position and travels in the direction of the wheel spring direction. This value is used to modify where the raycast actually starts relative to the start position.
> ```TS:Nada
> var SpringStartLength : Real


---  
 #  SteerFactor : [real](../nada_base_types/real.md)

> How much this wheel steers. [0, 1] where 1 is the max steering of the car.
> ```TS:Nada
> var SteerFactor : Real


---  
 #  WheelLocalStartPosition : [real3](../nada_base_types/real3.md)

> The local position on the car body that the wheel starts at (raycasts from).
> ```TS:Nada
> var WheelLocalStartPosition : Real3


---  
 #  WorldAngularVelocity : [real3](../nada_base_types/real3.md)

 `read-only`

> The axis that represents the world angular velocity of the wheel.
> ```TS:Nada
> var WorldAngularVelocity : Real3


---  
 #  WorldAxleAxis : [real3](../nada_base_types/real3.md)

 `read-only`

> The current axis of the wheel's axle in world space.
> ```TS:Nada
> var WorldAxleAxis : Real3


---  
 #  WorldForwardAxis : [real3](../nada_base_types/real3.md)

 `read-only`

> The current axis of the wheel's forward in world space.
> ```TS:Nada
> var WorldForwardAxis : Real3


---  
 #  WorldLinearVelocity : [real3](../nada_base_types/real3.md)

 `read-only`

> The velocity of the center of the wheel while taking into account the car's velocity.
> ```TS:Nada
> var WorldLinearVelocity : Real3


---  
 #  WorldSpringAxis : [real3](../nada_base_types/real3.md)

 `read-only`

> The current world-space spring axis of the wheel.
> ```TS:Nada
> var WorldSpringAxis : Real3


---  
 #  WorldWheelBasis : [quaternion](../nada_base_types/quaternion.md)

> Determines what directions the forward, axle, and spring are on the wheel. The forward direction is taken from the x-axis of the basis. Likewise the axle is from the y-axis and the spring is from the z-axis. Use ToQuaternion to construct this.
> ```TS:Nada
> var WorldWheelBasis : Quaternion


---  
 #  Methods


---  
 #  PhysicsCarWheel : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function PhysicsCarWheel()
> ``` 


---  
 

 
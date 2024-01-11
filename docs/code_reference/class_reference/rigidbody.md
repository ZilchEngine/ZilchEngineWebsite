 `Component` `Physics`



(NOTE) RigidBody defines the inertia (mass, velocity, etc...) of a rigid object. Any PhysicsEffects attached to a RigidBody without a region will be applied to the center of mass of this body.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ApplyAngularImpulse](rigidbody.md#applyangularimpulse-void)|[ ActiveBody](rigidbody.md#activebody-zilch-engine-d)|[component](component.md)| |
|[ ApplyAngularVelocity](rigidbody.md#applyangularvelocity-voi)|[ AllowSleep](rigidbody.md#allowsleep-zilch-engine-d)| | |
|[ ApplyForce](rigidbody.md#applyforce-void)|[ AngularVelocity](rigidbody.md#angularvelocity-zilch-eng)| | |
|[ ApplyForceAtOffsetVector](rigidbody.md#applyforceatoffsetvector)|[ Asleep](rigidbody.md#asleep-zilch-engine-docum)| | |
|[ ApplyForceAtOffsetVectorNoWakeUp](rigidbody.md#applyforceatoffsetvector)|[ DynamicState](rigidbody.md#dynamicstate-zilch-engine)| | |
|[ ApplyForceAtPoint](rigidbody.md#applyforceatpoint-void)|[ Force](rigidbody.md#force-zilch-engine-docume)| | |
|[ ApplyForceAtPointNoWakeUp](rigidbody.md#applyforceatpointnowakeu)|[ LocalInverseInertiaTensor](rigidbody.md#localinverseinertiatenso)| | |
|[ ApplyForceNoWakeUp](rigidbody.md#applyforcenowakeup-void)|[ Mass](rigidbody.md#mass-zilch-engine-documen)| | |
|[ ApplyImpulseAtOffsetVector](rigidbody.md#applyimpulseatoffsetvect)|[ Mode2D](rigidbody.md#mode2d-zilch-engine-docum)| | |
|[ ApplyImpulseAtPoint](rigidbody.md#applyimpulseatpoint-void)|[ RotationLocked](rigidbody.md#rotationlocked-zilch-engi)| | |
|[ ApplyLinearImpulse](rigidbody.md#applylinearimpulse-void)|[ Torque](rigidbody.md#torque-zilch-engine-docum)| | |
|[ ApplyLinearVelocity](rigidbody.md#applylinearvelocity-void)|[ Velocity](rigidbody.md#velocity-zilch-engine-doc)| | |
|[ ApplyTorque](rigidbody.md#applytorque-void)|[ WorldCenterOfMass](rigidbody.md#worldcenterofmass-zilch-e)| | |
|[ ApplyTorqueNoWakeUp](rigidbody.md#applytorquenowakeup-void)|[ WorldInverseInertiaTensor](rigidbody.md#worldinverseinertiatenso)| | |
|[ ApplyVelocityAtPoint](rigidbody.md#applyvelocityatpoint-voi)| | | |
|[ ForceAsleep](rigidbody.md#forceasleep-void)| | | |
|[ ForceAwake](rigidbody.md#forceawake-void)| | | |
|[ GetPointVelocity](rigidbody.md#getpointvelocity-zilch-en)| | | |
|[ Constructor](rigidbody.md#rigidbody-void)| | | |


 #  Properties


---  
 #  ActiveBody : [rigidbody](rigidbody.md)

 `read-only`

> If this is a static body then the active body (the one force/velocity should be applied to or calculated from) is the nearest parent body up the hierarchy that is not static. If one isn't found then this returns the current rigid body (this).
> ```TS:Nada
> var ActiveBody : RigidBody


---  
 #  AllowSleep : [boolean](../nada_base_types/boolean.md)

> Sleeping happens when an object has not "moved" (small enough linear + angular velocity) for long enough. If this happens then the physics engine stops updating this object (integration, collision detection, etc...) until an awake object hits it. Sleeping is purely an optimization. Sometimes it is not desirable for a body to ever fall asleep (such as a player).
> ```TS:Nada
> var AllowSleep : Boolean


---  
 #  AngularVelocity : [real3](../nada_base_types/real3.md)

> The angular velocity (radians per second) of this body in world space. Objects will rotate about this axis using the right-hand rule. Max bounds are around 1e+10, after this the angular velocity will be capped. Setting this will wake up the body if it's asleep.
> ```TS:Nada
> var AngularVelocity : Real3


---  
 #  Asleep : [boolean](../nada_base_types/boolean.md)

> Whether or not this object is currently asleep. Setting this to true will force the object asleep even if this causes invalid behavior (objects floating).
> ```TS:Nada
> var Asleep : Boolean


---  
 #  DynamicState : [RigidBodyDynamicState](../enum_reference.md#rigidbodydynamicstate)

> How this rigid body handles dynamics. Is it a regular rigid body (dynamic)? Does it not move (static)? Does the user want to manually move it and have objects properly collide with it (kinematic)? Note: Static vs. static does not check for collision.
> ```TS:Nada
> var DynamicState : RigidBodyDynamicState


---  
 #  Force : [real3](../nada_base_types/real3.md)

> The total accumulated force (in world space) that is being applied to the center of mass of this rigid body this frame. Setting this will wake up the body if it's asleep.
> ```TS:Nada
> var Force : Real3


---  
 #  LocalInverseInertiaTensor : [real3x3](../nada_base_types/real3x3.md)

 `read-only`

> The inverse inertia tensor in local space of this body. The local space inertia tensor doesn't change when the object rotates but is not typically useful for any calculations other than computing the world-space inverse inertia tensor.
> ```TS:Nada
> var LocalInverseInertiaTensor : Real3x3


---  
 #  Mass : [real](../nada_base_types/real.md)

 `read-only`

> The current mass of the rigid body. This includes all child colliders belonging to this body.
> ```TS:Nada
> var Mass : Real


---  
 #  Mode2D : [Mode2DStates](../enum_reference.md#mode2dstates)

> Used to make an object act as if it were 2D. This is done by locking it to the current z-plane and only allowing rotation about the world's z-axis. Objects can be set to always be 2D or 3D, or this can be deferred to the PhysicsSpace's Mode2D.
> ```TS:Nada
> var Mode2D : Mode2DStates


---  
 #  RotationLocked : [boolean](../nada_base_types/boolean.md)

> Makes physics unable to rotate this object. Manual rotations can still be applied.
> ```TS:Nada
> var RotationLocked : Boolean


---  
 #  Torque : [real3](../nada_base_types/real3.md)

> The total accumulated torque (in world space) that is being applied to the center of mass of this rigid body this frame. Setting this will wake up the body if it's asleep.
> ```TS:Nada
> var Torque : Real3


---  
 #  Velocity : [real3](../nada_base_types/real3.md)

> The velocity (units per second) of this body in world space. Max bounds are around 1e+10, after this the velocity will be capped. Setting this will wake up the body if it's asleep.
> ```TS:Nada
> var Velocity : Real3


---  
 #  WorldCenterOfMass : [real3](../nada_base_types/real3.md)

 `read-only`

> The position of the center of mass in world space.
> ```TS:Nada
> var WorldCenterOfMass : Real3


---  
 #  WorldInverseInertiaTensor : [real3x3](../nada_base_types/real3x3.md)

 `read-only`

> The inverse inertia tensor in world space of this body. Describes how hard it is to rotate an object about the world-space axes. Useful to convert any torque into an angular velocity.
> ```TS:Nada
> var WorldInverseInertiaTensor : Real3x3


---  
 #  Methods


---  
 #  ApplyAngularImpulse : Void

> Applies an angular impulse through the center of mass (world space). Only results in a change of angular velocity. Will wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |angular|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function ApplyAngularImpulse(angular : Real3)
> ``` 


---  
 #  ApplyAngularVelocity : Void

> Adds to the current angular velocity (world space). Will wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |angular|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function ApplyAngularVelocity(angular : Real3)
> ``` 


---  
 #  ApplyForce : Void

> Applies a force through the center of mass of the body (world space). Will wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |force|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function ApplyForce(force : Real3)
> ``` 


---  
 #  ApplyForceAtOffsetVector : Void

> Applies a force at an offset from the center of mass (world space). Results in a force and torque to the center of mass. Will wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |force|[real3](../nada_base_types/real3.md)| |
> |worldOffset|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function ApplyForceAtOffsetVector(force : Real3, worldOffset : Real3)
> ``` 


---  
 #  ApplyForceAtOffsetVectorNoWakeUp : Void

> Applies a force at an offset from the center of mass (world space). Results in a force and torque to the center of mass. Will not wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |force|[real3](../nada_base_types/real3.md)| |
> |worldOffset|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function ApplyForceAtOffsetVectorNoWakeUp(force : Real3, worldOffset : Real3)
> ``` 


---  
 #  ApplyForceAtPoint : Void

> Applies a force at a world point (world space). Results in a force and torque to the center of mass. Will wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |force|[real3](../nada_base_types/real3.md)| |
> |worldPoint|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function ApplyForceAtPoint(force : Real3, worldPoint : Real3)
> ``` 


---  
 #  ApplyForceAtPointNoWakeUp : Void

> Applies a force at a world point (world space). Results in a force and torque to the center of mass. Will not wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |force|[real3](../nada_base_types/real3.md)| |
> |worldPoint|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function ApplyForceAtPointNoWakeUp(force : Real3, worldPoint : Real3)
> ``` 


---  
 #  ApplyForceNoWakeUp : Void

> Applies a force through the center of mass of the body (world space). Will not wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |force|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function ApplyForceNoWakeUp(force : Real3)
> ``` 


---  
 #  ApplyImpulseAtOffsetVector : Void

> Applies an impulse at on offset from the center of mass (world space). Results in a change in linear and angular velocity. Will wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |impulse|[real3](../nada_base_types/real3.md)| |
> |worldOffset|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function ApplyImpulseAtOffsetVector(impulse : Real3, worldOffset : Real3)
> ``` 


---  
 #  ApplyImpulseAtPoint : Void

> Applies an impulse at a world point (world space). Results in a change to linear and angular velocity. Will wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |impulse|[real3](../nada_base_types/real3.md)| |
> |worldPoint|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function ApplyImpulseAtPoint(impulse : Real3, worldPoint : Real3)
> ``` 


---  
 #  ApplyLinearImpulse : Void

> Applies a linear impulse through the center of mass (world space). Only results in a change of linear velocity. Will wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |linear|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function ApplyLinearImpulse(linear : Real3)
> ``` 


---  
 #  ApplyLinearVelocity : Void

> Adds to the current linear velocity (world space). Will wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |linear|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function ApplyLinearVelocity(linear : Real3)
> ``` 


---  
 #  ApplyTorque : Void

> Applies a torque through the center of mass of the body (world space). Will wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |torque|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function ApplyTorque(torque : Real3)
> ``` 


---  
 #  ApplyTorqueNoWakeUp : Void

> Applies a torque through the center of mass of the body (world space). Will not wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |torque|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function ApplyTorqueNoWakeUp(torque : Real3)
> ``` 


---  
 #  ApplyVelocityAtPoint : Void

> Applies a velocity at a world space point on the object. Results in a change to linear and angular velocity. Will wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |velocity|[real3](../nada_base_types/real3.md)| |
> |worldPoint|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function ApplyVelocityAtPoint(velocity : Real3, worldPoint : Real3)
> ``` 


---  
 #  ForceAsleep : Void

> Forces the object asleep. Warning: calling this function could create gameplay flaws if used incorrectly, use at your own risk (and sparingly).
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ForceAsleep()
> ``` 


---  
 #  ForceAwake : Void

> Forces the object awake. Will reset the sleep timer.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ForceAwake()
> ``` 


---  
 #  GetPointVelocity : [real3](../nada_base_types/real3.md)

> Computes the linear point velocity of world-space point.
> |Name|Type|Description|
> |---|---|---|
> |worldPoint|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function GetPointVelocity(worldPoint : Real3) : Real3
> ``` 


---  
 #  RigidBody : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function RigidBody()
> ``` 


---  
 

 
 `Component` `Physics`



(NOTE) RigidBody defines the inertia (mass, velocity, etc...) of a rigid object. Any PhysicsEffects attached to a RigidBody without a region will be applied to the center of mass of this body.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ApplyAngularImpulse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#applyangularimpulse-void)|[ ActiveBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#activebody-zilch-engine-d)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)| |
|[ ApplyAngularVelocity](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#applyangularvelocity-voi)|[ AllowSleep](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#allowsleep-zilch-engine-d)| | |
|[ ApplyForce](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#applyforce-void)|[ AngularVelocity](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#angularvelocity-zilch-eng)| | |
|[ ApplyForceAtOffsetVector](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#applyforceatoffsetvector)|[ Asleep](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#asleep-zilch-engine-docum)| | |
|[ ApplyForceAtOffsetVectorNoWakeUp](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#applyforceatoffsetvector)|[ DynamicState](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#dynamicstate-zilch-engine)| | |
|[ ApplyForceAtPoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#applyforceatpoint-void)|[ Force](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#force-zilch-engine-docume)| | |
|[ ApplyForceAtPointNoWakeUp](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#applyforceatpointnowakeu)|[ LocalInverseInertiaTensor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#localinverseinertiatenso)| | |
|[ ApplyForceNoWakeUp](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#applyforcenowakeup-void)|[ Mass](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#mass-zilch-engine-documen)| | |
|[ ApplyImpulseAtOffsetVector](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#applyimpulseatoffsetvect)|[ Mode2D](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#mode2d-zilch-engine-docum)| | |
|[ ApplyImpulseAtPoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#applyimpulseatpoint-void)|[ RotationLocked](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#rotationlocked-zilch-engi)| | |
|[ ApplyLinearImpulse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#applylinearimpulse-void)|[ Torque](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#torque-zilch-engine-docum)| | |
|[ ApplyLinearVelocity](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#applylinearvelocity-void)|[ Velocity](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#velocity-zilch-engine-doc)| | |
|[ ApplyTorque](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#applytorque-void)|[ WorldCenterOfMass](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#worldcenterofmass-zilch-e)| | |
|[ ApplyTorqueNoWakeUp](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#applytorquenowakeup-void)|[ WorldInverseInertiaTensor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#worldinverseinertiatenso)| | |
|[ ApplyVelocityAtPoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#applyvelocityatpoint-voi)| | | |
|[ ForceAsleep](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#forceasleep-void)| | | |
|[ ForceAwake](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#forceawake-void)| | | |
|[ GetPointVelocity](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#getpointvelocity-zilch-en)| | | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md#rigidbody-void)| | | |


 #  Properties


---  
 #  ActiveBody : [rigidbody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)

 `read-only`

> If this is a static body then the active body (the one force/velocity should be applied to or calculated from) is the nearest parent body up the hierarchy that is not static. If one isn't found then this returns the current rigid body (this).
> ``` lang=cpp, name=Nada
> var ActiveBody : RigidBody


---  
 #  AllowSleep : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Sleeping happens when an object has not "moved" (small enough linear + angular velocity) for long enough. If this happens then the physics engine stops updating this object (integration, collision detection, etc...) until an awake object hits it. Sleeping is purely an optimization. Sometimes it is not desirable for a body to ever fall asleep (such as a player).
> ``` lang=cpp, name=Nada
> var AllowSleep : Boolean


---  
 #  AngularVelocity : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The angular velocity (radians per second) of this body in world space. Objects will rotate about this axis using the right-hand rule. Max bounds are around 1e+10, after this the angular velocity will be capped. Setting this will wake up the body if it's asleep.
> ``` lang=cpp, name=Nada
> var AngularVelocity : Real3


---  
 #  Asleep : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Whether or not this object is currently asleep. Setting this to true will force the object asleep even if this causes invalid behavior (objects floating).
> ``` lang=cpp, name=Nada
> var Asleep : Boolean


---  
 #  DynamicState : [RigidBodyDynamicState](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#rigidbodydynamicstate)

> How this rigid body handles dynamics. Is it a regular rigid body (dynamic)? Does it not move (static)? Does the user want to manually move it and have objects properly collide with it (kinematic)? Note: Static vs. static does not check for collision.
> ``` lang=cpp, name=Nada
> var DynamicState : RigidBodyDynamicState


---  
 #  Force : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The total accumulated force (in world space) that is being applied to the center of mass of this rigid body this frame. Setting this will wake up the body if it's asleep.
> ``` lang=cpp, name=Nada
> var Force : Real3


---  
 #  LocalInverseInertiaTensor : [real3x3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3x3.md)

 `read-only`

> The inverse inertia tensor in local space of this body. The local space inertia tensor doesn't change when the object rotates but is not typically useful for any calculations other than computing the world-space inverse inertia tensor.
> ``` lang=cpp, name=Nada
> var LocalInverseInertiaTensor : Real3x3


---  
 #  Mass : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

 `read-only`

> The current mass of the rigid body. This includes all child colliders belonging to this body.
> ``` lang=cpp, name=Nada
> var Mass : Real


---  
 #  Mode2D : [Mode2DStates](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#mode2dstates)

> Used to make an object act as if it were 2D. This is done by locking it to the current z-plane and only allowing rotation about the world's z-axis. Objects can be set to always be 2D or 3D, or this can be deferred to the PhysicsSpace's Mode2D.
> ``` lang=cpp, name=Nada
> var Mode2D : Mode2DStates


---  
 #  RotationLocked : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Makes physics unable to rotate this object. Manual rotations can still be applied.
> ``` lang=cpp, name=Nada
> var RotationLocked : Boolean


---  
 #  Torque : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The total accumulated torque (in world space) that is being applied to the center of mass of this rigid body this frame. Setting this will wake up the body if it's asleep.
> ``` lang=cpp, name=Nada
> var Torque : Real3


---  
 #  Velocity : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The velocity (units per second) of this body in world space. Max bounds are around 1e+10, after this the velocity will be capped. Setting this will wake up the body if it's asleep.
> ``` lang=cpp, name=Nada
> var Velocity : Real3


---  
 #  WorldCenterOfMass : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

 `read-only`

> The position of the center of mass in world space.
> ``` lang=cpp, name=Nada
> var WorldCenterOfMass : Real3


---  
 #  WorldInverseInertiaTensor : [real3x3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3x3.md)

 `read-only`

> The inverse inertia tensor in world space of this body. Describes how hard it is to rotate an object about the world-space axes. Useful to convert any torque into an angular velocity.
> ``` lang=cpp, name=Nada
> var WorldInverseInertiaTensor : Real3x3


---  
 #  Methods


---  
 #  ApplyAngularImpulse : Void

> Applies an angular impulse through the center of mass (world space). Only results in a change of angular velocity. Will wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |angular|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function ApplyAngularImpulse(angular : Real3)
> ``` 


---  
 #  ApplyAngularVelocity : Void

> Adds to the current angular velocity (world space). Will wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |angular|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function ApplyAngularVelocity(angular : Real3)
> ``` 


---  
 #  ApplyForce : Void

> Applies a force through the center of mass of the body (world space). Will wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |force|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function ApplyForce(force : Real3)
> ``` 


---  
 #  ApplyForceAtOffsetVector : Void

> Applies a force at an offset from the center of mass (world space). Results in a force and torque to the center of mass. Will wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |force|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |worldOffset|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function ApplyForceAtOffsetVector(force : Real3, worldOffset : Real3)
> ``` 


---  
 #  ApplyForceAtOffsetVectorNoWakeUp : Void

> Applies a force at an offset from the center of mass (world space). Results in a force and torque to the center of mass. Will not wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |force|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |worldOffset|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function ApplyForceAtOffsetVectorNoWakeUp(force : Real3, worldOffset : Real3)
> ``` 


---  
 #  ApplyForceAtPoint : Void

> Applies a force at a world point (world space). Results in a force and torque to the center of mass. Will wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |force|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |worldPoint|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function ApplyForceAtPoint(force : Real3, worldPoint : Real3)
> ``` 


---  
 #  ApplyForceAtPointNoWakeUp : Void

> Applies a force at a world point (world space). Results in a force and torque to the center of mass. Will not wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |force|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |worldPoint|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function ApplyForceAtPointNoWakeUp(force : Real3, worldPoint : Real3)
> ``` 


---  
 #  ApplyForceNoWakeUp : Void

> Applies a force through the center of mass of the body (world space). Will not wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |force|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function ApplyForceNoWakeUp(force : Real3)
> ``` 


---  
 #  ApplyImpulseAtOffsetVector : Void

> Applies an impulse at on offset from the center of mass (world space). Results in a change in linear and angular velocity. Will wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |impulse|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |worldOffset|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function ApplyImpulseAtOffsetVector(impulse : Real3, worldOffset : Real3)
> ``` 


---  
 #  ApplyImpulseAtPoint : Void

> Applies an impulse at a world point (world space). Results in a change to linear and angular velocity. Will wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |impulse|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |worldPoint|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function ApplyImpulseAtPoint(impulse : Real3, worldPoint : Real3)
> ``` 


---  
 #  ApplyLinearImpulse : Void

> Applies a linear impulse through the center of mass (world space). Only results in a change of linear velocity. Will wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |linear|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function ApplyLinearImpulse(linear : Real3)
> ``` 


---  
 #  ApplyLinearVelocity : Void

> Adds to the current linear velocity (world space). Will wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |linear|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function ApplyLinearVelocity(linear : Real3)
> ``` 


---  
 #  ApplyTorque : Void

> Applies a torque through the center of mass of the body (world space). Will wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |torque|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function ApplyTorque(torque : Real3)
> ``` 


---  
 #  ApplyTorqueNoWakeUp : Void

> Applies a torque through the center of mass of the body (world space). Will not wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |torque|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function ApplyTorqueNoWakeUp(torque : Real3)
> ``` 


---  
 #  ApplyVelocityAtPoint : Void

> Applies a velocity at a world space point on the object. Results in a change to linear and angular velocity. Will wake up the body if it's asleep.
> |Name|Type|Description|
> |---|---|---|
> |velocity|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |worldPoint|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function ApplyVelocityAtPoint(velocity : Real3, worldPoint : Real3)
> ``` 


---  
 #  ForceAsleep : Void

> Forces the object asleep. Warning: calling this function could create gameplay flaws if used incorrectly, use at your own risk (and sparingly).
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ForceAsleep()
> ``` 


---  
 #  ForceAwake : Void

> Forces the object awake. Will reset the sleep timer.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ForceAwake()
> ``` 


---  
 #  GetPointVelocity : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Computes the linear point velocity of world-space point.
> |Name|Type|Description|
> |---|---|---|
> |worldPoint|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function GetPointVelocity(worldPoint : Real3) : Real3
> ``` 


---  
 #  RigidBody : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function RigidBody()
> ``` 


---  
 

 
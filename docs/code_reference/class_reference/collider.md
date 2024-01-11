 `Component` `Physics`



(NOTE) A collider controls how collision detection is performed for an object. A collider also gives mass properties to a RigidBody(via the material and volume). If there is no RigidBody associated with this collider then it is considered static. Note: colliders without RigidBodies should not be moved at run-time!

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ComputeVolume](collider.md#computevolume-zilch-engin)|[ ActiveBody](collider.md#activebody-zilch-engine-d)|[component](component.md)|[boxcollider](boxcollider.md)|
|[ GetPointVelocity](collider.md#getpointvelocity-zilch-en)|[ CollisionGroup](collider.md#collisiongroup-zilch-engi)| |[capsulecollider](capsulecollider.md)|
| |[ ContactCount](collider.md#contactcount-zilch-engine)| |[convexmeshcollider](convexmeshcollider.md)|
| |[ Contacts](collider.md#contacts-zilch-engine-doc)| |[cylindercollider](cylindercollider.md)|
| |[ Ghost](collider.md#ghost-zilch-engine-docume)| |[ellipsoidcollider](ellipsoidcollider.md)|
| |[ JointCount](collider.md#jointcount-zilch-engine-d)| |[heightmapcollider](heightmapcollider.md)|
| |[ Joints](collider.md#joints-zilch-engine-docum)| |[meshcollider](meshcollider.md)|
| |[ Material](collider.md#material-zilch-engine-doc)| |[multiconvexmeshcollider](multiconvexmeshcollider.md)|
| |[ Offset](collider.md#offset-zilch-engine-docum)| |[spherecollider](spherecollider.md)|
| |[ SendsEvents](collider.md#sendsevents-zilch-engine)| | |
| |[ WorldAabb](collider.md#worldaabb-zilch-engine-do)| | |
| |[ WorldBoundingSphere](collider.md#worldboundingsphere-zero)| | |


 #  Properties


---  
 #  ActiveBody : [rigidbody](rigidbody.md)

 `read-only`

> The rigid body that "owns" this collider. This is the body that forces/impulses/etc... should be applied to.
> ```TS:Nada
> var ActiveBody : RigidBody


---  
 #  CollisionGroup : [collisiongroup](collisiongroup.md)

> The collision group is a tag used to alter collision behavior based upon the space's CollisionTable.
> ```TS:Nada
> var CollisionGroup : CollisionGroup


---  
 #  ContactCount : [integer](../nada_base_types/integer.md)

 `read-only`

> The current number of contacts/collisions with this collider.
> ```TS:Nada
> var ContactCount : Integer


---  
 #  Contacts : [contactrange](contactrange.md)

 `read-only`

> A range of all contacts for this collider.
> ```TS:Nada
> var Contacts : ContactRange


---  
 #  Ghost : [boolean](../nada_base_types/boolean.md)

> Ghosted colliders do not resolve collision. They do still detect collisions and send events. Ghosted colliders are typically used for trigger regions.
> ```TS:Nada
> var Ghost : Boolean


---  
 #  JointCount : [integer](../nada_base_types/integer.md)

 `read-only`

> The number of joints attached to this collider.
> ```TS:Nada
> var JointCount : Integer


---  
 #  Joints : [jointrange](jointrange.md)

 `read-only`

> A range of all joints attached to this collider.
> ```TS:Nada
> var Joints : JointRange


---  
 #  Material : [physicsmaterial](physicsmaterial.md)

> The material used to determine the density, restitution, and friction of this collider.
> ```TS:Nada
> var Material : PhysicsMaterial


---  
 #  Offset : [real3](../nada_base_types/real3.md)

> Moves the physics defined center of the object away from the transform's translation. Used to move physics to match a model.
> ```TS:Nada
> var Offset : Real3


---  
 #  SendsEvents : [boolean](../nada_base_types/boolean.md)

> Determines if this object will send collision events. Used mainly for increasing performance by not sending unnecessary collision events.
> ```TS:Nada
> var SendsEvents : Boolean


---  
 #  WorldAabb : [aabb](aabb.md)

 `read-only`

> Returns the world-space axis aligned bounding box (Aabb) of this collider.
> ```TS:Nada
> var WorldAabb : Aabb


---  
 #  WorldBoundingSphere : [sphere](sphere.md)

 `read-only`

> Returns the world-space bounding sphere of this collider.
> ```TS:Nada
> var WorldBoundingSphere : Sphere


---  
 #  Methods


---  
 #  ComputeVolume : [real](../nada_base_types/real.md)

> Compute the world-space volume of this collider.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ComputeVolume() : Real
> ``` 


---  
 #  GetPointVelocity : [real3](../nada_base_types/real3.md)

> Returns the point velocity of a world-space point with respect to the current rigid body's linear and angular velocity. If there is no rigid body this returns zero.
> |Name|Type|Description|
> |---|---|---|
> |worldPoint|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function GetPointVelocity(worldPoint : Real3) : Real3
> ``` 


---  
 

 
 `Component` `Physics`



(NOTE) A collider controls how collision detection is performed for an object. A collider also gives mass properties to a RigidBody(via the material and volume). If there is no RigidBody associated with this collider then it is considered static. Note: colliders without RigidBodies should not be moved at run-time!

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ComputeVolume](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md#computevolume-zilch-engin)|[ ActiveBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md#activebody-zilch-engine-d)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)|[boxcollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md)|
|[ GetPointVelocity](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md#getpointvelocity-zilch-en)|[ CollisionGroup](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md#collisiongroup-zilch-engi)| |[capsulecollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/capsulecollider.md)|
| |[ ContactCount](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md#contactcount-zilch-engine)| |[convexmeshcollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/convexmeshcollider.md)|
| |[ Contacts](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md#contacts-zilch-engine-doc)| |[cylindercollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cylindercollider.md)|
| |[ Ghost](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md#ghost-zilch-engine-docume)| |[ellipsoidcollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ellipsoidcollider.md)|
| |[ JointCount](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md#jointcount-zilch-engine-d)| |[heightmapcollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/heightmapcollider.md)|
| |[ Joints](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md#joints-zilch-engine-docum)| |[meshcollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/meshcollider.md)|
| |[ Material](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md#material-zilch-engine-doc)| |[multiconvexmeshcollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/multiconvexmeshcollider.md)|
| |[ Offset](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md#offset-zilch-engine-docum)| |[spherecollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spherecollider.md)|
| |[ SendsEvents](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md#sendsevents-zilch-engine)| | |
| |[ WorldAabb](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md#worldaabb-zilch-engine-do)| | |
| |[ WorldBoundingSphere](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md#worldboundingsphere-zero)| | |


 #  Properties


---  
 #  ActiveBody : [rigidbody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)

 `read-only`

> The rigid body that "owns" this collider. This is the body that forces/impulses/etc... should be applied to.
> ``` lang=cpp, name=Nada
> var ActiveBody : RigidBody


---  
 #  CollisionGroup : [collisiongroup](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisiongroup.md)

> The collision group is a tag used to alter collision behavior based upon the space's CollisionTable.
> ``` lang=cpp, name=Nada
> var CollisionGroup : CollisionGroup


---  
 #  ContactCount : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> The current number of contacts/collisions with this collider.
> ``` lang=cpp, name=Nada
> var ContactCount : Integer


---  
 #  Contacts : [contactrange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contactrange.md)

 `read-only`

> A range of all contacts for this collider.
> ``` lang=cpp, name=Nada
> var Contacts : ContactRange


---  
 #  Ghost : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Ghosted colliders do not resolve collision. They do still detect collisions and send events. Ghosted colliders are typically used for trigger regions.
> ``` lang=cpp, name=Nada
> var Ghost : Boolean


---  
 #  JointCount : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> The number of joints attached to this collider.
> ``` lang=cpp, name=Nada
> var JointCount : Integer


---  
 #  Joints : [jointrange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointrange.md)

 `read-only`

> A range of all joints attached to this collider.
> ``` lang=cpp, name=Nada
> var Joints : JointRange


---  
 #  Material : [physicsmaterial](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsmaterial.md)

> The material used to determine the density, restitution, and friction of this collider.
> ``` lang=cpp, name=Nada
> var Material : PhysicsMaterial


---  
 #  Offset : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Moves the physics defined center of the object away from the transform's translation. Used to move physics to match a model.
> ``` lang=cpp, name=Nada
> var Offset : Real3


---  
 #  SendsEvents : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Determines if this object will send collision events. Used mainly for increasing performance by not sending unnecessary collision events.
> ``` lang=cpp, name=Nada
> var SendsEvents : Boolean


---  
 #  WorldAabb : [aabb](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md)

 `read-only`

> Returns the world-space axis aligned bounding box (Aabb) of this collider.
> ``` lang=cpp, name=Nada
> var WorldAabb : Aabb


---  
 #  WorldBoundingSphere : [sphere](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sphere.md)

 `read-only`

> Returns the world-space bounding sphere of this collider.
> ``` lang=cpp, name=Nada
> var WorldBoundingSphere : Sphere


---  
 #  Methods


---  
 #  ComputeVolume : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Compute the world-space volume of this collider.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ComputeVolume() : Real
> ``` 


---  
 #  GetPointVelocity : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Returns the point velocity of a world-space point with respect to the current rigid body's linear and angular velocity. If there is no rigid body this returns zero.
> |Name|Type|Description|
> |---|---|---|
> |worldPoint|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function GetPointVelocity(worldPoint : Real3) : Real3
> ``` 


---  
 

 
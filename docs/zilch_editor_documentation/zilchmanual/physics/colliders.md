The [Collider](../../../code_reference/class_reference/collider.md) component is used to define a shape for collision detection. Together with the [RigidBody](rigidbody.md) component, this creates a game object for physics to move around. There are several pre-defined Collider types, as well as a few customizable types to choose from.
 - [BoxCollider](colliders/boxcollider.md)
 - [SphereCollider](colliders/spherecollider.md)
 - [CylinderCollider](colliders/cylindercollider.md)
 - [EllipsoidCollider](colliders/ellipsoidcollider.md)
 - [CapsuleCollider](colliders/capsulecollider.md)
 - [MeshCollider](colliders/meshcollider.md)
 - [ConvexMeshCollider](colliders/convexmeshcollider.md)
 - [MultiConvexMeshCollider](colliders/multiconvexmeshcollider.md)
 - [HeightMapCollider](colliders/heightmapcollider.md)

 #  The Collider Interface
A Collider is an interface component. This means only derived Collider types can be added to an object, not the base type. The Collider interface allows accessing common properties, such as ghost, between all Colliders without knowing the specific derived type.

 #  Colliders and RigidBodies
Colliders are used in combination with a [RigidBody](rigidbody.md) to give an object mass. The simplest object is one that has both a Collider and a RigidBody. See [Hierarchies](hierarchies.md) for more details. In either case, a Collider exposes the `ActiveBody` property to know what RigidBody a collider should apply forces to.

 #  Physics Material
The [PhysicsMaterial](physicsmaterial.md) on a Collider is used to determine how collision resolution should be handled. Knowing: 

(NOTE) mass = volume * density

the density on the material is used with the Collider's volume (implicit from the shape and size) to contribute mass and inertia to a RigidBody. Additionally the material defines surface properties such as friction and restitution which describe how energy is lost in a collision.

 #  Ghost Colliders
While a collider is often used to define a shape for collision resolution, it is also common to disable collision resolution through the {nav icon=check-square-o, name="Ghost"} property. The ghost property only disables collision resolution while continuing to detect collision. This is useful to create trigger regions where a user can check if something enters or exits an area. Additionally, ghost Colliders are often used to apply forces in an area with the Region component and [PhysicsEffects](physicseffectsandregions.md).

 #  Collision Groups
Sometimes a Collider should only collide with some objects. In this case the ghost property is not sufficient. One of the provided alternatives is to use the {nav icon=wrench, name="CollisionGroup"} property, which defines a group to be used in a CollisionTable. This allows customizing what group pairs go through collision detection and resolution. See [Collision Groups and Collision Tables](collisionoverview/collisiongroupsandtables.md) for more details.

 #  Collision Information
A Collider has two main methods of providing contact information (i.e. what other Colliders are in contact with this one). The most common way to do this is through [Collision Events](collisionoverview/collisionevents.md), which are sent to both objects involved in the contact by default. Additionally, a Collider exposes a range of current contacts to iterate through. In the same way, [Joints](joints.md) can also be iterated through.

---

 ##  Related Materials
 ###  Manual
 - [rigidbody.md](rigidbody.md)
 - [physicsmaterial.md](physicsmaterial.md)
 - [collisiongroupsandtables.md](collisionoverview/collisiongroupsandtables.md)
 - [collisionevents.md](collisionoverview/collisionevents.md)
 - [physicseffectsandregions.md](physicseffectsandregions.md)
 - [hierarchies.md](hierarchies.md)
 - [joints.md](joints.md)

 ###  Reference
 - [Collider](../../../code_reference/class_reference/collider.md)
 - [RigidBody](../../../code_reference/class_reference/rigidbody.md)
 - [PhysicsEffect](../../../code_reference/class_reference/physicseffect.md)
 - [Region](../../../code_reference/class_reference/region.md)
 - [CollisionEvent](../../../code_reference/class_reference/collisionevent.md)
 - [CollisionTable](../../../code_reference/class_reference/collisiontable.md)
 - [CollisionGroup](../../../code_reference/class_reference/collisiongroup.md)
 - [PhysicsMaterial](../../../code_reference/class_reference/physicsmaterial.md)
 - [Joint](../../../code_reference/class_reference/joint.md)
 

 
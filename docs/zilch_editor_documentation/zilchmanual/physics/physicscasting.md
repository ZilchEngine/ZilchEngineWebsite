
 #  PhysicsCasting

One of the most common run-time interactions with a [PhysicsSpace](physicsspace.md) is casting, which queries for all objects within a region of space. This allows common operations such as line-of-sight queries, volume queries, and so on.

Typically a cast will take 3 arguments:
  # The shape to cast
  # How many results to receive at max. This is needed for internal optimizations in physics. For Ray/Segments, the results will be sorted by the t-value.
  # The [CastFilter](../../../code_reference/class_reference/castfilter.md) describes how to filter out results when casting. Common operations include skipping objects of certain configurations (Static, Kinematic, [CollisionGroups](collisionoverview/collisiongroupsandtables.md), etc...).
  
Currently, the physics systems supports a few common casting types:

 ##  Ray Casting
[ray](../../../code_reference/class_reference/ray.md) casting checks for all shapes in a direction. Ray casts are common for things like line-of-sight tests.
 ##  Segment Casting
A [segment](../../../code_reference/class_reference/segment.md) cast is like a ray cast except it has an end position. Segment casts are used when there is a known max distance for the cast.
 ##  Sphere Casting
[sphere](../../../code_reference/class_reference/sphere.md) casting checks to see what objects are within a sphere. Useful for simple volume queries such as finding all objects within an explosion radius.
 ##  Aabb Casting
[aabb](../../../code_reference/class_reference/aabb.md) casting checks what objects are within an axis-aligned box. Sometimes a box is a better shape for casting, especially when the query area is long an thin.
 ##  Frustum Casting
[frustum](../../../code_reference/class_reference/frustum.md) casting checks what objects are within a frustum. Useful for queries that come from a camera where perspective should be taken into account.
 ##  Collider Casting
Sometimes a more complicated shape query is desired. [Collider](../../../code_reference/class_reference/collider.md) casting allows the user to say: "What if this collider was over there". This is commonly used for a simple preventative collision check.

 ##  CastFirst
Ray and Segments have an additional "CastFirst" operation for convenience. These cast functions implicitly have a max object count of `1`.
  
 #  DispatchWithin
In addition to regular casting, the [physicsspace.md](physicsspace.md) contains other common cast related functions. Sometimes casts are performed just to send events to all shapes within a region. This is common for a generic interaction system where each object may or may-not handle some event. Instead of casting and iterating over all results, the PhysicsSpace has the "DispatchWithin" functions. Currently only Sphere and Aabb dispatch functions exist.

 #  Sweeping
While a cast can be used as a preventative check, sometimes the accuracy is not enough. This is where the `SweepCollider` function comes in. Sweeping can be thought of as extending a collider's volume in a direction to find the exact times that a collision would happen with static objects. This allows writing Time-of-Impact logic to avoid missing any collisions.

NOTE: Swept casts are expensive operations and should be used only when important, such as a player.

---
 #  Related Materials
 ##  Manual
- [physicsspace.md](physicsspace.md)
- [colliders.md](colliders.md)
- [collisiongroupsandtables.md](collisionoverview/collisiongroupsandtables.md)
  
 ###  Reference
- [CastFilter](../../../code_reference/class_reference/castfilter.md)
- [CastResult](../../../code_reference/class_reference/castresult.md)
- [SweepResult](../../../code_reference/class_reference/sweepresult.md)
- [Ray](../../../code_reference/class_reference/ray.md)
- [Segment](../../../code_reference/class_reference/segment.md)
- [Aabb](../../../code_reference/class_reference/aabb.md)
- [Sphere](../../../code_reference/class_reference/sphere.md)
- [Frustum](../../../code_reference/class_reference/frustum.md)
- [PhysicsSpace](../../../code_reference/class_reference/physicsspace.md)
- [CollisionGroup](../../../code_reference/class_reference/collisiongroup.md)
- [Collider](../../../code_reference/class_reference/collider.md)
 

 
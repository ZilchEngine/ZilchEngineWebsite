A common issue during development is to have two objects not collide when the user thinks they should. To help aid debugging this, [PhysicsSpace](physicsspace.md) exposes the `WhyAreTheyNotColliding` function. This function takes a pair of objects and returns a string signifying why the physics space doesn't think they're colliding. Here's a short list of a few common reasons:
 - **There isn't a collision**: The objects might just not be colliding. This is often the case when making a 2D game and the objects are on different z-layers. Try to look at the property grid or change the camera angle to verify this.
 - **The collider is static:** See the [Collision Overview](collisionoverview.md) page for what goes through collision detection and collision resolution.
 - **No messages are sent:** Ensure that the Collider's SendsEvent checkBox property is true and that a [CollisionTable](collisionoverview/collisiongroupsandtables.md) is not interfering with these events. Additionally, if using the SweptController make sure:
    - [CustomCollisionEventTracker](../../../../code_reference/class_reference/customcollisioneventtracker.md) component is attached to the same object as the SweptController
    - SweptController's ForwardEvents checkBox property is set to true
 - **The listener didn't connect to the event:** Make sure that the object that is supposed to get a collision event actually connected to the event.
 - **The listener connected incorrectly:** There's two common scenarios for this.
   - 1. Make sure that the correct event type was connected to.
   - 2. Make sure that the listener connected to the right object. Was this the correct cog? Should this have been the PhysicsSpace?

---
 #  Related Materials
 ##  Manual
- [physicstroubleshooting.md](../physicstroubleshooting.md)
- [colliders.md](../colliders.md)
- [collisionoverview.md](../collisionoverview.md)
- [collisiongroupsandtables.md](../collisionoverview/collisiongroupsandtables.md)

 ##  Reference
- [Collider](../../../../code_reference/class_reference/collider.md)
- [PhysicsSpace](../../../../code_reference/class_reference/physicsspace.md)
- [CustomCollisionEventTracker](../../../../code_reference/class_reference/customcollisioneventtracker.md)
- [CollisionGroup](../../../../code_reference/class_reference/collisiongroup.md)
- [CollisionTable](../../../../code_reference/class_reference/collisiontable.md) 

 
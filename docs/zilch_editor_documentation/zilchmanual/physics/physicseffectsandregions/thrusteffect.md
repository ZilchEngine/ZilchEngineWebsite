The [ThrustEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/thrusteffect.md) component applies a directional force at the center of the attached object. Note that this is different than applying the force through the object's center of mass. If the attached object's center differs from the center of mass then this will apply both a linear and angular force. This effect is often used for thrusters on a ship or other point forces that need to apply torque.

 #  Application Methods
The ThrustEffect component expects to be used as a [Collider](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/physicseffectsandregions/colliders.md) or Hierarchy effect. These application methods allow the thrust's center to be defined independently of the center of mass of the [RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/physicseffectsandregions/rigidbody.md) If used as a RigidBody effect then this is no different than [ForceEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/physicseffectsandregions/forceeffect.md). Other application modes are undefined.

---
 #  Related Materials
 ##  Manual
- [physicseffectsandregions.md](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/physicseffectsandregions.md)
- [forceeffect.md](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/physicseffectsandregions/forceeffect.md)
- [rigidbody.md](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/physicseffectsandregions/rigidbody.md)
- [colliders.md](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/physicseffectsandregions/colliders.md)

 ##  Reference
- [ThrustEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/thrusteffect.md)
- [PhysicsEffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicseffect.md) 

 
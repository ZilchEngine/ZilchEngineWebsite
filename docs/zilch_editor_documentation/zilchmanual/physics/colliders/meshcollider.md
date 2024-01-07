(NOTE) **Recommended Reading:** The [Collider](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/colliders.md) page should be read before this page.

[MeshCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/meshcollider.md) defines a surface mesh for world geometry based upon a [PhysicsMesh](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsmesh.md) resource.

WARNING: A future version will likely combine all physics mesh types together.

MeshCollider defines a surface for collision; there are no volume or inertia properties to be computed. This means that a MeshCollider is assumed to be static and should not be used in conjunction with a dynamic [RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/colliders/rigidbody.md) (static is fine). The primary use of MeshCollider is to define static world geometry that is too complicated to represent in a more efficient way for physics.

NOTE: As MeshCollider is assumed to be static, collision detection is not performed between two MeshColliders. 

---
 #  Related Materials
 ##  Manual
- [colliders.md](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/colliders.md)
- [rigidbody.md](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/colliders/rigidbody.md)

 ##  Reference
- [MeshCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/meshcollider.md)
- [Collider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md)
- [RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md) 

 
(NOTE) **Recommended Reading:** The [Collider](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/colliders.md) page should be read before this page.

[HeightMapCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/heightmapcollider.md) defines collision for a [HeightMap](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/heightmap.md). Physics more efficiently represent collision for a HeightMap than a generic mesh.

NOTE: HeightMapCollider is assumed to be static and should not be used with a dynamic [RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/colliders/rigidbody.md).

 #  Thickness
HeightMapCollider exposes the Thickness  property to turn each triangle of the height map into a [prism](https://en.wikipedia.org/wiki/Triangular_prism ). This helps avoid tunneling with fast moving objects.

---
 #  Related Materials
 ##  Manual
 - [colliders.md](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/colliders.md)
 - [rigidbody.md](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/colliders/rigidbody.md)

 ##  Reference
 - [HeightMapCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/heightmapcollider.md)
 - [HeightMap](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/heightmap.md)
 - [RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md) 

 
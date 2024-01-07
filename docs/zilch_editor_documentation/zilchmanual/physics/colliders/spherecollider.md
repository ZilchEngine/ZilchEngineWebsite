[SphereCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spherecollider.md) defines a [sphere](https://en.wikipedia.org/wiki/Sphere ) shape for collision. The size of the sphere is determined byRadius  and the Transform's Scale .

(NOTE) **Recommended Reading:** The [Collider](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/colliders.md) page should be read before this page.

 #  Radius
A SphereCollider exposes the Radius  property which determines the pre-transform radius of the sphere. The SphereCollider will always be a perfect sphere, even when non-uniform scale is present. It does this by taking the largest scale value to determine the radius in world-space.

---
 ##  Related Materials
 ###  Manual
- [colliders.md](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/colliders.md)

 ###  Reference
- [SphereCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spherecollider.md)
- [Collider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md) 

 
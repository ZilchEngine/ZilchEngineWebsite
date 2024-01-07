(NOTE) **Recommended Reading:** The [Collider](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/colliders.md) page should be read before this page.

[ConvexMeshCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/convexmeshcollider.md) defines a [convex hull](https://en.wikipedia.org/wiki/Convex_hull ) for collision detection based upon a [ConvexMesh](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/convexmesh.md) resource.

WARNING: A future version will likely combine all physics mesh types together.

Unlike [MeshCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/colliders/meshcollider.md), convex meshes have a volume which means inertia properties can be computed. ConvexMeshColliders are complex shapes that are still efficient for physics. They are commonly used with dynamic rigid bodies to create an object with a complicated surface.

If a mesh is non-convex, the convex hull of the shape is used for collision detection. This means that the geometry will be an approximation of the surface. 



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/46628.png)


Pictured above is an illustration of the convex hull of an object. Note that the collision is bigger than the original shape.

---

 #  Related Materials
 ##  Manual
- [colliders.md](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/colliders.md)
- [meshcollider.md](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/colliders/meshcollider.md)
 ##  Reference
- [ConvexMeshCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/convexmeshcollider.md)
- [ConvexMesh](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/convexmesh.md)
- [MeshCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/meshcollider.md)
- [Collider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md) 

 
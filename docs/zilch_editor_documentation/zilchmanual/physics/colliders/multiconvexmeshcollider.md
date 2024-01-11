(NOTE) **Recommended Reading:** The [Collider](../colliders.md) page should be read before this page.

[MultiConvexMeshCollider](../../../../code_reference/class_reference/multiconvexmeshcollider.md) defines a collection of [convex hulls](https://en.wikipedia.org/wiki/Convex_hull ) for collision detection based upon a [MultiConvexMesh](../../../../code_reference/class_reference/multiconvexmesh.md) resource.

WARNING: A future version will likely combine all physics mesh types together.

MultiConvexMeshCollider allows more complicated shapes to be represented than a [ConvexMeshCollider](convexmeshcollider.md) while still retaining performance. Physics needs convex shapes for efficiency so this Collider represents non-convex shapes as a collection of sub convex meshes.

Currently, the editor for this mesh type only works for 2D shapes (sprites). 3D meshes can be made, but only through script. Future plans include implementing 3D approximate convex decomposition.

 #  Troubleshooting
As the MultiConvexMeshCollider contains multiple convex pieces, seams can exist between the pieces. This can cause [edge catching](physicstroubleshooting/edgecatching.md) issues when objects slide across the surface. Additionally, an object can get sandwiched in the interior between two sub-meshes.

---

 #  Related Materials
 ##  Manual
- [colliders.md](../colliders.md)
- [convexmeshcollider.md](convexmeshcollider.md)
- [edgecatching.md](physicstroubleshooting/edgecatching.md)
 ##  Reference
- [MultiConvexMeshCollider](../../../../code_reference/class_reference/multiconvexmeshcollider.md)
- [MultiConvexMesh](../../../../code_reference/class_reference/multiconvexmesh.md)
- [ConvexMeshCollider](../../../../code_reference/class_reference/convexmeshcollider.md)
- [Collider](../../../../code_reference/class_reference/collider.md) 

 
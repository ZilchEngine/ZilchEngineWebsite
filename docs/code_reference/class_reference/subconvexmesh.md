 `Physics`



(NOTE) Contains the indices of a convex mesh. The triangle indices are the primary method to configure this (required for mass computations). The regular indices are used for debug drawing and to reduce intersection tests by removing duplicate points. If left empty, Indices will be auto-filled from the triangle indices.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[Indices](subconvexmesh.md#indices-zilch-engine-docu)|[safeid32object](safeid32object.md)| |
| |[Mesh](subconvexmesh.md#mesh-zilch-engine-documen)| | |
| |[TriangleIndices](subconvexmesh.md#triangleindices-zilch-eng)| | |
| |[Valid](subconvexmesh.md#valid-zilch-engine-docume)| | |


 #  Properties


---  
 #  Indices : [multiconvexmeshindexdata](multiconvexmeshindexdata.md)

 `read-only`

> The vertex indices on the main mesh used to generate the convex hull.
> ```TS:Nada
> var Indices : MultiConvexMeshIndexData


---  
 #  Mesh : [multiconvexmesh](multiconvexmesh.md)

> The MultiConvexMesh that owns this sub-mesh.
> ```TS:Nada
> var Mesh : MultiConvexMesh


---  
 #  TriangleIndices : [multiconvexmeshindexdata](multiconvexmeshindexdata.md)

 `read-only`

> The vertex indices on the main mesh used to generate triangle indices for computing mass information and debug drawing. More indices are needed for determining triangles than for generating the convex mesh.
> ```TS:Nada
> var TriangleIndices : MultiConvexMeshIndexData


---  
 #  Valid : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Is this sub-mesh incorrectly configured. Typically means that the indices don't point to valid vertices. Also the number of triangle indices could be incorrect (multiple of 3).
> ```TS:Nada
> var Valid : Boolean


---  
 #  Methods


---  
 

 
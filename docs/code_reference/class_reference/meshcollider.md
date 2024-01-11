 `Component` `Physics`



(NOTE) Defines the collision for a generic mesh from a collection of triangles ( PhysicsMesh resource). This collider type is not expected to have a dynamic or kinematic RigidBody.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](meshcollider.md#meshcollider-void)|[ DrawEdges](meshcollider.md#drawedges-zilch-engine-do)|[collider](collider.md)| |
| |[ DrawFaceNormals](meshcollider.md#drawfacenormals-zilch-eng)| | |
| |[ DrawFaces](meshcollider.md#drawfaces-zilch-engine-do)| | |
| |[ PhysicsMesh](meshcollider.md#physicsmesh-zilch-engine)| | |


 #  Properties


---  
 #  DrawEdges : [boolean](../nada_base_types/boolean.md)

> Whether to debug draw the edges of each triangle.
> ``` lang=cpp, name=Nada
> var DrawEdges : Boolean


---  
 #  DrawFaceNormals : [boolean](../nada_base_types/boolean.md)

> Whether to debug draw the normals of each triangle.
> ``` lang=cpp, name=Nada
> var DrawFaceNormals : Boolean


---  
 #  DrawFaces : [boolean](../nada_base_types/boolean.md)

> Whether to debug draw the faces of each triangle.
> ``` lang=cpp, name=Nada
> var DrawFaces : Boolean


---  
 #  PhysicsMesh : [physicsmesh](physicsmesh.md)

> The mesh resource used to define collision. This mesh is just a surface mesh of triangles (no volume is defined).
> ``` lang=cpp, name=Nada
> var PhysicsMesh : PhysicsMesh


---  
 #  Methods


---  
 #  MeshCollider : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function MeshCollider()
> ``` 


---  
 

 
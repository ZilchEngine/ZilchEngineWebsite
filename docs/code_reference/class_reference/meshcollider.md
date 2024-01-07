 `Component` `Physics`



(NOTE) Defines the collision for a generic mesh from a collection of triangles ( PhysicsMesh resource). This collider type is not expected to have a dynamic or kinematic RigidBody.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/meshcollider.md#meshcollider-void)|[ DrawEdges](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/meshcollider.md#drawedges-zilch-engine-do)|[collider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md)| |
| |[ DrawFaceNormals](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/meshcollider.md#drawfacenormals-zilch-eng)| | |
| |[ DrawFaces](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/meshcollider.md#drawfaces-zilch-engine-do)| | |
| |[ PhysicsMesh](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/meshcollider.md#physicsmesh-zilch-engine)| | |


 #  Properties


---  
 #  DrawEdges : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Whether to debug draw the edges of each triangle.
> ``` lang=cpp, name=Nada
> var DrawEdges : Boolean


---  
 #  DrawFaceNormals : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Whether to debug draw the normals of each triangle.
> ``` lang=cpp, name=Nada
> var DrawFaceNormals : Boolean


---  
 #  DrawFaces : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Whether to debug draw the faces of each triangle.
> ``` lang=cpp, name=Nada
> var DrawFaces : Boolean


---  
 #  PhysicsMesh : [physicsmesh](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsmesh.md)

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
 

 
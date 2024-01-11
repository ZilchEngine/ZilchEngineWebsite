 `Resource` `Physics`



(NOTE) Represents a collection of convex meshes that was decomposed from a mesh.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ CreateRuntime](multiconvexmesh.md#createruntime-zilch-engin)|[ Modified](multiconvexmesh.md#modified-zilch-engine-doc)|Resource| |
|[ RuntimeClone](multiconvexmesh.md#runtimeclone-zilch-engine)|[ SubMeshes](multiconvexmesh.md#submeshes-zilch-engine-do)| | |
|[ UpdateAndNotifyIfModified](multiconvexmesh.md#updateandnotifyifmodifie)|[ Valid](multiconvexmesh.md#valid-zilch-engine-docume)| | |
|[ Validate](multiconvexmesh.md#validate-zilch-engine-doc)|[ Vertices](multiconvexmesh.md#vertices-zilch-engine-doc)| | |


 #  Properties


---  
 #  Modified : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Is the resource currently modified?
> ``` lang=cpp, name=Nada
> var Modified : Boolean


---  
 #  SubMeshes : [multiconvexmeshsubmeshdata](multiconvexmeshsubmeshdata.md)

 `read-only`

> A collection of sub-convex meshes.
> ``` lang=cpp, name=Nada
> var SubMeshes : MultiConvexMeshSubMeshData


---  
 #  Valid : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Is the resource correctly setup? Typically involves a mis-match in indices and vertices.
> ``` lang=cpp, name=Nada
> var Valid : Boolean


---  
 #  Vertices : [multiconvexmeshvertexdata](multiconvexmeshvertexdata.md)

 `read-only`

> The vertex buffer data of this mesh.
> ``` lang=cpp, name=Nada
> var Vertices : MultiConvexMeshVertexData


---  
 #  Methods


---  
 #  CreateRuntime : [multiconvexmesh](multiconvexmesh.md)

 `static`

> Creates a MultiConvexMesh for run-time modifications.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function CreateRuntime() : MultiConvexMesh
> ``` 


---  
 #  RuntimeClone : [multiconvexmesh](multiconvexmesh.md)

> Creates a clone of this mesh for run-time modifications.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function RuntimeClone() : MultiConvexMesh
> ``` 


---  
 #  UpdateAndNotifyIfModified : Void

> Rebuild all extra mesh information if it is currently modified. This includes things like the center of mass, volume, aabb, edge info and more.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function UpdateAndNotifyIfModified()
> ``` 


---  
 #  Validate : [boolean](../nada_base_types/boolean.md)

> Check if the mesh is valid. Optionally throw a script exception if it is invalid.
> |Name|Type|Description|
> |---|---|---|
> |throwExceptionIfInvalid|[boolean](../nada_base_types/boolean.md)| |
> ``` lang=cpp, name=Nada
> function Validate(throwExceptionIfInvalid : Boolean) : Boolean
> ``` 


---  
 

 
 `Resource` `Physics`



(NOTE) Base class of mesh type physics resources. Stores the actual mesh (no optimization structures) and information about the mesh such as mass and inertia.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ UpdateAndNotifyIfModified](genericphysicsmesh.md#updateandnotifyifmodifie)|[ Indices](genericphysicsmesh.md#indices-zilch-engine-docu)|Resource|[convexmesh](convexmesh.md)|
|[ Validate](genericphysicsmesh.md#validate-zilch-engine-doc)|[ Vertices](genericphysicsmesh.md#vertices-zilch-engine-doc)| |[physicsmesh](physicsmesh.md)|


 #  Properties


---  
 #  Indices : [physicsmeshindexdata](physicsmeshindexdata.md)

 `read-only`

> The index buffer data of this mesh.
> ``` lang=cpp, name=Nada
> var Indices : PhysicsMeshIndexData


---  
 #  Vertices : [physicsmeshvertexdata](physicsmeshvertexdata.md)

 `read-only`

> The vertex buffer data of this mesh.
> ``` lang=cpp, name=Nada
> var Vertices : PhysicsMeshVertexData


---  
 #  Methods


---  
 #  UpdateAndNotifyIfModified : Void

> Rebuild all extra mesh information if it is currently modified. This includes things like the center of mass, volume, aabb, edge info and more (some derived types may have a mid-phase, etc...)
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
 

 
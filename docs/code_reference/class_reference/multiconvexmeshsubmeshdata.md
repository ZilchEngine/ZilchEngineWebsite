 `Physics`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Add](multiconvexmeshsubmeshdata.md#add-zilch-engine-document)|[ All](multiconvexmeshsubmeshdata.md#all-zilch-engine-document)|[safeid32object](safeid32object.md)| |
|[ Clear](multiconvexmeshsubmeshdata.md#clear-void)|[ Count](multiconvexmeshsubmeshdata.md#count-zilch-engine-docume)| | |
|[ Get](multiconvexmeshsubmeshdata.md#get-zilch-engine-document)| | | |
|[ RemoveAt](multiconvexmeshsubmeshdata.md#removeat-void)| | | |


 #  Properties


---  
 #  All : [multiconvexmeshsubmeshrange](multiconvexmeshsubmeshrange.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var All : MultiConvexMeshSubMeshRange


---  
 #  Count : [integer](../nada_base_types/integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Count : Integer


---  
 #  Methods


---  
 #  Add : [subconvexmesh](subconvexmesh.md)

> Create and add a new SubConvexMesh. Returns the new mesh for modification.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Add() : SubConvexMesh
> ``` 


---  
 #  Clear : Void

> Clears all sub-meshes.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Clear()
> ``` 


---  
 #  Get : [subconvexmesh](subconvexmesh.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ||[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Get( : Integer) : SubConvexMesh
> ``` 


---  
 #  RemoveAt : Void

> Remove the sub-mesh at the given index.
> |Name|Type|Description|
> |---|---|---|
> |arrayIndex|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function RemoveAt(arrayIndex : Integer)
> ``` 


---  
 

 
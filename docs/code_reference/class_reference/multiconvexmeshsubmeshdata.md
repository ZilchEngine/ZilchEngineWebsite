 `Physics`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Add](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/multiconvexmeshsubmeshdata.md#add-zilch-engine-document)|[ All](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/multiconvexmeshsubmeshdata.md#all-zilch-engine-document)|[safeid32object](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/safeid32object.md)| |
|[ Clear](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/multiconvexmeshsubmeshdata.md#clear-void)|[ Count](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/multiconvexmeshsubmeshdata.md#count-zilch-engine-docume)| | |
|[ Get](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/multiconvexmeshsubmeshdata.md#get-zilch-engine-document)| | | |
|[ RemoveAt](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/multiconvexmeshsubmeshdata.md#removeat-void)| | | |


 #  Properties


---  
 #  All : [multiconvexmeshsubmeshrange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/multiconvexmeshsubmeshrange.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var All : MultiConvexMeshSubMeshRange


---  
 #  Count : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Count : Integer


---  
 #  Methods


---  
 #  Add : [subconvexmesh](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/subconvexmesh.md)

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
 #  Get : [subconvexmesh](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/subconvexmesh.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ||[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Get( : Integer) : SubConvexMesh
> ``` 


---  
 #  RemoveAt : Void

> Remove the sub-mesh at the given index.
> |Name|Type|Description|
> |---|---|---|
> |arrayIndex|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function RemoveAt(arrayIndex : Integer)
> ``` 


---  
 

 
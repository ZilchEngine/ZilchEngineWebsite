 `Resource` `Graphics`



(NOTE) Data that represents a mesh in the way that is intended to be used by graphics hardware.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ CreateRuntime](mesh.md#createruntime-zilch-engin)|[ Indices](mesh.md#indices-zilch-engine-docu)|Resource| |
|[ RuntimeClone](mesh.md#runtimeclone-zilch-engine)|[ PrimitiveType](mesh.md#primitivetype-zilch-engin)| | |
|[ Upload](mesh.md#upload-void)|[ Vertices](mesh.md#vertices-zilch-engine-doc)| | |
|[ UploadNoRayCastInfo](mesh.md#uploadnoraycastinfo-void)| | | |
|[ UploadNoRayCastInfoOrAabb](mesh.md#uploadnoraycastinfooraab)| | | |


 #  Properties


---  
 #  Indices : [indexbuffer](indexbuffer.md)

 `read-only`

> Indices used to define non-sequential primitive construction from vertices, such as shared vertices.
> ```TS:Nada
> var Indices : IndexBuffer


---  
 #  PrimitiveType : [PrimitiveType](../enum_reference.md#primitivetype)

> The type of primitives to be made with the vertex data.
> ```TS:Nada
> var PrimitiveType : PrimitiveType


---  
 #  Vertices : [vertexbuffer](vertexbuffer.md)

 `read-only`

> Vertex data and attribute semantics for defining data that can be uploaded to the gpu.
> ```TS:Nada
> var Vertices : VertexBuffer


---  
 #  Methods


---  
 #  CreateRuntime : [mesh](mesh.md)

 `static`

> Makes an anonymous Mesh resource that can be defined by script and uploaded to the gpu.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function CreateRuntime() : Mesh
> ``` 


---  
 #  RuntimeClone : [mesh](mesh.md)

> Creates a clone of this Mesh. As a clone is expected to be modified, an upload function must be called before this mesh can be used.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function RuntimeClone() : Mesh
> ``` 


---  
 #  Upload : Void

> Upload vertex buffer and index buffer data to the gpu. This will also build the aabb and information needed for raycasting.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Upload()
> ``` 


---  
 #  UploadNoRayCastInfo : Void

> Same as Upload except raycasting information will not be built. This avoids a possible spike when a custom mesh will never need to be raycasted against.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function UploadNoRayCastInfo()
> ``` 


---  
 #  UploadNoRayCastInfoOrAabb : Void

> Same as Upload except raycasting information and the aabb will not be built. This should be used when the user is manually setting an aabb or frustum culling is disabled.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function UploadNoRayCastInfoOrAabb()
> ``` 


---  
 

 
 `Resource` `Graphics`



(NOTE) Data that represents a mesh in the way that is intended to be used by graphics hardware.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ CreateRuntime](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mesh.md#createruntime-zilch-engin)|[ Indices](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mesh.md#indices-zilch-engine-docu)|Resource| |
|[ RuntimeClone](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mesh.md#runtimeclone-zilch-engine)|[ PrimitiveType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mesh.md#primitivetype-zilch-engin)| | |
|[ Upload](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mesh.md#upload-void)|[ Vertices](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mesh.md#vertices-zilch-engine-doc)| | |
|[ UploadNoRayCastInfo](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mesh.md#uploadnoraycastinfo-void)| | | |
|[ UploadNoRayCastInfoOrAabb](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mesh.md#uploadnoraycastinfooraab)| | | |


 #  Properties


---  
 #  Indices : [indexbuffer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/indexbuffer.md)

 `read-only`

> Indices used to define non-sequential primitive construction from vertices, such as shared vertices.
> ``` lang=cpp, name=Nada
> var Indices : IndexBuffer


---  
 #  PrimitiveType : [PrimitiveType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#primitivetype)

> The type of primitives to be made with the vertex data.
> ``` lang=cpp, name=Nada
> var PrimitiveType : PrimitiveType


---  
 #  Vertices : [vertexbuffer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/vertexbuffer.md)

 `read-only`

> Vertex data and attribute semantics for defining data that can be uploaded to the gpu.
> ``` lang=cpp, name=Nada
> var Vertices : VertexBuffer


---  
 #  Methods


---  
 #  CreateRuntime : [mesh](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mesh.md)

 `static`

> Makes an anonymous Mesh resource that can be defined by script and uploaded to the gpu.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function CreateRuntime() : Mesh
> ``` 


---  
 #  RuntimeClone : [mesh](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mesh.md)

> Creates a clone of this Mesh. As a clone is expected to be modified, an upload function must be called before this mesh can be used.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function RuntimeClone() : Mesh
> ``` 


---  
 #  Upload : Void

> Upload vertex buffer and index buffer data to the gpu. This will also build the aabb and information needed for raycasting.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Upload()
> ``` 


---  
 #  UploadNoRayCastInfo : Void

> Same as Upload except raycasting information will not be built. This avoids a possible spike when a custom mesh will never need to be raycasted against.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function UploadNoRayCastInfo()
> ``` 


---  
 #  UploadNoRayCastInfoOrAabb : Void

> Same as Upload except raycasting information and the aabb will not be built. This should be used when the user is manually setting an aabb or frustum culling is disabled.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function UploadNoRayCastInfoOrAabb()
> ``` 


---  
 

 
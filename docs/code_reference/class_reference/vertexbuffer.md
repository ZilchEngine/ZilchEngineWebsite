 `Graphics`

(NOTE) Vertex data and attribute semantics for defining data that can be uploaded to the gpu.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddAttribute](vertexbuffer.md#addattribute-void)|[ VertexCount](vertexbuffer.md#vertexcount-zilch-engine)|[safeid32](safeid32.md)| |
|[ AddByte](vertexbuffer.md#addbyte-void)| | | |
|[ AddReal](vertexbuffer.md#addreal-void)| | | |
|[ AddShort](vertexbuffer.md#addshort-void)| | | |
|[ ClearAttributes](vertexbuffer.md#clearattributes-void)| | | |
|[ ClearData](vertexbuffer.md#cleardata-void)| | | |
|[ GetAttributes](vertexbuffer.md#getattributes-zilch-engin)| | | |
|[ GetElementCount](vertexbuffer.md#getelementcount-zilch-eng)| | | |
|[ GetElementType](vertexbuffer.md#getelementtype-zilch-engi)| | | |
|[ GetVertexData](vertexbuffer.md#getvertexdata-zilch-engin)| | | |
|[ IsValidVertexData](vertexbuffer.md#isvalidvertexdata-zilch-e)| | | |


 #  Properties


---  
 #  VertexCount : [integer](../nada_base_types/integer.md)

 `read-only`

> Returns the number of vertices that have a complete set of data stored.
> ``` lang=cpp, name=Nada
> var VertexCount : Integer


---  
 #  Methods


---  
 #  AddAttribute : Void

> Adds an attribute to the definition of the vertices that are to be stored. Add the attributes in the order that they should be stored in memory on a vertex.
> |Name|Type|Description|
> |---|---|---|
> |semantic|[VertexSemantic](../enum_reference.md#vertexsemantic)| |
> |elementType|[VertexElementType](../enum_reference.md#vertexelementtype)| |
> |elementCount|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function AddAttribute(semantic : VertexSemantic, elementType : VertexElementType, elementCount : Integer)
> ``` 


---  
 #  AddByte : Void

> Adds data as bytes to the buffer, data is expected in the order of the attributes, one vertex after another.
> |Name|Type|Description|
> |---|---|---|
> |value|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function AddByte(value : Integer)
> ``` 


---  
 #  AddByte : Void

> Adds data as bytes to the buffer, data is expected in the order of the attributes, one vertex after another.
> |Name|Type|Description|
> |---|---|---|
> ||[integer2](../nada_base_types/integer2.md)| |
> ``` lang=cpp, name=Nada
> function AddByte( : Integer2)
> ``` 


---  
 #  AddByte : Void

> Adds data as bytes to the buffer, data is expected in the order of the attributes, one vertex after another.
> |Name|Type|Description|
> |---|---|---|
> ||[integer3](../nada_base_types/integer3.md)| |
> ``` lang=cpp, name=Nada
> function AddByte( : Integer3)
> ``` 


---  
 #  AddByte : Void

> Adds data as bytes to the buffer, data is expected in the order of the attributes, one vertex after another.
> |Name|Type|Description|
> |---|---|---|
> ||[integer4](../nada_base_types/integer4.md)| |
> ``` lang=cpp, name=Nada
> function AddByte( : Integer4)
> ``` 


---  
 #  AddReal : Void

> Adds data as floats to the buffer, data is expected in the order of the attributes, one vertex after another.
> |Name|Type|Description|
> |---|---|---|
> |value|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function AddReal(value : Real)
> ``` 


---  
 #  AddReal : Void

> Adds data as floats to the buffer, data is expected in the order of the attributes, one vertex after another.
> |Name|Type|Description|
> |---|---|---|
> |value|[real2](../nada_base_types/real2.md)| |
> ``` lang=cpp, name=Nada
> function AddReal(value : Real2)
> ``` 


---  
 #  AddReal : Void

> Adds data as floats to the buffer, data is expected in the order of the attributes, one vertex after another.
> |Name|Type|Description|
> |---|---|---|
> |value|[real3](../nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function AddReal(value : Real3)
> ``` 


---  
 #  AddReal : Void

> Adds data as floats to the buffer, data is expected in the order of the attributes, one vertex after another.
> |Name|Type|Description|
> |---|---|---|
> |value|[real4](../nada_base_types/real4.md)| |
> ``` lang=cpp, name=Nada
> function AddReal(value : Real4)
> ``` 


---  
 #  AddShort : Void

> Adds data as shorts to the buffer, data is expected in the order of the attributes, one vertex after another.
> |Name|Type|Description|
> |---|---|---|
> |value|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function AddShort(value : Integer)
> ``` 


---  
 #  AddShort : Void

> Adds data as shorts to the buffer, data is expected in the order of the attributes, one vertex after another.
> |Name|Type|Description|
> |---|---|---|
> ||[integer2](../nada_base_types/integer2.md)| |
> ``` lang=cpp, name=Nada
> function AddShort( : Integer2)
> ``` 


---  
 #  AddShort : Void

> Adds data as shorts to the buffer, data is expected in the order of the attributes, one vertex after another.
> |Name|Type|Description|
> |---|---|---|
> ||[integer3](../nada_base_types/integer3.md)| |
> ``` lang=cpp, name=Nada
> function AddShort( : Integer3)
> ``` 


---  
 #  AddShort : Void

> Adds data as shorts to the buffer, data is expected in the order of the attributes, one vertex after another.
> |Name|Type|Description|
> |---|---|---|
> ||[integer4](../nada_base_types/integer4.md)| |
> ``` lang=cpp, name=Nada
> function AddShort( : Integer4)
> ``` 


---  
 #  ClearAttributes : Void

> Clears all added attributes from the vertex definition so they can be redefined.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ClearAttributes()
> ``` 


---  
 #  ClearData : Void

> Clears all added vertex data so new data can be added.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ClearData()
> ``` 


---  
 #  GetAttributes : [vertexsemanticrange](vertexsemanticrange.md)

> Returns a range of attribute semantics in the order that they were added.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function GetAttributes() : VertexSemanticRange
> ``` 


---  
 #  GetElementCount : [integer](../nada_base_types/integer.md)

> Returns the number of elements stored for the given attribute, throws exception if the attribute is not in the vertex definition.
> |Name|Type|Description|
> |---|---|---|
> |semantic|[VertexSemantic](../enum_reference.md#vertexsemantic)| |
> ``` lang=cpp, name=Nada
> function GetElementCount(semantic : VertexSemantic) : Integer
> ``` 


---  
 #  GetElementType : [VertexElementType](../enum_reference.md#vertexelementtype)

> Returns the type that is used to store the given attribute, throws exception if the attribute is not in the vertex definition.
> |Name|Type|Description|
> |---|---|---|
> |semantic|[VertexSemantic](../enum_reference.md#vertexsemantic)| |
> ``` lang=cpp, name=Nada
> function GetElementType(semantic : VertexSemantic) : VertexElementType
> ``` 


---  
 #  GetVertexData : [real4](../nada_base_types/real4.md)

> Gets the data of an attribute of a vertex, returns values of 0 if read is invalid.
> |Name|Type|Description|
> |---|---|---|
> |vertexIndex|[integer](../nada_base_types/integer.md)| |
> |semantic|[VertexSemantic](../enum_reference.md#vertexsemantic)| |
> ``` lang=cpp, name=Nada
> function GetVertexData(vertexIndex : Integer, semantic : VertexSemantic) : Real4
> ``` 


---  
 #  GetVertexData : [real4](../nada_base_types/real4.md)

> Gets the data of an attribute of a vertex, throws exception if attribute info doesn't match or read is invalid.
> |Name|Type|Description|
> |---|---|---|
> |vertexIndex|[integer](../nada_base_types/integer.md)| |
> |semantic|[VertexSemantic](../enum_reference.md#vertexsemantic)| |
> |type|[VertexElementType](../enum_reference.md#vertexelementtype)| |
> |count|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function GetVertexData(vertexIndex : Integer, semantic : VertexSemantic, type : VertexElementType, count : Integer) : Real4
> ``` 


---  
 #  IsValidVertexData : [boolean](../nada_base_types/boolean.md)

> Returns false if GetVertexData() would throw an exception with the same arguments.
> |Name|Type|Description|
> |---|---|---|
> |vertexIndex|[integer](../nada_base_types/integer.md)| |
> |semantic|[VertexSemantic](../enum_reference.md#vertexsemantic)| |
> |type|[VertexElementType](../enum_reference.md#vertexelementtype)| |
> |count|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function IsValidVertexData(vertexIndex : Integer, semantic : VertexSemantic, type : VertexElementType, count : Integer) : Boolean
> ``` 


---  
 

 
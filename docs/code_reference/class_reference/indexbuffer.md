 `Graphics`

(NOTE) Indices used to define non-sequential primitive construction from vertices, such as shared vertices.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Add](indexbuffer.md#add-void)|[Count](indexbuffer.md#count-zilch-engine-docume)|[safeid32](safeid32.md)| |
|[Clear](indexbuffer.md#clear-void)| | | |
|[Get](indexbuffer.md#get-zilch-engine-document)| | | |


 #  Properties


---  
 #  Count : [integer](../nada_base_types/integer.md)

> Number of vertex indices currently in buffer. Can be set manually to invoke vertex shading that number of times, with or without vertex data.
> ```TS:Nada
> var Count : Integer


---  
 #  Methods


---  
 #  Add : Void

> Add a vertex index to the buffer.
> |Name|Type|Description|
> |---|---|---|
> |value|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function Add(value : Integer)
> ``` 


---  
 #  Clear : Void

> Clears all stored indices so that new ones can be added.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Clear()
> ``` 


---  
 #  Get : [integer](../nada_base_types/integer.md)

> Returns the vertex index that is stored at the given index of this buffer.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function Get(index : Integer) : Integer
> ``` 


---  
 

 
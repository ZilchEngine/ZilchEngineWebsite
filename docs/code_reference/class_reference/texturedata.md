 `Graphics`

(NOTE) Modifiable texture data that can be used to upload to a runtime Texture resource. All formats use one interface for get/set, all values are converted to/from floats and unused channels are ignored. Integer formats are represented in the normalized range [0, 1].

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Get](texturedata.md#get-zilch-engine-document)|[Format](texturedata.md#format-zilch-engine-docum)| | |
|[Set](texturedata.md#set-void)|[Height](texturedata.md#height-zilch-engine-docum)| | |
|[Constructor](texturedata.md#texturedata-void)|[PixelCount](texturedata.md#pixelcount-zilch-engine-d)| | |
| |[Width](texturedata.md#width-zilch-engine-docume)| | |


 #  Properties


---  
 #  Format : [TextureFormat](../enum_reference.md#textureformat)

 `read-only`

> Memory format of the stored pixel data.
> ```TS:Nada
> var Format : TextureFormat


---  
 #  Height : [integer](../nada_base_types/integer.md)

 `read-only`

> Height of the texture data in pixels.
> ```TS:Nada
> var Height : Integer


---  
 #  PixelCount : [integer](../nada_base_types/integer.md)

 `read-only`

> Total number of pixels in texture data.
> ```TS:Nada
> var PixelCount : Integer


---  
 #  Width : [integer](../nada_base_types/integer.md)

 `read-only`

> Width of the texture data in pixels.
> ```TS:Nada
> var Width : Integer


---  
 #  Methods


---  
 #  Get : [real4](../nada_base_types/real4.md)

> Returns the pixel values at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function Get(index : Integer) : Real4
> ``` 


---  
 #  Get : [real4](../nada_base_types/real4.md)

> Returns the pixel values at the given index.
> |Name|Type|Description|
> |---|---|---|
> |x|[integer](../nada_base_types/integer.md)| |
> |y|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function Get(x : Integer, y : Integer) : Real4
> ``` 


---  
 #  Set : Void

> Sets the pixel values at the given index.
> |Name|Type|Description|
> |---|---|---|
> |x|[integer](../nada_base_types/integer.md)| |
> |y|[integer](../nada_base_types/integer.md)| |
> |value|[real4](../nada_base_types/real4.md)| |
> ```TS:Nada
> function Set(x : Integer, y : Integer, value : Real4)
> ``` 


---  
 #  Set : Void

> Sets the pixel values at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> |value|[real4](../nada_base_types/real4.md)| |
> ```TS:Nada
> function Set(index : Integer, value : Real4)
> ``` 


---  
 #  TextureData : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |format|[TextureFormat](../enum_reference.md#textureformat)| |
> |width|[integer](../nada_base_types/integer.md)| |
> |height|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function TextureData(format : TextureFormat, width : Integer, height : Integer)
> ``` 


---  
 

 
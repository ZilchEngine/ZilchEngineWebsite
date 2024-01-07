 `Graphics`

(NOTE) Modifiable texture data that can be used to upload to a runtime Texture resource. All formats use one interface for get/set, all values are converted to/from floats and unused channels are ignored. Integer formats are represented in the normalized range [0, 1].

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Get](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/texturedata.md#get-zilch-engine-document)|[ Format](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/texturedata.md#format-zilch-engine-docum)| | |
|[ Set](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/texturedata.md#set-void)|[ Height](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/texturedata.md#height-zilch-engine-docum)| | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/texturedata.md#texturedata-void)|[ PixelCount](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/texturedata.md#pixelcount-zilch-engine-d)| | |
| |[ Width](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/texturedata.md#width-zilch-engine-docume)| | |


 #  Properties


---  
 #  Format : [TextureFormat](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#textureformat)

 `read-only`

> Memory format of the stored pixel data.
> ``` lang=cpp, name=Nada
> var Format : TextureFormat


---  
 #  Height : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Height of the texture data in pixels.
> ``` lang=cpp, name=Nada
> var Height : Integer


---  
 #  PixelCount : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Total number of pixels in texture data.
> ``` lang=cpp, name=Nada
> var PixelCount : Integer


---  
 #  Width : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Width of the texture data in pixels.
> ``` lang=cpp, name=Nada
> var Width : Integer


---  
 #  Methods


---  
 #  Get : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

> Returns the pixel values at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Get(index : Integer) : Real4
> ``` 


---  
 #  Get : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

> Returns the pixel values at the given index.
> |Name|Type|Description|
> |---|---|---|
> |x|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |y|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Get(x : Integer, y : Integer) : Real4
> ``` 


---  
 #  Set : Void

> Sets the pixel values at the given index.
> |Name|Type|Description|
> |---|---|---|
> |x|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |y|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |value|[real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)| |
> ``` lang=cpp, name=Nada
> function Set(x : Integer, y : Integer, value : Real4)
> ``` 


---  
 #  Set : Void

> Sets the pixel values at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |value|[real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)| |
> ``` lang=cpp, name=Nada
> function Set(index : Integer, value : Real4)
> ``` 


---  
 #  TextureData : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |format|[TextureFormat](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#textureformat)| |
> |width|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |height|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function TextureData(format : TextureFormat, width : Integer, height : Integer)
> ``` 


---  
 

 
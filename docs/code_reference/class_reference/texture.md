 `Resource` `Graphics`



(NOTE) Data that represents a texture in the way that is intended to be used by graphics hardware.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ CreateRuntime](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/texture.md#createruntime-zilch-engin)|[ AddressingX](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/texture.md#addressingx-zilch-engine)|Resource| |
|[ SubUpload](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/texture.md#subupload-void)|[ AddressingY](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/texture.md#addressingy-zilch-engine)| | |
|[ Upload](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/texture.md#upload-void)|[ Anisotropy](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/texture.md#anisotropy-zilch-engine-d)| | |
| |[ CompareFunc](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/texture.md#comparefunc-zilch-engine)| | |
| |[ CompareMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/texture.md#comparemode-zilch-engine)| | |
| |[ Compression](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/texture.md#compression-zilch-engine)| | |
| |[ Filtering](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/texture.md#filtering-zilch-engine-do)| | |
| |[ Format](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/texture.md#format-zilch-engine-docum)| | |
| |[ Height](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/texture.md#height-zilch-engine-docum)| | |
| |[ MipMapping](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/texture.md#mipmapping-zilch-engine-d)| | |
| |[ Size](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/texture.md#size-zilch-engine-documen)| | |
| |[ Type](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/texture.md#type-zilch-engine-documen)| | |
| |[ Width](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/texture.md#width-zilch-engine-docume)| | |


 #  Properties


---  
 #  AddressingX : [TextureAddressing](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#textureaddressing)

> How to treat uv coordinates outside of [0, 1] along the Texture's width.
> ``` lang=cpp, name=Nada
> var AddressingX : TextureAddressing


---  
 #  AddressingY : [TextureAddressing](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#textureaddressing)

> How to treat uv coordinates outside of [0, 1] along the Texture's height.
> ``` lang=cpp, name=Nada
> var AddressingY : TextureAddressing


---  
 #  Anisotropy : [TextureAnisotropy](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#textureanisotropy)

> Max ratio of anisotropy that filtering will account for at oblique viewing angles.
> ``` lang=cpp, name=Nada
> var Anisotropy : TextureAnisotropy


---  
 #  CompareFunc : [TextureCompareFunc](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#texturecomparefunc)

> Which method of comparison should be used if CompareMode is set to Enable.
> ``` lang=cpp, name=Nada
> var CompareFunc : TextureCompareFunc


---  
 #  CompareMode : [TextureCompareMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#texturecomparemode)

> If sampling in hardware should perform comparison instead of fetching. Requires using SamplerShadow2d in the shader.
> ``` lang=cpp, name=Nada
> var CompareMode : TextureCompareMode


---  
 #  Compression : [TextureCompression](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#texturecompression)

 `read-only`

> Block compression method being used. Requires pre-processing, cannot be set for runtime Textures.
> ``` lang=cpp, name=Nada
> var Compression : TextureCompression


---  
 #  Filtering : [TextureFiltering](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#texturefiltering)

> How samples should be blended under minification/magnification.
> ``` lang=cpp, name=Nada
> var Filtering : TextureFiltering


---  
 #  Format : [TextureFormat](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#textureformat)

 `read-only`

> Memory format of the stored pixel data. Set on Upload() for runtime Textures.
> ``` lang=cpp, name=Nada
> var Format : TextureFormat


---  
 #  Height : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Height of the Texture in pixels. Set on Upload() for runtime Textures.
> ``` lang=cpp, name=Nada
> var Height : Integer


---  
 #  MipMapping : [TextureMipMapping](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#texturemipmapping)

> If downsampled versions of the texture (mip maps) should be generated. PreGenerated is not valid for runtime Textures.
> ``` lang=cpp, name=Nada
> var MipMapping : TextureMipMapping


---  
 #  Size : [integer2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md)

 `read-only`

> Width and height (x, y) of the Texture in pixels. Set on Upload() for runtime Textures.
> ``` lang=cpp, name=Nada
> var Size : Integer2


---  
 #  Type : [TextureType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#texturetype)

 `read-only`

> The type of texture data being represented.
> ``` lang=cpp, name=Nada
> var Type : TextureType


---  
 #  Width : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Width of the Texture in pixels. Set on Upload() for runtime Textures.
> ``` lang=cpp, name=Nada
> var Width : Integer


---  
 #  Methods


---  
 #  CreateRuntime : [texture](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/texture.md)

 `static`

> Makes an anonymous Texture resource that can be defined by script and uploaded to the gpu.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function CreateRuntime() : Texture
> ``` 


---  
 #  SubUpload : Void

> Uploads the given texture data, overwriting a sub region of the texture data that is already on the gpu.
> |Name|Type|Description|
> |---|---|---|
> |textureData|[texturedata](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/texturedata.md)| |
> |xOffset|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |yOffset|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function SubUpload(textureData : TextureData, xOffset : Integer, yOffset : Integer)
> ``` 


---  
 #  Upload : Void

> Uploads the given texture data to the gpu, configured with the current settings of this Texture.
> |Name|Type|Description|
> |---|---|---|
> |textureData|[texturedata](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/texturedata.md)| |
> ``` lang=cpp, name=Nada
> function Upload(textureData : TextureData)
> ``` 


---  
 

 
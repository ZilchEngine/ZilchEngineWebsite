 `Resource` `Graphics`



(NOTE) Data that represents a texture in the way that is intended to be used by graphics hardware.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[CreateRuntime](texture.md#createruntime-zilch-engin)|[AddressingX](texture.md#addressingx-zilch-engine)|Resource| |
|[SubUpload](texture.md#subupload-void)|[AddressingY](texture.md#addressingy-zilch-engine)| | |
|[Upload](texture.md#upload-void)|[Anisotropy](texture.md#anisotropy-zilch-engine-d)| | |
| |[CompareFunc](texture.md#comparefunc-zilch-engine)| | |
| |[CompareMode](texture.md#comparemode-zilch-engine)| | |
| |[Compression](texture.md#compression-zilch-engine)| | |
| |[Filtering](texture.md#filtering-zilch-engine-do)| | |
| |[Format](texture.md#format-zilch-engine-docum)| | |
| |[Height](texture.md#height-zilch-engine-docum)| | |
| |[MipMapping](texture.md#mipmapping-zilch-engine-d)| | |
| |[Size](texture.md#size-zilch-engine-documen)| | |
| |[Type](texture.md#type-zilch-engine-documen)| | |
| |[Width](texture.md#width-zilch-engine-docume)| | |


 #  Properties


---  
 #  AddressingX : [TextureAddressing](../enum_reference.md#textureaddressing)

> How to treat uv coordinates outside of [0, 1] along the Texture's width.
> ```TS:Nada
> var AddressingX : TextureAddressing


---  
 #  AddressingY : [TextureAddressing](../enum_reference.md#textureaddressing)

> How to treat uv coordinates outside of [0, 1] along the Texture's height.
> ```TS:Nada
> var AddressingY : TextureAddressing


---  
 #  Anisotropy : [TextureAnisotropy](../enum_reference.md#textureanisotropy)

> Max ratio of anisotropy that filtering will account for at oblique viewing angles.
> ```TS:Nada
> var Anisotropy : TextureAnisotropy


---  
 #  CompareFunc : [TextureCompareFunc](../enum_reference.md#texturecomparefunc)

> Which method of comparison should be used if CompareMode is set to Enable.
> ```TS:Nada
> var CompareFunc : TextureCompareFunc


---  
 #  CompareMode : [TextureCompareMode](../enum_reference.md#texturecomparemode)

> If sampling in hardware should perform comparison instead of fetching. Requires using SamplerShadow2d in the shader.
> ```TS:Nada
> var CompareMode : TextureCompareMode


---  
 #  Compression : [TextureCompression](../enum_reference.md#texturecompression)

 `read-only`

> Block compression method being used. Requires pre-processing, cannot be set for runtime Textures.
> ```TS:Nada
> var Compression : TextureCompression


---  
 #  Filtering : [TextureFiltering](../enum_reference.md#texturefiltering)

> How samples should be blended under minification/magnification.
> ```TS:Nada
> var Filtering : TextureFiltering


---  
 #  Format : [TextureFormat](../enum_reference.md#textureformat)

 `read-only`

> Memory format of the stored pixel data. Set on Upload() for runtime Textures.
> ```TS:Nada
> var Format : TextureFormat


---  
 #  Height : [integer](../nada_base_types/integer.md)

 `read-only`

> Height of the Texture in pixels. Set on Upload() for runtime Textures.
> ```TS:Nada
> var Height : Integer


---  
 #  MipMapping : [TextureMipMapping](../enum_reference.md#texturemipmapping)

> If downsampled versions of the texture (mip maps) should be generated. PreGenerated is not valid for runtime Textures.
> ```TS:Nada
> var MipMapping : TextureMipMapping


---  
 #  Size : [integer2](../nada_base_types/integer2.md)

 `read-only`

> Width and height (x, y) of the Texture in pixels. Set on Upload() for runtime Textures.
> ```TS:Nada
> var Size : Integer2


---  
 #  Type : [TextureType](../enum_reference.md#texturetype)

 `read-only`

> The type of texture data being represented.
> ```TS:Nada
> var Type : TextureType


---  
 #  Width : [integer](../nada_base_types/integer.md)

 `read-only`

> Width of the Texture in pixels. Set on Upload() for runtime Textures.
> ```TS:Nada
> var Width : Integer


---  
 #  Methods


---  
 #  CreateRuntime : [texture](texture.md)

 `static`

> Makes an anonymous Texture resource that can be defined by script and uploaded to the gpu.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function CreateRuntime() : Texture
> ``` 


---  
 #  SubUpload : Void

> Uploads the given texture data, overwriting a sub region of the texture data that is already on the gpu.
> |Name|Type|Description|
> |---|---|---|
> |textureData|[texturedata](texturedata.md)| |
> |xOffset|[integer](../nada_base_types/integer.md)| |
> |yOffset|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function SubUpload(textureData : TextureData, xOffset : Integer, yOffset : Integer)
> ``` 


---  
 #  Upload : Void

> Uploads the given texture data to the gpu, configured with the current settings of this Texture.
> |Name|Type|Description|
> |---|---|---|
> |textureData|[texturedata](texturedata.md)| |
> ```TS:Nada
> function Upload(textureData : TextureData)
> ``` 


---  
 

 
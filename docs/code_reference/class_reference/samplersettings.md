 `Graphics`

(NOTE) Used when requesting a RenderTarget to configure how its texture is sampled.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](samplersettings.md#samplersettings-void)|[ AddressingX](samplersettings.md#addressingx-zilch-engine)| | |
| |[ AddressingY](samplersettings.md#addressingy-zilch-engine)| | |
| |[ CompareFunc](samplersettings.md#comparefunc-zilch-engine)| | |
| |[ CompareMode](samplersettings.md#comparemode-zilch-engine)| | |
| |[ Filtering](samplersettings.md#filtering-zilch-engine-do)| | |


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
 #  Filtering : [TextureFiltering](../enum_reference.md#texturefiltering)

> How samples should be blended under minification/magnification.
> ```TS:Nada
> var Filtering : TextureFiltering


---  
 #  Methods


---  
 #  SamplerSettings : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function SamplerSettings()
> ``` 


---  
 

 
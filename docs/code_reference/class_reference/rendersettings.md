 `Graphics`

(NOTE) Contains all output targets and render settings needed for a render task.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](rendersettings.md#rendersettings-void)|[ BlendSettings](rendersettings.md#blendsettings-zilch-engin)| | |
| |[ ColorTarget](rendersettings.md#colortarget-zilch-engine)| | |
| |[ CullMode](rendersettings.md#cullmode-zilch-engine-doc)| | |
| |[ DepthSettings](rendersettings.md#depthsettings-zilch-engin)| | |
| |[ DepthTarget](rendersettings.md#depthtarget-zilch-engine)| | |
| |[ GlobalShaderInputs](rendersettings.md#globalshaderinputs-zero)| | |
| |[ MultiRenderTarget](rendersettings.md#multirendertarget-zilch-e)| | |


 #  Properties


---  
 #  BlendSettings : [blendsettings](blendsettings.md)

> Settings to use when blending shader output with the ColorTarget, implicitly BlendSettings0.
> ```TS:Nada
> var BlendSettings : BlendSettings


---  
 #  ColorTarget : [rendertarget](rendertarget.md)

> The RenderTarget of a color format to output to, implicitly RenderTarget0.
> ```TS:Nada
> var ColorTarget : RenderTarget


---  
 #  CullMode : [CullMode](../enum_reference.md#cullmode)

> 
> ```TS:Nada
> var CullMode : CullMode


---  
 #  DepthSettings : [depthsettings](depthsettings.md)

> Settings to use when doing depth/stencil testing with DepthTarget.
> ```TS:Nada
> var DepthSettings : DepthSettings


---  
 #  DepthTarget : [rendertarget](rendertarget.md)

> The RenderTarget of a depth format to use as a depth buffer for depth/stencil testing.
> ```TS:Nada
> var DepthTarget : RenderTarget


---  
 #  GlobalShaderInputs : [shaderinputs](shaderinputs.md)

> Shader input values to be globally overridden for all objects/shaders.
> ```TS:Nada
> var GlobalShaderInputs : ShaderInputs


---  
 #  MultiRenderTarget : [multirendertarget](multirendertarget.md)

 `read-only`

> Interface for configuring multiple color target outputs.
> ```TS:Nada
> var MultiRenderTarget : MultiRenderTarget


---  
 #  Methods


---  
 #  RenderSettings : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function RenderSettings()
> ``` 


---  
 #  RenderSettings : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ||[rendersettings](rendersettings.md)| |
> ```TS:Nada
> function RenderSettings( : RenderSettings)
> ``` 


---  
 

 
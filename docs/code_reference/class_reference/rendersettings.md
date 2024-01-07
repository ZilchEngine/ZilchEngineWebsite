 `Graphics`

(NOTE) Contains all output targets and render settings needed for a render task.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rendersettings.md#rendersettings-void)|[ BlendSettings](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rendersettings.md#blendsettings-zilch-engin)| | |
| |[ ColorTarget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rendersettings.md#colortarget-zilch-engine)| | |
| |[ CullMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rendersettings.md#cullmode-zilch-engine-doc)| | |
| |[ DepthSettings](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rendersettings.md#depthsettings-zilch-engin)| | |
| |[ DepthTarget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rendersettings.md#depthtarget-zilch-engine)| | |
| |[ GlobalShaderInputs](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rendersettings.md#globalshaderinputs-zero)| | |
| |[ MultiRenderTarget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rendersettings.md#multirendertarget-zilch-e)| | |


 #  Properties


---  
 #  BlendSettings : [blendsettings](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/blendsettings.md)

> Settings to use when blending shader output with the ColorTarget, implicitly BlendSettings0.
> ``` lang=cpp, name=Nada
> var BlendSettings : BlendSettings


---  
 #  ColorTarget : [rendertarget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rendertarget.md)

> The RenderTarget of a color format to output to, implicitly RenderTarget0.
> ``` lang=cpp, name=Nada
> var ColorTarget : RenderTarget


---  
 #  CullMode : [CullMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#cullmode)

> 
> ``` lang=cpp, name=Nada
> var CullMode : CullMode


---  
 #  DepthSettings : [depthsettings](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/depthsettings.md)

> Settings to use when doing depth/stencil testing with DepthTarget.
> ``` lang=cpp, name=Nada
> var DepthSettings : DepthSettings


---  
 #  DepthTarget : [rendertarget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rendertarget.md)

> The RenderTarget of a depth format to use as a depth buffer for depth/stencil testing.
> ``` lang=cpp, name=Nada
> var DepthTarget : RenderTarget


---  
 #  GlobalShaderInputs : [shaderinputs](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/shaderinputs.md)

> Shader input values to be globally overridden for all objects/shaders.
> ``` lang=cpp, name=Nada
> var GlobalShaderInputs : ShaderInputs


---  
 #  MultiRenderTarget : [multirendertarget](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/multirendertarget.md)

 `read-only`

> Interface for configuring multiple color target outputs.
> ``` lang=cpp, name=Nada
> var MultiRenderTarget : MultiRenderTarget


---  
 #  Methods


---  
 #  RenderSettings : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function RenderSettings()
> ``` 


---  
 #  RenderSettings : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ||[rendersettings](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rendersettings.md)| |
> ``` lang=cpp, name=Nada
> function RenderSettings( : RenderSettings)
> ``` 


---  
 

 
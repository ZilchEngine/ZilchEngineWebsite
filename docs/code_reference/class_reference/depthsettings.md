 `Graphics`

(NOTE) Settings for how the depth buffer should control pixel output.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](depthsettings.md#depthsettings-void)|[ DepthCompareFunc](depthsettings.md#depthcomparefunc-zilch-en)| | |
| |[ DepthFailOp](depthsettings.md#depthfailop-zilch-engine)| | |
| |[ DepthFailOpBackFace](depthsettings.md#depthfailopbackface-zero)| | |
| |[ DepthMode](depthsettings.md#depthmode-zilch-engine-do)| | |
| |[ DepthPassOp](depthsettings.md#depthpassop-zilch-engine)| | |
| |[ DepthPassOpBackFace](depthsettings.md#depthpassopbackface-zero)| | |
| |[ StencilCompareFunc](depthsettings.md#stencilcomparefunc-zero)| | |
| |[ StencilCompareFuncBackFace](depthsettings.md#stencilcomparefuncbackfa)| | |
| |[ StencilFailOp](depthsettings.md#stencilfailop-zilch-engin)| | |
| |[ StencilFailOpBackFace](depthsettings.md#stencilfailopbackface-ze)| | |
| |[ StencilMode](depthsettings.md#stencilmode-zilch-engine)| | |
| |[ StencilReadMask](depthsettings.md#stencilreadmask-zilch-eng)| | |
| |[ StencilReadMaskBackFace](depthsettings.md#stencilreadmaskbackface)| | |
| |[ StencilTestValue](depthsettings.md#stenciltestvalue-zilch-en)| | |
| |[ StencilTestValueBackFace](depthsettings.md#stenciltestvaluebackface)| | |
| |[ StencilWriteMask](depthsettings.md#stencilwritemask-zilch-en)| | |
| |[ StencilWriteMaskBackFace](depthsettings.md#stencilwritemaskbackface)| | |


 #  Properties


---  
 #  DepthCompareFunc : [TextureCompareFunc](../enum_reference.md#texturecomparefunc)

> 
> ```TS:Nada
> var DepthCompareFunc : TextureCompareFunc


---  
 #  DepthFailOp : [StencilOp](../enum_reference.md#stencilop)

> 
> ```TS:Nada
> var DepthFailOp : StencilOp


---  
 #  DepthFailOpBackFace : [StencilOp](../enum_reference.md#stencilop)

> 
> ```TS:Nada
> var DepthFailOpBackFace : StencilOp


---  
 #  DepthMode : [DepthMode](../enum_reference.md#depthmode)

> 
> ```TS:Nada
> var DepthMode : DepthMode


---  
 #  DepthPassOp : [StencilOp](../enum_reference.md#stencilop)

> 
> ```TS:Nada
> var DepthPassOp : StencilOp


---  
 #  DepthPassOpBackFace : [StencilOp](../enum_reference.md#stencilop)

> 
> ```TS:Nada
> var DepthPassOpBackFace : StencilOp


---  
 #  StencilCompareFunc : [TextureCompareFunc](../enum_reference.md#texturecomparefunc)

> 
> ```TS:Nada
> var StencilCompareFunc : TextureCompareFunc


---  
 #  StencilCompareFuncBackFace : [TextureCompareFunc](../enum_reference.md#texturecomparefunc)

> 
> ```TS:Nada
> var StencilCompareFuncBackFace : TextureCompareFunc


---  
 #  StencilFailOp : [StencilOp](../enum_reference.md#stencilop)

> 
> ```TS:Nada
> var StencilFailOp : StencilOp


---  
 #  StencilFailOpBackFace : [StencilOp](../enum_reference.md#stencilop)

> 
> ```TS:Nada
> var StencilFailOpBackFace : StencilOp


---  
 #  StencilMode : [StencilMode](../enum_reference.md#stencilmode)

> 
> ```TS:Nada
> var StencilMode : StencilMode


---  
 #  StencilReadMask : [byte](../nada_base_types/byte.md)

> Bit mask for buffer value and test value when being compared.
> ```TS:Nada
> var StencilReadMask : Byte


---  
 #  StencilReadMaskBackFace : [byte](../nada_base_types/byte.md)

> Bit mask for buffer value and test value when being compared, for triangle back faces if in separate mode.
> ```TS:Nada
> var StencilReadMaskBackFace : Byte


---  
 #  StencilTestValue : [byte](../nada_base_types/byte.md)

> Value that will be used to compare against the stencil buffer for all pixels.
> ```TS:Nada
> var StencilTestValue : Byte


---  
 #  StencilTestValueBackFace : [byte](../nada_base_types/byte.md)

> Value that will be used to compare against the stencil buffer for all pixels, for triangle back faces if in separate mode.
> ```TS:Nada
> var StencilTestValueBackFace : Byte


---  
 #  StencilWriteMask : [byte](../nada_base_types/byte.md)

> Bit mask for which bits in the buffer can be modified.
> ```TS:Nada
> var StencilWriteMask : Byte


---  
 #  StencilWriteMaskBackFace : [byte](../nada_base_types/byte.md)

> Bit mask for which bits in the buffer can be modified, for triangle back faces if in separate mode.
> ```TS:Nada
> var StencilWriteMaskBackFace : Byte


---  
 #  Methods


---  
 #  DepthSettings : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function DepthSettings()
> ``` 


---  
 #  DepthSettings : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |other|[depthsettings](depthsettings.md)| |
> ```TS:Nada
> function DepthSettings(other : DepthSettings)
> ``` 


---  
 

 
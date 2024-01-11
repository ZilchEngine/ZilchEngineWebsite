 `Event` `Graphics`



(NOTE) Interface for adding tasks for the renderer, essentially defining a rendering pipeline.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddRenderTaskClearTarget](rendertasksevent.md#addrendertaskcleartarget)|[ CameraViewportCog](rendertasksevent.md#cameraviewportcog-zilch-e)|[event](event.md)| |
|[ AddRenderTaskPostProcess](rendertasksevent.md#addrendertaskpostprocess)|[ ViewportSize](rendertasksevent.md#viewportsize-zilch-engine)| | |
|[ AddRenderTaskRenderPass](rendertasksevent.md#addrendertaskrenderpass)| | | |
|[ AddRenderTaskSubRenderGroupPass](rendertasksevent.md#addrendertasksubrendergr)| | | |
|[ CreateSubRenderGroupPass](rendertasksevent.md#createsubrendergrouppass)| | | |
|[ GetFinalTarget](rendertasksevent.md#getfinaltarget-zilch-engi)| | | |
|[ GetRenderTarget](rendertasksevent.md#getrendertarget-zilch-eng)| | | |


 #  Properties


---  
 #  CameraViewportCog : [cog](cog.md)

 `read-only`

> Object with the CameraViewport component that this event is getting tasks for.
> ``` lang=cpp, name=Nada
> var CameraViewportCog : Cog


---  
 #  ViewportSize : [integer2](../nada_base_types/integer2.md)

 `read-only`

> Size of the UI viewport, or the resolution on CameraViewport if not rendering to viewport.
> ``` lang=cpp, name=Nada
> var ViewportSize : Integer2


---  
 #  Methods


---  
 #  AddRenderTaskClearTarget : Void

> Initializes all the internal texture data for the given RenderTargets.
> |Name|Type|Description|
> |---|---|---|
> |renderSettings|[rendersettings](rendersettings.md)| |
> |color|[real4](../nada_base_types/real4.md)| |
> ``` lang=cpp, name=Nada
> function AddRenderTaskClearTarget(renderSettings : RenderSettings, color : Real4)
> ``` 


---  
 #  AddRenderTaskClearTarget : Void

> Initializes all the internal texture data for the given RenderTargets.
> |Name|Type|Description|
> |---|---|---|
> |renderSettings|[rendersettings](rendersettings.md)| |
> |color|[real4](../nada_base_types/real4.md)| |
> |depth|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function AddRenderTaskClearTarget(renderSettings : RenderSettings, color : Real4, depth : Real)
> ``` 


---  
 #  AddRenderTaskClearTarget : Void

> Initializes all the internal texture data for the given RenderTargets.
> |Name|Type|Description|
> |---|---|---|
> |renderSettings|[rendersettings](rendersettings.md)| |
> |color|[real4](../nada_base_types/real4.md)| |
> |depth|[real](../nada_base_types/real.md)| |
> |stencil|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function AddRenderTaskClearTarget(renderSettings : RenderSettings, color : Real4, depth : Real, stencil : Integer)
> ``` 


---  
 #  AddRenderTaskClearTarget : Void

> Initializes all the internal texture data for the given RenderTargets.
> |Name|Type|Description|
> |---|---|---|
> |renderSettings|[rendersettings](rendersettings.md)| |
> |color|[real4](../nada_base_types/real4.md)| |
> |depth|[real](../nada_base_types/real.md)| |
> |stencil|[integer](../nada_base_types/integer.md)| |
> |stencilWriteMask|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function AddRenderTaskClearTarget(renderSettings : RenderSettings, color : Real4, depth : Real, stencil : Integer, stencilWriteMask : Integer)
> ``` 


---  
 #  AddRenderTaskClearTarget : Void

> Initializes all the internal texture data for the given RenderTargets.
> |Name|Type|Description|
> |---|---|---|
> |depthTarget|[rendertarget](rendertarget.md)| |
> |depth|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function AddRenderTaskClearTarget(depthTarget : RenderTarget, depth : Real)
> ``` 


---  
 #  AddRenderTaskClearTarget : Void

> Initializes all the internal texture data for the given RenderTargets.
> |Name|Type|Description|
> |---|---|---|
> |depthTarget|[rendertarget](rendertarget.md)| |
> |depth|[real](../nada_base_types/real.md)| |
> |stencil|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function AddRenderTaskClearTarget(depthTarget : RenderTarget, depth : Real, stencil : Integer)
> ``` 


---  
 #  AddRenderTaskClearTarget : Void

> Initializes all the internal texture data for the given RenderTargets.
> |Name|Type|Description|
> |---|---|---|
> |depthTarget|[rendertarget](rendertarget.md)| |
> |depth|[real](../nada_base_types/real.md)| |
> |stencil|[integer](../nada_base_types/integer.md)| |
> |stencilWriteMask|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function AddRenderTaskClearTarget(depthTarget : RenderTarget, depth : Real, stencil : Integer, stencilWriteMask : Integer)
> ``` 


---  
 #  AddRenderTaskClearTarget : Void

> Initializes all the internal texture data for the given RenderTargets.
> |Name|Type|Description|
> |---|---|---|
> |colorTarget|[rendertarget](rendertarget.md)| |
> |color|[real4](../nada_base_types/real4.md)| |
> ``` lang=cpp, name=Nada
> function AddRenderTaskClearTarget(colorTarget : RenderTarget, color : Real4)
> ``` 


---  
 #  AddRenderTaskClearTarget : Void

> Initializes all the internal texture data for the given RenderTargets.
> |Name|Type|Description|
> |---|---|---|
> |colorTarget|[rendertarget](rendertarget.md)| |
> |depthTarget|[rendertarget](rendertarget.md)| |
> |color|[real4](../nada_base_types/real4.md)| |
> |depth|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function AddRenderTaskClearTarget(colorTarget : RenderTarget, depthTarget : RenderTarget, color : Real4, depth : Real)
> ``` 


---  
 #  AddRenderTaskClearTarget : Void

> Initializes all the internal texture data for the given RenderTargets.
> |Name|Type|Description|
> |---|---|---|
> |colorTarget|[rendertarget](rendertarget.md)| |
> |depthTarget|[rendertarget](rendertarget.md)| |
> |color|[real4](../nada_base_types/real4.md)| |
> |depth|[real](../nada_base_types/real.md)| |
> |stencil|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function AddRenderTaskClearTarget(colorTarget : RenderTarget, depthTarget : RenderTarget, color : Real4, depth : Real, stencil : Integer)
> ``` 


---  
 #  AddRenderTaskClearTarget : Void

> Initializes all the internal texture data for the given RenderTargets.
> |Name|Type|Description|
> |---|---|---|
> |colorTarget|[rendertarget](rendertarget.md)| |
> |depthTarget|[rendertarget](rendertarget.md)| |
> |color|[real4](../nada_base_types/real4.md)| |
> |depth|[real](../nada_base_types/real.md)| |
> |stencil|[integer](../nada_base_types/integer.md)| |
> |stencilWriteMask|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function AddRenderTaskClearTarget(colorTarget : RenderTarget, depthTarget : RenderTarget, color : Real4, depth : Real, stencil : Integer, stencilWriteMask : Integer)
> ``` 


---  
 #  AddRenderTaskPostProcess : Void

> Invokes the pixel shader for every pixel of the RenderTargets.
> |Name|Type|Description|
> |---|---|---|
> |renderSettings|[rendersettings](rendersettings.md)| |
> |material|[material](material.md)| |
> ``` lang=cpp, name=Nada
> function AddRenderTaskPostProcess(renderSettings : RenderSettings, material : Material)
> ``` 


---  
 #  AddRenderTaskPostProcess : Void

> Invokes the pixel shader for every pixel of the RenderTargets.
> |Name|Type|Description|
> |---|---|---|
> |renderSettings|[rendersettings](rendersettings.md)| |
> |postProcess|[materialblock](materialblock.md)| |
> ``` lang=cpp, name=Nada
> function AddRenderTaskPostProcess(renderSettings : RenderSettings, postProcess : MaterialBlock)
> ``` 


---  
 #  AddRenderTaskPostProcess : Void

> Invokes the pixel shader for every pixel of the RenderTargets.
> |Name|Type|Description|
> |---|---|---|
> |renderTarget|[rendertarget](rendertarget.md)| |
> |material|[material](material.md)| |
> ``` lang=cpp, name=Nada
> function AddRenderTaskPostProcess(renderTarget : RenderTarget, material : Material)
> ``` 


---  
 #  AddRenderTaskPostProcess : Void

> Invokes the pixel shader for every pixel of the RenderTargets.
> |Name|Type|Description|
> |---|---|---|
> |renderTarget|[rendertarget](rendertarget.md)| |
> |postProcess|[materialblock](materialblock.md)| |
> ``` lang=cpp, name=Nada
> function AddRenderTaskPostProcess(renderTarget : RenderTarget, postProcess : MaterialBlock)
> ``` 


---  
 #  AddRenderTaskRenderPass : Void

> Renders a group of objects with the given settings. The RenderPass fragment defines what data is written to RenderTargets.
> |Name|Type|Description|
> |---|---|---|
> |renderSettings|[rendersettings](rendersettings.md)| |
> |graphicalRange|[graphicalrangeinterface](graphicalrangeinterface.md)| |
> |renderPass|[materialblock](materialblock.md)| |
> ``` lang=cpp, name=Nada
> function AddRenderTaskRenderPass(renderSettings : RenderSettings, graphicalRange : GraphicalRangeInterface, renderPass : MaterialBlock)
> ``` 


---  
 #  AddRenderTaskRenderPass : Void

> Renders a group of objects with the given settings. The RenderPass fragment defines what data is written to RenderTargets.
> |Name|Type|Description|
> |---|---|---|
> |renderSettings|[rendersettings](rendersettings.md)| |
> |renderGroup|[rendergroup](rendergroup.md)| |
> |renderPass|[materialblock](materialblock.md)| |
> ``` lang=cpp, name=Nada
> function AddRenderTaskRenderPass(renderSettings : RenderSettings, renderGroup : RenderGroup, renderPass : MaterialBlock)
> ``` 


---  
 #  AddRenderTaskSubRenderGroupPass : Void

> Renders all objects within a RenderGroup hierarchy, sorted in the order defined by the base RenderGroup, and can use unique render settings for each RenderGroup in the hierarchy.
> |Name|Type|Description|
> |---|---|---|
> |subRenderGroupPass|[subrendergrouppass](subrendergrouppass.md)| |
> ``` lang=cpp, name=Nada
> function AddRenderTaskSubRenderGroupPass(subRenderGroupPass : SubRenderGroupPass)
> ``` 


---  
 #  CreateSubRenderGroupPass : [subrendergrouppass](subrendergrouppass.md)

> Creates the interface used to define unique render settings for a base RenderGroup and its sub RenderGroups. The given RenderGroup is used to define the hierarchy, or sub hierarchy, that should be rendered. The given RenderGroup also defines the sort order for all objects that are within its hierarchy. Returned SubRenderGroupPass is only valid during this event.
> |Name|Type|Description|
> |---|---|---|
> |baseGroup|[rendergroup](rendergroup.md)| |
> ``` lang=cpp, name=Nada
> function CreateSubRenderGroupPass(baseGroup : RenderGroup) : SubRenderGroupPass
> ``` 


---  
 #  GetFinalTarget : [rendertarget](rendertarget.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ||[integer2](../nada_base_types/integer2.md)| |
> ||[TextureFormat](../enum_reference.md#textureformat)| |
> ``` lang=cpp, name=Nada
> function GetFinalTarget( : Integer2,  : TextureFormat) : RenderTarget
> ``` 


---  
 #  GetFinalTarget : [rendertarget](rendertarget.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ||[integer2](../nada_base_types/integer2.md)| |
> ||[TextureFormat](../enum_reference.md#textureformat)| |
> ||[samplersettings](samplersettings.md)| |
> ``` lang=cpp, name=Nada
> function GetFinalTarget( : Integer2,  : TextureFormat,  : SamplerSettings) : RenderTarget
> ``` 


---  
 #  GetRenderTarget : [rendertarget](rendertarget.md)

> Returns a RenderTarget for use when adding render tasks. Target only valid during this event. Will render to the given texture instead of an internally managed texture.
> |Name|Type|Description|
> |---|---|---|
> ||[integer2](../nada_base_types/integer2.md)| |
> ||[TextureFormat](../enum_reference.md#textureformat)| |
> ``` lang=cpp, name=Nada
> function GetRenderTarget( : Integer2,  : TextureFormat) : RenderTarget
> ``` 


---  
 #  GetRenderTarget : [rendertarget](rendertarget.md)

> Returns a RenderTarget for use when adding render tasks. Target only valid during this event. Will render to the given texture instead of an internally managed texture.
> |Name|Type|Description|
> |---|---|---|
> ||[integer2](../nada_base_types/integer2.md)| |
> ||[TextureFormat](../enum_reference.md#textureformat)| |
> ||[samplersettings](samplersettings.md)| |
> ``` lang=cpp, name=Nada
> function GetRenderTarget( : Integer2,  : TextureFormat,  : SamplerSettings) : RenderTarget
> ``` 


---  
 #  GetRenderTarget : [rendertarget](rendertarget.md)

> Returns a RenderTarget for use when adding render tasks. Target only valid during this event. Will render to the given texture instead of an internally managed texture.
> |Name|Type|Description|
> |---|---|---|
> |texture|[texture](texture.md)| |
> ``` lang=cpp, name=Nada
> function GetRenderTarget(texture : Texture) : RenderTarget
> ``` 


---  
 

 
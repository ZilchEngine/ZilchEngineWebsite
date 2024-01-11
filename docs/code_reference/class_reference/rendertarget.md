 `Graphics`

(NOTE) Interface for rendering output. Texture data is managed and recycled by the engine.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Release](rendertarget.md#release-void)|[ Texture](rendertarget.md#texture-zilch-engine-docu)|[safeid32](safeid32.md)| |


 #  Properties


---  
 #  Texture : [texture](texture.md)

 `read-only`

> Texture that is rendered to. Can be used as shader input to a separate rendering operation.
> ```TS:Nada
> var Texture : Texture


---  
 #  Methods


---  
 #  Release : Void

> Allows the managed Texture being referenced by this RenderTarget to be reused by the renderer if the same specifications are requested again. Also deletes this RenderTarget.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Release()
> ``` 


---  
 

 
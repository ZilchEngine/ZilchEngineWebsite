 `Component` `Gameplay`



(NOTE) Manages all setup between Camera, Renderer, and viewport UI that is required to define how anything is to be rendered.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](cameraviewport.md#cameraviewport-void)|[Camera](cameraviewport.md#camera-zilch-engine-docum)|[component](component.md)| |
|[ScreenToViewport](cameraviewport.md#screentoviewport-zilch-en)|[CameraPath](cameraviewport.md#camerapath-zilch-engine-d)| | |
|[ScreenToWorldPlane](cameraviewport.md#screentoworldplane-zero)|[FinalTexture](cameraviewport.md#finaltexture-zilch-engine)| | |
|[ScreenToWorldRay](cameraviewport.md#screentoworldray-zilch-en)|[ForwardViewportEvents](cameraviewport.md#forwardviewportevents-ze)| | |
|[ScreenToWorldViewPlane](cameraviewport.md#screentoworldviewplane-z)|[Frustum](cameraviewport.md#frustum-zilch-engine-docu)| | |
|[ScreenToWorldZPlane](cameraviewport.md#screentoworldzplane-zero)|[MarginColor](cameraviewport.md#margincolor-zilch-engine)| | |
|[ViewPlaneSize](cameraviewport.md#viewplanesize-zilch-engin)|[MouseWorldRay](cameraviewport.md#mouseworldray-zilch-engin)| | |
|[ViewportTakeFocus](cameraviewport.md#viewporttakefocus-zilch-e)|[NormalizedOffset](cameraviewport.md#normalizedoffset-zilch-en)| | |
|[ViewportToScreen](cameraviewport.md#viewporttoscreen-zilch-en)|[NormalizedSize](cameraviewport.md#normalizedsize-zilch-engi)| | |
|[WorldToScreen](cameraviewport.md#worldtoscreen-zilch-engin)|[RendererPath](cameraviewport.md#rendererpath-zilch-engine)| | |
| |[RenderInEditor](cameraviewport.md#renderineditor-zilch-engi)| | |
| |[RenderInGame](cameraviewport.md#renderingame-zilch-engine)| | |
| |[RenderOrder](cameraviewport.md#renderorder-zilch-engine)| | |
| |[RenderToViewport](cameraviewport.md#rendertoviewport-zilch-en)| | |
| |[ResolutionOrAspect](cameraviewport.md#resolutionoraspect-zero)| | |
| |[ViewportHasFocus](cameraviewport.md#viewporthasfocus-zilch-en)| | |
| |[ViewportOffset](cameraviewport.md#viewportoffset-zilch-engi)| | |
| |[ViewportOffsetWithMargin](cameraviewport.md#viewportoffsetwithmargin)| | |
| |[ViewportResolution](cameraviewport.md#viewportresolution-zero)| | |
| |[ViewportResolutionWithMargin](cameraviewport.md#viewportresolutionwithma)| | |
| |[ViewportScaling](cameraviewport.md#viewportscaling-zilch-eng)| | |
| |[ViewToPerspective](cameraviewport.md#viewtoperspective-zilch-e)| | |
| |[WorldToPerspective](cameraviewport.md#worldtoperspective-zero)| | |
| |[WorldToView](cameraviewport.md#worldtoview-zilch-engine)| | |


 #  Properties


---  
 #  Camera : [camera](camera.md)

 `read-only`

> Find the Camera component from the CameraPath (or null if it doesn't exist).
> ```TS:Nada
> var Camera : Camera


---  
 #  CameraPath : [cogpath](cogpath.md)

> Object with the Camera component to be used for rendering. A Camera can only be used by one CameraViewport, if already used by another usage will be stolen when assigned.
> ```TS:Nada
> var CameraPath : CogPath


---  
 #  FinalTexture : [texture](texture.md)

 `read-only`

> Texture that contains the end result of this CameraViewport's rendering. Must be explicitly written to in renderer script.
> ```TS:Nada
> var FinalTexture : Texture


---  
 #  ForwardViewportEvents : [boolean](../nada_base_types/boolean.md)

> Forwards mouse events to viewports underneath this viewport.
> ```TS:Nada
> var ForwardViewportEvents : Boolean


---  
 #  Frustum : [frustum](frustum.md)

 `read-only`

> Creates a frustum using the CameraViewport's settings (including aspect ratio). If the Camera is null, then this will throw an exception.
> ```TS:Nada
> var Frustum : Frustum


---  
 #  MarginColor : [real4](../nada_base_types/real4.md)

> Color to used for letterbox/scaling margins.
> ```TS:Nada
> var MarginColor : Real4


---  
 #  MouseWorldRay : [ray](ray.md)

 `read-only`

> Get the world ray starting from the mouse.
> ```TS:Nada
> var MouseWorldRay : Ray


---  
 #  NormalizedOffset : [real2](../nada_base_types/real2.md)

> Offset of the viewport in normalized UI coordinates.
> ```TS:Nada
> var NormalizedOffset : Real2


---  
 #  NormalizedSize : [real2](../nada_base_types/real2.md)

> Size of viewport in normalized UI coordinates.
> ```TS:Nada
> var NormalizedSize : Real2


---  
 #  RendererPath : [cogpath](cogpath.md)

> Object with renderer script that connects to RenderTasksUpdate that determines what rendering will be done.
> ```TS:Nada
> var RendererPath : CogPath


---  
 #  RenderInEditor : [boolean](../nada_base_types/boolean.md)

> If rendering will be ran in edit mode.
> ```TS:Nada
> var RenderInEditor : Boolean


---  
 #  RenderInGame : [boolean](../nada_base_types/boolean.md)

> If rendering will be ran in play game mode.
> ```TS:Nada
> var RenderInGame : Boolean


---  
 #  RenderOrder : [integer](../nada_base_types/integer.md)

> The order that rendering should be done relative to other CameraViewports, lowest to highest.
> ```TS:Nada
> var RenderOrder : Integer


---  
 #  RenderToViewport : [boolean](../nada_base_types/boolean.md)

> If the rendering result in FinalTexture should also be placed on the UI viewport.
> ```TS:Nada
> var RenderToViewport : Boolean


---  
 #  ResolutionOrAspect : [integer2](../nada_base_types/integer2.md)

> 
> ```TS:Nada
> var ResolutionOrAspect : Integer2


---  
 #  ViewportHasFocus : [boolean](../nada_base_types/boolean.md)

 `read-only`

> If the viewport created by this CameraViewport, if rendering to one, has focus.
> ```TS:Nada
> var ViewportHasFocus : Boolean


---  
 #  ViewportOffset : [real2](../nada_base_types/real2.md)

 `read-only`

> The current offset of the viewport, in pixels.
> ```TS:Nada
> var ViewportOffset : Real2


---  
 #  ViewportOffsetWithMargin : [real2](../nada_base_types/real2.md)

 `read-only`

> The current offset of the viewport's margin, in pixels.
> ```TS:Nada
> var ViewportOffsetWithMargin : Real2


---  
 #  ViewportResolution : [real2](../nada_base_types/real2.md)

 `read-only`

> The current resolution of the viewport.
> ```TS:Nada
> var ViewportResolution : Real2


---  
 #  ViewportResolutionWithMargin : [real2](../nada_base_types/real2.md)

 `read-only`

> The current resolution of the viewport including margin.
> ```TS:Nada
> var ViewportResolutionWithMargin : Real2


---  
 #  ViewportScaling : [ViewportScaling](../enum_reference.md#viewportscaling)

> Method to use for sizing the viewport.
> ```TS:Nada
> var ViewportScaling : ViewportScaling


---  
 #  ViewToPerspective : [real4x4](../nada_base_types/real4x4.md)

 `read-only`

> Transformation that defines how the view frustum is mapped to normalized coordinates, pre W divide.
> ```TS:Nada
> var ViewToPerspective : Real4x4


---  
 #  WorldToPerspective : [real4x4](../nada_base_types/real4x4.md)

 `read-only`

> Concatenation of the WorldToView and ViewToPerspective transformations.
> ```TS:Nada
> var WorldToPerspective : Real4x4


---  
 #  WorldToView : [real4x4](../nada_base_types/real4x4.md)

 `read-only`

> Transformation that defines view space as the Camera at the origin and the view direction as -Z.
> ```TS:Nada
> var WorldToView : Real4x4


---  
 #  Methods


---  
 #  CameraViewport : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function CameraViewport()
> ``` 


---  
 #  ScreenToViewport : [real2](../nada_base_types/real2.md)

> Convert a screen point to a point relative to the viewport.
> |Name|Type|Description|
> |---|---|---|
> |screenPoint|[real2](../nada_base_types/real2.md)| |
> ```TS:Nada
> function ScreenToViewport(screenPoint : Real2) : Real2
> ``` 


---  
 #  ScreenToWorldPlane : [real3](../nada_base_types/real3.md)

> Convert the screen point to a position on a given plane.
> |Name|Type|Description|
> |---|---|---|
> |screenPoint|[real2](../nada_base_types/real2.md)| |
> |worldPlaneNormal|[real3](../nada_base_types/real3.md)| |
> |worldPlanePosition|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function ScreenToWorldPlane(screenPoint : Real2, worldPlaneNormal : Real3, worldPlanePosition : Real3) : Real3
> ``` 


---  
 #  ScreenToWorldRay : [ray](ray.md)

> Convert a screen point to a ray.
> |Name|Type|Description|
> |---|---|---|
> |screenPoint|[real2](../nada_base_types/real2.md)| |
> ```TS:Nada
> function ScreenToWorldRay(screenPoint : Real2) : Ray
> ``` 


---  
 #  ScreenToWorldViewPlane : [real3](../nada_base_types/real3.md)

> Convert the screen point to a position on the view plane at a given depth.
> |Name|Type|Description|
> |---|---|---|
> |screenPoint|[real2](../nada_base_types/real2.md)| |
> |viewDepth|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function ScreenToWorldViewPlane(screenPoint : Real2, viewDepth : Real) : Real3
> ``` 


---  
 #  ScreenToWorldZPlane : [real3](../nada_base_types/real3.md)

> Convert the screen point to a position on the z plane at a given depth.
> |Name|Type|Description|
> |---|---|---|
> |screenPoint|[real2](../nada_base_types/real2.md)| |
> |worldDepth|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function ScreenToWorldZPlane(screenPoint : Real2, worldDepth : Real) : Real3
> ``` 


---  
 #  ViewPlaneSize : [real2](../nada_base_types/real2.md)

> Size of the screen at a Depth.
> |Name|Type|Description|
> |---|---|---|
> |viewDepth|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function ViewPlaneSize(viewDepth : Real) : Real2
> ``` 


---  
 #  ViewportTakeFocus : [boolean](../nada_base_types/boolean.md)

> Returns whether or not it succeeded in taking focus. Will always fail if RenderToViewport is false.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ViewportTakeFocus() : Boolean
> ``` 


---  
 #  ViewportToScreen : [real2](../nada_base_types/real2.md)

> Convert a viewport point to a screen point.
> |Name|Type|Description|
> |---|---|---|
> |viewportPoint|[real2](../nada_base_types/real2.md)| |
> ```TS:Nada
> function ViewportToScreen(viewportPoint : Real2) : Real2
> ``` 


---  
 #  WorldToScreen : [real2](../nada_base_types/real2.md)

> Convert a world point to a screen point.
> |Name|Type|Description|
> |---|---|---|
> |worldPoint|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function WorldToScreen(worldPoint : Real3) : Real2
> ``` 


---  
 

 
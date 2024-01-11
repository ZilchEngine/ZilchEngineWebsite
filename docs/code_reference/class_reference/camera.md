 `Component` `Graphics`



(NOTE) Represents a viewpoint for rendering.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](camera.md#camera-void)|[ CameraViewportCog](camera.md#cameraviewportcog-zilch-e)|[component](component.md)| |
|[ GetFrustum](camera.md#getfrustum-zilch-engine-d)|[ FarPlane](camera.md#farplane-zilch-engine-doc)| | |
| |[ FieldOfView](camera.md#fieldofview-zilch-engine)| | |
| |[ NearPlane](camera.md#nearplane-zilch-engine-do)| | |
| |[ PerspectiveMode](camera.md#perspectivemode-zilch-eng)| | |
| |[ Size](camera.md#size-zilch-engine-documen)| | |
| |[ WorldDirection](camera.md#worlddirection-zilch-engi)| | |
| |[ WorldTranslation](camera.md#worldtranslation-zilch-en)| | |
| |[ WorldUp](camera.md#worldup-zilch-engine-docu)| | |


 #  Properties


---  
 #  CameraViewportCog : [cog](cog.md)

 `read-only`

> The object that has a CameraViewport component using this Camera, if any.
> ```TS:Nada
> var CameraViewportCog : Cog


---  
 #  FarPlane : [real](../nada_base_types/real.md)

> The far clipping plane, always positive and in the view direction.
> ```TS:Nada
> var FarPlane : Real


---  
 #  FieldOfView : [real](../nada_base_types/real.md)

> The vertical field of view of the Camera, in degrees. Horizontal fov derived from aspect ratio (Hor+).
> ```TS:Nada
> var FieldOfView : Real


---  
 #  NearPlane : [real](../nada_base_types/real.md)

> The near clipping plane, always positive and in the view direction.
> ```TS:Nada
> var NearPlane : Real


---  
 #  PerspectiveMode : [PerspectiveMode](../enum_reference.md#perspectivemode)

> How the scene is projected on to the view plane.
> ```TS:Nada
> var PerspectiveMode : PerspectiveMode


---  
 #  Size : [real](../nada_base_types/real.md)

> Size (width and height) of the orthographic projection, in world units.
> ```TS:Nada
> var Size : Real


---  
 #  WorldDirection : [real3](../nada_base_types/real3.md)

 `read-only`

> Direction the Camera is facing, in world space.
> ```TS:Nada
> var WorldDirection : Real3


---  
 #  WorldTranslation : [real3](../nada_base_types/real3.md)

 `read-only`

> Translation of the Camera, in world space.
> ```TS:Nada
> var WorldTranslation : Real3


---  
 #  WorldUp : [real3](../nada_base_types/real3.md)

 `read-only`

> The upright direction of the Camera(perpendicular to facing direction), in world space.
> ```TS:Nada
> var WorldUp : Real3


---  
 #  Methods


---  
 #  Camera : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Camera()
> ``` 


---  
 #  GetFrustum : [frustum](frustum.md)

> Creates a frustum using the Camera's settings along with the given aspect ratio.
> |Name|Type|Description|
> |---|---|---|
> |aspect|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function GetFrustum(aspect : Real) : Frustum
> ``` 


---  
 

 
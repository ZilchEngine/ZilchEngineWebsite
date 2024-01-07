 `Component` `Graphics`



(NOTE) Represents a viewpoint for rendering.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/camera.md#camera-void)|[ CameraViewportCog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/camera.md#cameraviewportcog-zilch-e)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)| |
|[ GetFrustum](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/camera.md#getfrustum-zilch-engine-d)|[ FarPlane](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/camera.md#farplane-zilch-engine-doc)| | |
| |[ FieldOfView](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/camera.md#fieldofview-zilch-engine)| | |
| |[ NearPlane](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/camera.md#nearplane-zilch-engine-do)| | |
| |[ PerspectiveMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/camera.md#perspectivemode-zilch-eng)| | |
| |[ Size](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/camera.md#size-zilch-engine-documen)| | |
| |[ WorldDirection](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/camera.md#worlddirection-zilch-engi)| | |
| |[ WorldTranslation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/camera.md#worldtranslation-zilch-en)| | |
| |[ WorldUp](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/camera.md#worldup-zilch-engine-docu)| | |


 #  Properties


---  
 #  CameraViewportCog : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

 `read-only`

> The object that has a CameraViewport component using this Camera, if any.
> ``` lang=cpp, name=Nada
> var CameraViewportCog : Cog


---  
 #  FarPlane : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The far clipping plane, always positive and in the view direction.
> ``` lang=cpp, name=Nada
> var FarPlane : Real


---  
 #  FieldOfView : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The vertical field of view of the Camera, in degrees. Horizontal fov derived from aspect ratio (Hor+).
> ``` lang=cpp, name=Nada
> var FieldOfView : Real


---  
 #  NearPlane : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The near clipping plane, always positive and in the view direction.
> ``` lang=cpp, name=Nada
> var NearPlane : Real


---  
 #  PerspectiveMode : [PerspectiveMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#perspectivemode)

> How the scene is projected on to the view plane.
> ``` lang=cpp, name=Nada
> var PerspectiveMode : PerspectiveMode


---  
 #  Size : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Size (width and height) of the orthographic projection, in world units.
> ``` lang=cpp, name=Nada
> var Size : Real


---  
 #  WorldDirection : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

 `read-only`

> Direction the Camera is facing, in world space.
> ``` lang=cpp, name=Nada
> var WorldDirection : Real3


---  
 #  WorldTranslation : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

 `read-only`

> Translation of the Camera, in world space.
> ``` lang=cpp, name=Nada
> var WorldTranslation : Real3


---  
 #  WorldUp : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

 `read-only`

> The upright direction of the Camera(perpendicular to facing direction), in world space.
> ``` lang=cpp, name=Nada
> var WorldUp : Real3


---  
 #  Methods


---  
 #  Camera : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Camera()
> ``` 


---  
 #  GetFrustum : [frustum](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/frustum.md)

> Creates a frustum using the Camera's settings along with the given aspect ratio.
> |Name|Type|Description|
> |---|---|---|
> |aspect|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function GetFrustum(aspect : Real) : Frustum
> ``` 


---  
 

 
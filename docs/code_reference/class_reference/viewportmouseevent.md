 `Event` `Gameplay`



(NOTE) All mouse events that are forwarded to reactive components or the space use this event to add extra data.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ToWorldPlane](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/viewportmouseevent.md#toworldplane-zilch-engine)|[ CameraViewport](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/viewportmouseevent.md#cameraviewport-zilch-engi)|[mouseevent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/mouseevent.md)|[manipulatortoolevent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/manipulatortoolevent.md)|
|[ ToWorldViewPlane](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/viewportmouseevent.md#toworldviewplane-zilch-en)|[ HitDistance](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/viewportmouseevent.md#hitdistance-zilch-engine)| | |
|[ ToWorldZPlane](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/viewportmouseevent.md#toworldzplane-zilch-engin)|[ HitNormal](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/viewportmouseevent.md#hitnormal-zilch-engine-do)| | |
| |[ HitObject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/viewportmouseevent.md#hitobject-zilch-engine-do)| | |
| |[ HitPosition](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/viewportmouseevent.md#hitposition-zilch-engine)| | |
| |[ HitUv](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/viewportmouseevent.md#hituv-zilch-engine-docume)| | |
| |[ RayDirection](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/viewportmouseevent.md#raydirection-zilch-engine)| | |
| |[ RayStart](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/viewportmouseevent.md#raystart-zilch-engine-doc)| | |
| |[ WorldRay](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/viewportmouseevent.md#worldray-zilch-engine-doc)| | |


 #  Properties


---  
 #  CameraViewport : [cameraviewport](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cameraviewport.md)

 `read-only`

> Camera viewport that generated this event.
> ``` lang=cpp, name=Nada
> var CameraViewport : CameraViewport


---  
 #  HitDistance : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The distance away the hit point is. Used with Reactive components.
> ``` lang=cpp, name=Nada
> var HitDistance : Real


---  
 #  HitNormal : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The normal at the intersection point with an object. Used with Reactive components.
> ``` lang=cpp, name=Nada
> var HitNormal : Real3


---  
 #  HitObject : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

 `read-only`

> Object hit in ray cast.
> ``` lang=cpp, name=Nada
> var HitObject : Cog


---  
 #  HitPosition : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The intersection point with an object. Used with Reactive components.
> ``` lang=cpp, name=Nada
> var HitPosition : Real3


---  
 #  HitUv : [real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)

> The uv texture coordinate at the intersection point, if applicable. Used with Reactive components.
> ``` lang=cpp, name=Nada
> var HitUv : Real2


---  
 #  RayDirection : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Mouse Ray Direction.
> ``` lang=cpp, name=Nada
> var RayDirection : Real3


---  
 #  RayStart : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Mouse Ray start.
> ``` lang=cpp, name=Nada
> var RayStart : Real3


---  
 #  WorldRay : [ray](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ray.md)

> The world mouse ray.
> ``` lang=cpp, name=Nada
> var WorldRay : Ray


---  
 #  Methods


---  
 #  ToWorldPlane : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The world mouse position on any arbitrary plane.
> |Name|Type|Description|
> |---|---|---|
> |worldPlaneNormal|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |worldPlanePosition|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function ToWorldPlane(worldPlaneNormal : Real3, worldPlanePosition : Real3) : Real3
> ``` 


---  
 #  ToWorldViewPlane : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The world mouse position on the view plane at view depth.
> |Name|Type|Description|
> |---|---|---|
> |viewDepth|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function ToWorldViewPlane(viewDepth : Real) : Real3
> ``` 


---  
 #  ToWorldZPlane : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The world mouse position on the z plane at depth.
> |Name|Type|Description|
> |---|---|---|
> |worldDepth|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function ToWorldZPlane(worldDepth : Real) : Real3
> ``` 


---  
 

 
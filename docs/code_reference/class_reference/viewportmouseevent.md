 `Event` `Gameplay`



(NOTE) All mouse events that are forwarded to reactive components or the space use this event to add extra data.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ToWorldPlane](viewportmouseevent.md#toworldplane-zilch-engine)|[CameraViewport](viewportmouseevent.md#cameraviewport-zilch-engi)|[mouseevent](mouseevent.md)|[manipulatortoolevent](manipulatortoolevent.md)|
|[ToWorldViewPlane](viewportmouseevent.md#toworldviewplane-zilch-en)|[HitDistance](viewportmouseevent.md#hitdistance-zilch-engine)| | |
|[ToWorldZPlane](viewportmouseevent.md#toworldzplane-zilch-engin)|[HitNormal](viewportmouseevent.md#hitnormal-zilch-engine-do)| | |
| |[HitObject](viewportmouseevent.md#hitobject-zilch-engine-do)| | |
| |[HitPosition](viewportmouseevent.md#hitposition-zilch-engine)| | |
| |[HitUv](viewportmouseevent.md#hituv-zilch-engine-docume)| | |
| |[RayDirection](viewportmouseevent.md#raydirection-zilch-engine)| | |
| |[RayStart](viewportmouseevent.md#raystart-zilch-engine-doc)| | |
| |[WorldRay](viewportmouseevent.md#worldray-zilch-engine-doc)| | |


 #  Properties


---  
 #  CameraViewport : [cameraviewport](cameraviewport.md)

 `read-only`

> Camera viewport that generated this event.
> ```TS:Nada
> var CameraViewport : CameraViewport


---  
 #  HitDistance : [real](../nada_base_types/real.md)

> The distance away the hit point is. Used with Reactive components.
> ```TS:Nada
> var HitDistance : Real


---  
 #  HitNormal : [real3](../nada_base_types/real3.md)

> The normal at the intersection point with an object. Used with Reactive components.
> ```TS:Nada
> var HitNormal : Real3


---  
 #  HitObject : [cog](cog.md)

 `read-only`

> Object hit in ray cast.
> ```TS:Nada
> var HitObject : Cog


---  
 #  HitPosition : [real3](../nada_base_types/real3.md)

> The intersection point with an object. Used with Reactive components.
> ```TS:Nada
> var HitPosition : Real3


---  
 #  HitUv : [real2](../nada_base_types/real2.md)

> The uv texture coordinate at the intersection point, if applicable. Used with Reactive components.
> ```TS:Nada
> var HitUv : Real2


---  
 #  RayDirection : [real3](../nada_base_types/real3.md)

> Mouse Ray Direction.
> ```TS:Nada
> var RayDirection : Real3


---  
 #  RayStart : [real3](../nada_base_types/real3.md)

> Mouse Ray start.
> ```TS:Nada
> var RayStart : Real3


---  
 #  WorldRay : [ray](ray.md)

> The world mouse ray.
> ```TS:Nada
> var WorldRay : Ray


---  
 #  Methods


---  
 #  ToWorldPlane : [real3](../nada_base_types/real3.md)

> The world mouse position on any arbitrary plane.
> |Name|Type|Description|
> |---|---|---|
> |worldPlaneNormal|[real3](../nada_base_types/real3.md)| |
> |worldPlanePosition|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function ToWorldPlane(worldPlaneNormal : Real3, worldPlanePosition : Real3) : Real3
> ``` 


---  
 #  ToWorldViewPlane : [real3](../nada_base_types/real3.md)

> The world mouse position on the view plane at view depth.
> |Name|Type|Description|
> |---|---|---|
> |viewDepth|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function ToWorldViewPlane(viewDepth : Real) : Real3
> ``` 


---  
 #  ToWorldZPlane : [real3](../nada_base_types/real3.md)

> The world mouse position on the z plane at depth.
> |Name|Type|Description|
> |---|---|---|
> |worldDepth|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function ToWorldZPlane(worldDepth : Real) : Real3
> ``` 


---  
 

 
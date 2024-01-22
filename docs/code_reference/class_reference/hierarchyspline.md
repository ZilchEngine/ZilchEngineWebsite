 `Component` `Engine`



(NOTE) A spline that builds its control points from all child cogs that have Transforms.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ForceRebuild](hierarchyspline.md#forcerebuild-void)|[Closed](hierarchyspline.md#closed-zilch-engine-docum)|[component](component.md)| |
|[Constructor](hierarchyspline.md#hierarchyspline-void)|[DebugDrawSpline](hierarchyspline.md#debugdrawspline-zilch-eng)| | |
|[RebuildIfModified](hierarchyspline.md#rebuildifmodified-void)|[Error](hierarchyspline.md#error-zilch-engine-docume)| | |
| |[Spline](hierarchyspline.md#spline-zilch-engine-docum)| | |
| |[SplineColor](hierarchyspline.md#splinecolor-zilch-engine)| | |
| |[SplineType](hierarchyspline.md#splinetype-zilch-engine-d)| | |


 #  Properties


---  
 #  Closed : [boolean](../nada_base_types/boolean.md)

> Does the spline loop back on itself?
> ```TS:Nada
> var Closed : Boolean


---  
 #  DebugDrawSpline : [boolean](../nada_base_types/boolean.md)

> Should the spline draw every frame? Mainly used for debugging purposes.
> ```TS:Nada
> var DebugDrawSpline : Boolean


---  
 #  Error : [real](../nada_base_types/real.md)

> The max number of units that a line segment is allowed to deviate from the curve.
> ```TS:Nada
> var Error : Real


---  
 #  Spline : [spline](spline.md)

 `read-only`

> The internal spline data.
> ```TS:Nada
> var Spline : Spline


---  
 #  SplineColor : [real4](../nada_base_types/real4.md)

> What color should that spline be drawn with.
> ```TS:Nada
> var SplineColor : Real4


---  
 #  SplineType : [SplineType](../enum_reference.md#splinetype)

> The kind of spline (Linear, BSpline, CatmullRom). Determines how the control points affect the curve.
> ```TS:Nada
> var SplineType : SplineType


---  
 #  Methods


---  
 #  ForceRebuild : Void

> Forcibly rebuilds the baked points for the spline.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ForceRebuild()
> ``` 


---  
 #  HierarchySpline : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function HierarchySpline()
> ``` 


---  
 #  RebuildIfModified : Void

> Rebuild the baked points if there are any changes to the spline's control points. This should never need to be manually called.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function RebuildIfModified()
> ``` 


---  
 

 
 `Component` `Engine`



(NOTE) A spline that builds its control points from all child cogs that have Transforms.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ForceRebuild](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/hierarchyspline.md#forcerebuild-void)|[ Closed](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/hierarchyspline.md#closed-zilch-engine-docum)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)| |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/hierarchyspline.md#hierarchyspline-void)|[ DebugDrawSpline](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/hierarchyspline.md#debugdrawspline-zilch-eng)| | |
|[ RebuildIfModified](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/hierarchyspline.md#rebuildifmodified-void)|[ Error](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/hierarchyspline.md#error-zilch-engine-docume)| | |
| |[ Spline](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/hierarchyspline.md#spline-zilch-engine-docum)| | |
| |[ SplineColor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/hierarchyspline.md#splinecolor-zilch-engine)| | |
| |[ SplineType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/hierarchyspline.md#splinetype-zilch-engine-d)| | |


 #  Properties


---  
 #  Closed : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Does the spline loop back on itself?
> ``` lang=cpp, name=Nada
> var Closed : Boolean


---  
 #  DebugDrawSpline : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Should the spline draw every frame? Mainly used for debugging purposes.
> ``` lang=cpp, name=Nada
> var DebugDrawSpline : Boolean


---  
 #  Error : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The max number of units that a line segment is allowed to deviate from the curve.
> ``` lang=cpp, name=Nada
> var Error : Real


---  
 #  Spline : [spline](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spline.md)

 `read-only`

> The internal spline data.
> ``` lang=cpp, name=Nada
> var Spline : Spline


---  
 #  SplineColor : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

> What color should that spline be drawn with.
> ``` lang=cpp, name=Nada
> var SplineColor : Real4


---  
 #  SplineType : [SplineType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#splinetype)

> The kind of spline (Linear, BSpline, CatmullRom). Determines how the control points affect the curve.
> ``` lang=cpp, name=Nada
> var SplineType : SplineType


---  
 #  Methods


---  
 #  ForceRebuild : Void

> Forcibly rebuilds the baked points for the spline.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ForceRebuild()
> ``` 


---  
 #  HierarchySpline : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function HierarchySpline()
> ``` 


---  
 #  RebuildIfModified : Void

> Rebuild the baked points if there are any changes to the spline's control points. This should never need to be manually called.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function RebuildIfModified()
> ``` 


---  
 

 
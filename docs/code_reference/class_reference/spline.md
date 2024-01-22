 `Engine`

(NOTE) A spline built from control points. Bakes out the curve using an error term (distance from actual spline). Provides an interface to sample the curve at a given arc-length distance in order to provide constant speed interpolation.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Clone](spline.md#clone-zilch-engine-docume)|[BakedPoints](spline.md#bakedpoints-zilch-engine)|[referencecountedeventobject](referencecountedeventobject.md)| |
|[Create](spline.md#create-zilch-engine-docum)|[Closed](spline.md#closed-zilch-engine-docum)| | |
|[DebugDraw](spline.md#debugdraw-void)|[ControlPoints](spline.md#controlpoints-zilch-engin)| | |
|[ForceRebuild](spline.md#forcerebuild-void)|[Error](spline.md#error-zilch-engine-docume)| | |
|[RebuildIfModified](spline.md#rebuildifmodified-void)|[SplineType](spline.md#splinetype-zilch-engine-d)| | |
|[SampleDistance](spline.md#sampledistance-zilch-engi)|[TotalDistance](spline.md#totaldistance-zilch-engin)| | |
|[SampleNormalized](spline.md#samplenormalized-zilch-en)| | | |


 #  Properties


---  
 #  BakedPoints : [splinebakedpoints](splinebakedpoints.md)

 `read-only`

> The read-only curve points baked out to line segments using the provided error.
> ```TS:Nada
> var BakedPoints : SplineBakedPoints


---  
 #  Closed : [boolean](../nada_base_types/boolean.md)

> Does the spline loop back on itself?
> ```TS:Nada
> var Closed : Boolean


---  
 #  ControlPoints : [splinecontrolpoints](splinecontrolpoints.md)

 `read-only`

> The control points used to bake out the curve.
> ```TS:Nada
> var ControlPoints : SplineControlPoints


---  
 #  Error : [real](../nada_base_types/real.md)

> The max number of units that a line segment is allowed to deviate from the curve.
> ```TS:Nada
> var Error : Real


---  
 #  SplineType : [SplineType](../enum_reference.md#splinetype)

> The kind of spline (Linear, BSpline, CatmullRom). Determines how the control points affect the curve.
> ```TS:Nada
> var SplineType : SplineType


---  
 #  TotalDistance : [real](../nada_base_types/real.md)

 `read-only`

> The total arc-length of the curve. Use to normalize the curve if you wish.
> ```TS:Nada
> var TotalDistance : Real


---  
 #  Methods


---  
 #  Clone : [spline](spline.md)

> Create a new copy of this spline.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Clone() : Spline
> ``` 


---  
 #  Create : [spline](spline.md)

 `static`

> Create a new instance of a spline.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Create() : Spline
> ``` 


---  
 #  DebugDraw : Void

> Draw the baked points of the curve with the provided color.
> |Name|Type|Description|
> |---|---|---|
> |color|[real4](../nada_base_types/real4.md)| |
> ```TS:Nada
> function DebugDraw(color : Real4)
> ``` 


---  
 #  ForceRebuild : Void

> Forcibly rebuild the baked points from the control points.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ForceRebuild()
> ``` 


---  
 #  RebuildIfModified : Void

> Rebuild the baked points from the control points if they have changed. Should not need to be manually called unless the user wants to control the timing when the points are baked.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function RebuildIfModified()
> ``` 


---  
 #  SampleDistance : [splinesampledata](splinesampledata.md)

> Samples the curve at a given arc-length distance.
> |Name|Type|Description|
> |---|---|---|
> |distance|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function SampleDistance(distance : Real) : SplineSampleData
> ``` 


---  
 #  SampleNormalized : [splinesampledata](splinesampledata.md)

> Samples the curve with a time in the range of [0, 1].
> |Name|Type|Description|
> |---|---|---|
> |time|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function SampleNormalized(time : Real) : SplineSampleData
> ``` 


---  
 

 
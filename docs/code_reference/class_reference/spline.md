 `Engine`

(NOTE) A spline built from control points. Bakes out the curve using an error term (distance from actual spline). Provides an interface to sample the curve at a given arc-length distance in order to provide constant speed interpolation.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Clone](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spline.md#clone-zilch-engine-docume)|[ BakedPoints](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spline.md#bakedpoints-zilch-engine)|[referencecountedeventobject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/referencecountedeventobject.md)| |
|[ Create](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spline.md#create-zilch-engine-docum)|[ Closed](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spline.md#closed-zilch-engine-docum)| | |
|[ DebugDraw](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spline.md#debugdraw-void)|[ ControlPoints](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spline.md#controlpoints-zilch-engin)| | |
|[ ForceRebuild](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spline.md#forcerebuild-void)|[ Error](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spline.md#error-zilch-engine-docume)| | |
|[ RebuildIfModified](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spline.md#rebuildifmodified-void)|[ SplineType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spline.md#splinetype-zilch-engine-d)| | |
|[ SampleDistance](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spline.md#sampledistance-zilch-engi)|[ TotalDistance](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spline.md#totaldistance-zilch-engin)| | |
|[ SampleNormalized](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spline.md#samplenormalized-zilch-en)| | | |


 #  Properties


---  
 #  BakedPoints : [splinebakedpoints](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/splinebakedpoints.md)

 `read-only`

> The read-only curve points baked out to line segments using the provided error.
> ``` lang=cpp, name=Nada
> var BakedPoints : SplineBakedPoints


---  
 #  Closed : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Does the spline loop back on itself?
> ``` lang=cpp, name=Nada
> var Closed : Boolean


---  
 #  ControlPoints : [splinecontrolpoints](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/splinecontrolpoints.md)

 `read-only`

> The control points used to bake out the curve.
> ``` lang=cpp, name=Nada
> var ControlPoints : SplineControlPoints


---  
 #  Error : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The max number of units that a line segment is allowed to deviate from the curve.
> ``` lang=cpp, name=Nada
> var Error : Real


---  
 #  SplineType : [SplineType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#splinetype)

> The kind of spline (Linear, BSpline, CatmullRom). Determines how the control points affect the curve.
> ``` lang=cpp, name=Nada
> var SplineType : SplineType


---  
 #  TotalDistance : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

 `read-only`

> The total arc-length of the curve. Use to normalize the curve if you wish.
> ``` lang=cpp, name=Nada
> var TotalDistance : Real


---  
 #  Methods


---  
 #  Clone : [spline](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spline.md)

> Create a new copy of this spline.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Clone() : Spline
> ``` 


---  
 #  Create : [spline](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spline.md)

 `static`

> Create a new instance of a spline.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Create() : Spline
> ``` 


---  
 #  DebugDraw : Void

> Draw the baked points of the curve with the provided color.
> |Name|Type|Description|
> |---|---|---|
> |color|[real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)| |
> ``` lang=cpp, name=Nada
> function DebugDraw(color : Real4)
> ``` 


---  
 #  ForceRebuild : Void

> Forcibly rebuild the baked points from the control points.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ForceRebuild()
> ``` 


---  
 #  RebuildIfModified : Void

> Rebuild the baked points from the control points if they have changed. Should not need to be manually called unless the user wants to control the timing when the points are baked.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function RebuildIfModified()
> ``` 


---  
 #  SampleDistance : [splinesampledata](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/splinesampledata.md)

> Samples the curve at a given arc-length distance.
> |Name|Type|Description|
> |---|---|---|
> |distance|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function SampleDistance(distance : Real) : SplineSampleData
> ``` 


---  
 #  SampleNormalized : [splinesampledata](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/splinesampledata.md)

> Samples the curve with a time in the range of [0, 1].
> |Name|Type|Description|
> |---|---|---|
> |time|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function SampleNormalized(time : Real) : SplineSampleData
> ``` 


---  
 

 
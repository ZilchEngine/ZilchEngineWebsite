 `Engine`

(NOTE) Control points for the Spline class. Modifying this will cause the spline to be marked as modified to rebuild the baked curve when needed.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Add](splinecontrolpoints.md#add-void)|[Count](splinecontrolpoints.md#count-zilch-engine-docume)|[safeid32object](safeid32object.md)| |
|[Clear](splinecontrolpoints.md#clear-void)| | | |
|[Get](splinecontrolpoints.md#get-zilch-engine-document)| | | |
|[Set](splinecontrolpoints.md#set-void)| | | |


 #  Properties


---  
 #  Count : [integer](../nada_base_types/integer.md)

 `read-only`

> The number of control points contained.
> ```TS:Nada
> var Count : Integer


---  
 #  Methods


---  
 #  Add : Void

> Add a new point to the end of the array.
> |Name|Type|Description|
> |---|---|---|
> |controlPoint|[splinecontrolpoint](splinecontrolpoint.md)| |
> ```TS:Nada
> function Add(controlPoint : SplineControlPoint)
> ``` 


---  
 #  Clear : Void

> Clear all control points.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Clear()
> ``` 


---  
 #  Get : [splinecontrolpoint](splinecontrolpoint.md)

> Get the control point at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function Get(index : Integer) : SplineControlPoint
> ``` 


---  
 #  Set : Void

> Sets the control point at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> |value|[splinecontrolpoint](splinecontrolpoint.md)| |
> ```TS:Nada
> function Set(index : Integer, value : SplineControlPoint)
> ``` 


---  
 

 
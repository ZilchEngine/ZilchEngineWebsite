 `Engine`

(NOTE) Control points for the Spline class. Modifying this will cause the spline to be marked as modified to rebuild the baked curve when needed.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Add](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/splinecontrolpoints.md#add-void)|[ Count](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/splinecontrolpoints.md#count-zilch-engine-docume)|[safeid32object](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/safeid32object.md)| |
|[ Clear](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/splinecontrolpoints.md#clear-void)| | | |
|[ Get](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/splinecontrolpoints.md#get-zilch-engine-document)| | | |
|[ Set](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/splinecontrolpoints.md#set-void)| | | |


 #  Properties


---  
 #  Count : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> The number of control points contained.
> ``` lang=cpp, name=Nada
> var Count : Integer


---  
 #  Methods


---  
 #  Add : Void

> Add a new point to the end of the array.
> |Name|Type|Description|
> |---|---|---|
> |controlPoint|[splinecontrolpoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/splinecontrolpoint.md)| |
> ``` lang=cpp, name=Nada
> function Add(controlPoint : SplineControlPoint)
> ``` 


---  
 #  Clear : Void

> Clear all control points.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Clear()
> ``` 


---  
 #  Get : [splinecontrolpoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/splinecontrolpoint.md)

> Get the control point at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Get(index : Integer) : SplineControlPoint
> ``` 


---  
 #  Set : Void

> Sets the control point at the given index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |value|[splinecontrolpoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/splinecontrolpoint.md)| |
> ``` lang=cpp, name=Nada
> function Set(index : Integer, value : SplineControlPoint)
> ``` 


---  
 

 
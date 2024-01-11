 `Component` `Gameplay`



|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Capture](mousecapture.md#capture-zilch-engine-docu)|[ IsCaptured](mousecapture.md#iscaptured-zilch-engine-d)|[component](component.md)| |
|[ Constructor](mousecapture.md#mousecapture-void)| | | |
|[ ReleaseCapture](mousecapture.md#releasecapture-void)| | | |


 #  Properties


---  
 #  IsCaptured : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Returns whether or not this has an active mouse capture.
> ``` lang=cpp, name=Nada
> var IsCaptured : Boolean


---  
 #  Methods


---  
 #  Capture : [boolean](../nada_base_types/boolean.md)

> Starts the mouse manipulation. All mouse events will now only go to the owner of this Component. Returns whether or not the manipulation can be started.
> |Name|Type|Description|
> |---|---|---|
> |e|[viewportmouseevent](viewportmouseevent.md)| |
> ``` lang=cpp, name=Nada
> function Capture(e : ViewportMouseEvent) : Boolean
> ``` 


---  
 #  MouseCapture : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function MouseCapture()
> ``` 


---  
 #  ReleaseCapture : Void

> Releases the mouse manipulation.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ReleaseCapture()
> ``` 


---  
 #  ReleaseCapture : Void

> Releases the mouse manipulation.
> |Name|Type|Description|
> |---|---|---|
> |e|[viewportmouseevent](viewportmouseevent.md)| |
> ``` lang=cpp, name=Nada
> function ReleaseCapture(e : ViewportMouseEvent)
> ``` 


---  
 

 
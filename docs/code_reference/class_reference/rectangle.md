 `Engine`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Contains](rectangle.md#contains-zilch-engine-doc)|[ Bottom](rectangle.md#bottom-zilch-engine-docum)| | |
|[ Expand](rectangle.md#expand-void)|[ BottomLeft](rectangle.md#bottomleft-zilch-engine-d)| | |
|[ GetCardinalLocation](rectangle.md#getcardinallocation-zero)|[ BottomRight](rectangle.md#bottomright-zilch-engine)| | |
|[ GetLocation](rectangle.md#getlocation-zilch-engine)|[ Center](rectangle.md#center-zilch-engine-docum)| | |
|[ Overlap](rectangle.md#overlap-zilch-engine-docu)|[ Left](rectangle.md#left-zilch-engine-documen)| | |
|[ Overlaps](rectangle.md#overlaps-zilch-engine-doc)|[ Max](rectangle.md#max-zilch-engine-document)| | |
|[ RemoveThickness](rectangle.md#removethickness-void)|[ Min](rectangle.md#min-zilch-engine-document)| | |
|[ ResizeToPoint](rectangle.md#resizetopoint-void)|[ Right](rectangle.md#right-zilch-engine-docume)| | |
|[ SetLocation](rectangle.md#setlocation-void)|[ Size](rectangle.md#size-zilch-engine-documen)| | |
|[ Transform](rectangle.md#transform-void)|[ Top](rectangle.md#top-zilch-engine-document)| | |
|[ Transformed](rectangle.md#transformed-zilch-engine)|[ TopLeft](rectangle.md#topleft-zilch-engine-docu)| | |
| |[ TopRight](rectangle.md#topright-zilch-engine-doc)| | |


 #  Properties


---  
 #  Bottom : [real](../nada_base_types/real.md)

> 
> ``` lang=cpp, name=Nada
> var Bottom : Real


---  
 #  BottomLeft : [real2](../nada_base_types/real2.md)

> 
> ``` lang=cpp, name=Nada
> var BottomLeft : Real2


---  
 #  BottomRight : [real2](../nada_base_types/real2.md)

> 
> ``` lang=cpp, name=Nada
> var BottomRight : Real2


---  
 #  Center : [real2](../nada_base_types/real2.md)

> 
> ``` lang=cpp, name=Nada
> var Center : Real2


---  
 #  Left : [real](../nada_base_types/real.md)

> 
> ``` lang=cpp, name=Nada
> var Left : Real


---  
 #  Max : [real2](../nada_base_types/real2.md)

> 
> ``` lang=cpp, name=Nada
> var Max : Real2


---  
 #  Min : [real2](../nada_base_types/real2.md)

> 
> ``` lang=cpp, name=Nada
> var Min : Real2


---  
 #  Right : [real](../nada_base_types/real.md)

> 
> ``` lang=cpp, name=Nada
> var Right : Real


---  
 #  Size : [real2](../nada_base_types/real2.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Size : Real2


---  
 #  Top : [real](../nada_base_types/real.md)

> 
> ``` lang=cpp, name=Nada
> var Top : Real


---  
 #  TopLeft : [real2](../nada_base_types/real2.md)

> 
> ``` lang=cpp, name=Nada
> var TopLeft : Real2


---  
 #  TopRight : [real2](../nada_base_types/real2.md)

> 
> ``` lang=cpp, name=Nada
> var TopRight : Real2


---  
 #  Methods


---  
 #  Contains : [boolean](../nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real2](../nada_base_types/real2.md)| |
> ``` lang=cpp, name=Nada
> function Contains(p0 : Real2) : Boolean
> ``` 


---  
 #  Contains : [boolean](../nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[rectangle](rectangle.md)| |
> ``` lang=cpp, name=Nada
> function Contains(p0 : Rectangle) : Boolean
> ``` 


---  
 #  Expand : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real2](../nada_base_types/real2.md)| |
> ``` lang=cpp, name=Nada
> function Expand(p0 : Real2)
> ``` 


---  
 #  GetCardinalLocation : [real](../nada_base_types/real.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[Location](../enum_reference.md#location)| |
> ``` lang=cpp, name=Nada
> function GetCardinalLocation(p0 : Location) : Real
> ``` 


---  
 #  GetLocation : [real2](../nada_base_types/real2.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[Location](../enum_reference.md#location)| |
> ``` lang=cpp, name=Nada
> function GetLocation(p0 : Location) : Real2
> ``` 


---  
 #  Overlap : [boolean](../nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[rectangle](rectangle.md)| |
> ``` lang=cpp, name=Nada
> function Overlap(p0 : Rectangle) : Boolean
> ``` 


---  
 #  Overlaps : [boolean](../nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[rectangle](rectangle.md)| |
> ``` lang=cpp, name=Nada
> function Overlaps(p0 : Rectangle) : Boolean
> ``` 


---  
 #  RemoveThickness : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[thickness](thickness.md)| |
> ``` lang=cpp, name=Nada
> function RemoveThickness(p0 : Thickness)
> ``` 


---  
 #  ResizeToPoint : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[Location](../enum_reference.md#location)| |
> |p1|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function ResizeToPoint(p0 : Location, p1 : Real)
> ``` 


---  
 #  ResizeToPoint : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[Location](../enum_reference.md#location)| |
> |p1|[real2](../nada_base_types/real2.md)| |
> ``` lang=cpp, name=Nada
> function ResizeToPoint(p0 : Location, p1 : Real2)
> ``` 


---  
 #  ResizeToPoint : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[Location](../enum_reference.md#location)| |
> |p1|[real2](../nada_base_types/real2.md)| |
> |p2|[real2](../nada_base_types/real2.md)| |
> ``` lang=cpp, name=Nada
> function ResizeToPoint(p0 : Location, p1 : Real2, p2 : Real2)
> ``` 


---  
 #  SetLocation : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[Location](../enum_reference.md#location)| |
> |p1|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function SetLocation(p0 : Location, p1 : Real)
> ``` 


---  
 #  SetLocation : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[Location](../enum_reference.md#location)| |
> |p1|[real2](../nada_base_types/real2.md)| |
> ``` lang=cpp, name=Nada
> function SetLocation(p0 : Location, p1 : Real2)
> ``` 


---  
 #  Transform : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real2x2](../nada_base_types/real2x2.md)| |
> ``` lang=cpp, name=Nada
> function Transform(p0 : Real2x2)
> ``` 


---  
 #  Transform : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real3x3](../nada_base_types/real3x3.md)| |
> ``` lang=cpp, name=Nada
> function Transform(p0 : Real3x3)
> ``` 


---  
 #  Transform : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real4x4](../nada_base_types/real4x4.md)| |
> ``` lang=cpp, name=Nada
> function Transform(p0 : Real4x4)
> ``` 


---  
 #  Transformed : [rectangle](rectangle.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real2x2](../nada_base_types/real2x2.md)| |
> ``` lang=cpp, name=Nada
> function Transformed(p0 : Real2x2) : Rectangle
> ``` 


---  
 #  Transformed : [rectangle](rectangle.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real3x3](../nada_base_types/real3x3.md)| |
> ``` lang=cpp, name=Nada
> function Transformed(p0 : Real3x3) : Rectangle
> ``` 


---  
 #  Transformed : [rectangle](rectangle.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[real4x4](../nada_base_types/real4x4.md)| |
> ``` lang=cpp, name=Nada
> function Transformed(p0 : Real4x4) : Rectangle
> ``` 


---  
 

 
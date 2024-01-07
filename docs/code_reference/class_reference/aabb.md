 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md#aabb-void)|[ Center](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md#center-zilch-engine-docum)| | |
|[ ContainsPoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md#containspoint-zilch-engin)|[ Extents](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md#extents-zilch-engine-docu)| | |
|[ Expand](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md#expand-void)|[ HalfExtents](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md#halfextents-zilch-engine)| | |
|[ Overlap](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md#overlap-zilch-engine-docu)|[ Max](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md#max-zilch-engine-document)| | |
|[ Overlaps](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md#overlaps-zilch-engine-doc)|[ Min](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md#min-zilch-engine-document)| | |
|[ Set](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md#set-void)|[ SurfaceArea](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md#surfacearea-zilch-engine)| | |
|[ SetInvalid](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md#setinvalid-void)|[ Volume](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md#volume-zilch-engine-docum)| | |
|[ ZeroOut](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md#zeroout-void)| | | |


 #  Properties


---  
 #  Center : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> 
> ``` lang=cpp, name=Nada
> var Center : Real3


---  
 #  Extents : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> 
> ``` lang=cpp, name=Nada
> var Extents : Real3


---  
 #  HalfExtents : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> 
> ``` lang=cpp, name=Nada
> var HalfExtents : Real3


---  
 #  Max : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> 
> ``` lang=cpp, name=Nada
> var Max : Real3


---  
 #  Min : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> 
> ``` lang=cpp, name=Nada
> var Min : Real3


---  
 #  SurfaceArea : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var SurfaceArea : Real


---  
 #  Volume : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Volume : Real


---  
 #  Methods


---  
 #  Aabb : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Aabb()
> ``` 


---  
 #  Aabb : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[aabb](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md)| |
> ``` lang=cpp, name=Nada
> function Aabb(p0 : Aabb)
> ``` 


---  
 #  Aabb : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |center|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |halfExtents|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function Aabb(center : Real3, halfExtents : Real3)
> ``` 


---  
 #  ContainsPoint : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Does this aabb contain the given point?
> |Name|Type|Description|
> |---|---|---|
> |p0|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function ContainsPoint(p0 : Real3) : Boolean
> ``` 


---  
 #  Expand : Void

> Expand this aabb to contain the given aabb.
> |Name|Type|Description|
> |---|---|---|
> |p0|[aabb](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md)| |
> ``` lang=cpp, name=Nada
> function Expand(p0 : Aabb)
> ``` 


---  
 #  Expand : [aabb](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md)

 `static`

> Creates an aabb that contains the two given aabbs.
> |Name|Type|Description|
> |---|---|---|
> |p0|[aabb](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md)| |
> |p1|[aabb](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md)| |
> ``` lang=cpp, name=Nada
> function Expand(p0 : Aabb, p1 : Aabb) : Aabb
> ``` 


---  
 #  Expand : [aabb](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md)

 `static`

> Creates an aabb that contains the given aabb and point.
> |Name|Type|Description|
> |---|---|---|
> |p0|[aabb](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md)| |
> |p1|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function Expand(p0 : Aabb, p1 : Real3) : Aabb
> ``` 


---  
 #  Expand : Void

> Expand this aabb to contain the given point.
> |Name|Type|Description|
> |---|---|---|
> |p0|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function Expand(p0 : Real3)
> ``` 


---  
 #  Overlap : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> This function is deprecated. Use Overlaps instead
> |Name|Type|Description|
> |---|---|---|
> |p0|[aabb](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md)| |
> ``` lang=cpp, name=Nada
> function Overlap(p0 : Aabb) : Boolean
> ``` 


---  
 #  Overlaps : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Does this aabb overlap/intersect the given aabb?
> |Name|Type|Description|
> |---|---|---|
> |p0|[aabb](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md)| |
> ``` lang=cpp, name=Nada
> function Overlaps(p0 : Aabb) : Boolean
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function Set(point : Real3)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |center|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |halfExtents|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function Set(center : Real3, halfExtents : Real3)
> ``` 


---  
 #  SetInvalid : Void

> Sets this aabb to an invalid aabb (Real3.PositiveMax, Real3.NegativeMin)). This also makes expansion easier.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function SetInvalid()
> ``` 


---  
 #  ZeroOut : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ZeroOut()
> ``` 


---  
 

 
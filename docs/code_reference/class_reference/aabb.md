 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](aabb.md#aabb-void)|[Center](aabb.md#center-zilch-engine-docum)| | |
|[ContainsPoint](aabb.md#containspoint-zilch-engin)|[Extents](aabb.md#extents-zilch-engine-docu)| | |
|[Expand](aabb.md#expand-void)|[HalfExtents](aabb.md#halfextents-zilch-engine)| | |
|[Overlap](aabb.md#overlap-zilch-engine-docu)|[Max](aabb.md#max-zilch-engine-document)| | |
|[Overlaps](aabb.md#overlaps-zilch-engine-doc)|[Min](aabb.md#min-zilch-engine-document)| | |
|[Set](aabb.md#set-void)|[SurfaceArea](aabb.md#surfacearea-zilch-engine)| | |
|[SetInvalid](aabb.md#setinvalid-void)|[Volume](aabb.md#volume-zilch-engine-docum)| | |
|[ZeroOut](aabb.md#zeroout-void)| | | |


 #  Properties


---  
 #  Center : [real3](../nada_base_types/real3.md)

> 
> ```TS:Nada
> var Center : Real3


---  
 #  Extents : [real3](../nada_base_types/real3.md)

> 
> ```TS:Nada
> var Extents : Real3


---  
 #  HalfExtents : [real3](../nada_base_types/real3.md)

> 
> ```TS:Nada
> var HalfExtents : Real3


---  
 #  Max : [real3](../nada_base_types/real3.md)

> 
> ```TS:Nada
> var Max : Real3


---  
 #  Min : [real3](../nada_base_types/real3.md)

> 
> ```TS:Nada
> var Min : Real3


---  
 #  SurfaceArea : [real](../nada_base_types/real.md)

 `read-only`

> 
> ```TS:Nada
> var SurfaceArea : Real


---  
 #  Volume : [real](../nada_base_types/real.md)

 `read-only`

> 
> ```TS:Nada
> var Volume : Real


---  
 #  Methods


---  
 #  Aabb : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Aabb()
> ``` 


---  
 #  Aabb : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[aabb](aabb.md)| |
> ```TS:Nada
> function Aabb(p0 : Aabb)
> ``` 


---  
 #  Aabb : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |center|[real3](../nada_base_types/real3.md)| |
> |halfExtents|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function Aabb(center : Real3, halfExtents : Real3)
> ``` 


---  
 #  ContainsPoint : [boolean](../nada_base_types/boolean.md)

> Does this aabb contain the given point?
> |Name|Type|Description|
> |---|---|---|
> |p0|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function ContainsPoint(p0 : Real3) : Boolean
> ``` 


---  
 #  Expand : Void

> Expand this aabb to contain the given aabb.
> |Name|Type|Description|
> |---|---|---|
> |p0|[aabb](aabb.md)| |
> ```TS:Nada
> function Expand(p0 : Aabb)
> ``` 


---  
 #  Expand : [aabb](aabb.md)

 `static`

> Creates an aabb that contains the two given aabbs.
> |Name|Type|Description|
> |---|---|---|
> |p0|[aabb](aabb.md)| |
> |p1|[aabb](aabb.md)| |
> ```TS:Nada
> function Expand(p0 : Aabb, p1 : Aabb) : Aabb
> ``` 


---  
 #  Expand : [aabb](aabb.md)

 `static`

> Creates an aabb that contains the given aabb and point.
> |Name|Type|Description|
> |---|---|---|
> |p0|[aabb](aabb.md)| |
> |p1|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function Expand(p0 : Aabb, p1 : Real3) : Aabb
> ``` 


---  
 #  Expand : Void

> Expand this aabb to contain the given point.
> |Name|Type|Description|
> |---|---|---|
> |p0|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function Expand(p0 : Real3)
> ``` 


---  
 #  Overlap : [boolean](../nada_base_types/boolean.md)

> This function is deprecated. Use Overlaps instead
> |Name|Type|Description|
> |---|---|---|
> |p0|[aabb](aabb.md)| |
> ```TS:Nada
> function Overlap(p0 : Aabb) : Boolean
> ``` 


---  
 #  Overlaps : [boolean](../nada_base_types/boolean.md)

> Does this aabb overlap/intersect the given aabb?
> |Name|Type|Description|
> |---|---|---|
> |p0|[aabb](aabb.md)| |
> ```TS:Nada
> function Overlaps(p0 : Aabb) : Boolean
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function Set(point : Real3)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |center|[real3](../nada_base_types/real3.md)| |
> |halfExtents|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function Set(center : Real3, halfExtents : Real3)
> ``` 


---  
 #  SetInvalid : Void

> Sets this aabb to an invalid aabb (Real3.PositiveMax, Real3.NegativeMin)). This also makes expansion easier.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function SetInvalid()
> ``` 


---  
 #  ZeroOut : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ZeroOut()
> ``` 


---  
 

 
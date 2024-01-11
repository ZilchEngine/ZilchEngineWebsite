 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Expand](sphere.md#expand-void)|[ Center](sphere.md#center-zilch-engine-docum)| | |
|[ Overlap](sphere.md#overlap-zilch-engine-docu)|[ Radius](sphere.md#radius-zilch-engine-docum)| | |
|[ Overlaps](sphere.md#overlaps-zilch-engine-doc)|[ SurfaceArea](sphere.md#surfacearea-zilch-engine)| | |
|[ Constructor](sphere.md#sphere-void)|[ Volume](sphere.md#volume-zilch-engine-docum)| | |


 #  Properties


---  
 #  Center : [real3](../nada_base_types/real3.md)

> 
> ``` lang=cpp, name=Nada
> var Center : Real3


---  
 #  Radius : [real](../nada_base_types/real.md)

> 
> ``` lang=cpp, name=Nada
> var Radius : Real


---  
 #  SurfaceArea : [real](../nada_base_types/real.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var SurfaceArea : Real


---  
 #  Volume : [real](../nada_base_types/real.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Volume : Real


---  
 #  Methods


---  
 #  Expand : Void

> Expand this sphere to contain the given point.
> |Name|Type|Description|
> |---|---|---|
> |p0|[real3](../nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function Expand(p0 : Real3)
> ``` 


---  
 #  Expand : [sphere](sphere.md)

 `static`

> Creates a sphere that contains the given sphere and point.
> |Name|Type|Description|
> |---|---|---|
> |p0|[sphere](sphere.md)| |
> |p1|[real3](../nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function Expand(p0 : Sphere, p1 : Real3) : Sphere
> ``` 


---  
 #  Overlap : [boolean](../nada_base_types/boolean.md)

> This function is deprecated. Use Overlaps instead
> |Name|Type|Description|
> |---|---|---|
> |p0|[sphere](sphere.md)| |
> ``` lang=cpp, name=Nada
> function Overlap(p0 : Sphere) : Boolean
> ``` 


---  
 #  Overlaps : [boolean](../nada_base_types/boolean.md)

> Does this sphere overlap/intersect the given sphere?
> |Name|Type|Description|
> |---|---|---|
> |p0|[sphere](sphere.md)| |
> ``` lang=cpp, name=Nada
> function Overlaps(p0 : Sphere) : Boolean
> ``` 


---  
 #  Sphere : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Sphere()
> ``` 


---  
 #  Sphere : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |center|[real3](../nada_base_types/real3.md)| |
> |radius|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function Sphere(center : Real3, radius : Real)
> ``` 


---  
 #  Sphere : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[sphere](sphere.md)| |
> ``` lang=cpp, name=Nada
> function Sphere(p0 : Sphere)
> ``` 


---  
 

 
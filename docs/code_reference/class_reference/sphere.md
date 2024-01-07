 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Expand](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sphere.md#expand-void)|[ Center](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sphere.md#center-zilch-engine-docum)| | |
|[ Overlap](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sphere.md#overlap-zilch-engine-docu)|[ Radius](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sphere.md#radius-zilch-engine-docum)| | |
|[ Overlaps](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sphere.md#overlaps-zilch-engine-doc)|[ SurfaceArea](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sphere.md#surfacearea-zilch-engine)| | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sphere.md#sphere-void)|[ Volume](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sphere.md#volume-zilch-engine-docum)| | |


 #  Properties


---  
 #  Center : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> 
> ``` lang=cpp, name=Nada
> var Center : Real3


---  
 #  Radius : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> 
> ``` lang=cpp, name=Nada
> var Radius : Real


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
 #  Expand : Void

> Expand this sphere to contain the given point.
> |Name|Type|Description|
> |---|---|---|
> |p0|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function Expand(p0 : Real3)
> ``` 


---  
 #  Expand : [sphere](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sphere.md)

 `static`

> Creates a sphere that contains the given sphere and point.
> |Name|Type|Description|
> |---|---|---|
> |p0|[sphere](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sphere.md)| |
> |p1|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function Expand(p0 : Sphere, p1 : Real3) : Sphere
> ``` 


---  
 #  Overlap : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> This function is deprecated. Use Overlaps instead
> |Name|Type|Description|
> |---|---|---|
> |p0|[sphere](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sphere.md)| |
> ``` lang=cpp, name=Nada
> function Overlap(p0 : Sphere) : Boolean
> ``` 


---  
 #  Overlaps : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Does this sphere overlap/intersect the given sphere?
> |Name|Type|Description|
> |---|---|---|
> |p0|[sphere](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sphere.md)| |
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
> |center|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |radius|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function Sphere(center : Real3, radius : Real)
> ``` 


---  
 #  Sphere : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[sphere](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sphere.md)| |
> ``` lang=cpp, name=Nada
> function Sphere(p0 : Sphere)
> ``` 


---  
 

 
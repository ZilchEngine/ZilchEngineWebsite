 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetPoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ray.md#getpoint-zilch-engine-doc)|[ Direction](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ray.md#direction-zilch-engine-do)| | |
|[ GetTValue](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ray.md#gettvalue-zilch-engine-do)|[ Start](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ray.md#start-zilch-engine-docume)| | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ray.md#ray-void)| | | |


 #  Properties


---  
 #  Direction : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> 
> ``` lang=cpp, name=Nada
> var Direction : Real3


---  
 #  Start : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> 
> ``` lang=cpp, name=Nada
> var Start : Real3


---  
 #  Methods


---  
 #  GetPoint : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Returns the point at the given t-value.
> |Name|Type|Description|
> |---|---|---|
> |tValue|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function GetPoint(tValue : Real) : Real3
> ``` 


---  
 #  GetTValue : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Returns the t-value that would result in the given point projected onto the ray.
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function GetTValue(point : Real3) : Real
> ``` 


---  
 #  Ray : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Ray()
> ``` 


---  
 #  Ray : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[ray](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ray.md)| |
> ``` lang=cpp, name=Nada
> function Ray(p0 : Ray)
> ``` 


---  
 #  Ray : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |start|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |direction|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function Ray(start : Real3, direction : Real3)
> ``` 


---  
 

 
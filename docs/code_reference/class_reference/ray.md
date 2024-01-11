 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetPoint](ray.md#getpoint-zilch-engine-doc)|[ Direction](ray.md#direction-zilch-engine-do)| | |
|[ GetTValue](ray.md#gettvalue-zilch-engine-do)|[ Start](ray.md#start-zilch-engine-docume)| | |
|[ Constructor](ray.md#ray-void)| | | |


 #  Properties


---  
 #  Direction : [real3](../nada_base_types/real3.md)

> 
> ```TS:Nada
> var Direction : Real3


---  
 #  Start : [real3](../nada_base_types/real3.md)

> 
> ```TS:Nada
> var Start : Real3


---  
 #  Methods


---  
 #  GetPoint : [real3](../nada_base_types/real3.md)

> Returns the point at the given t-value.
> |Name|Type|Description|
> |---|---|---|
> |tValue|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function GetPoint(tValue : Real) : Real3
> ``` 


---  
 #  GetTValue : [real](../nada_base_types/real.md)

> Returns the t-value that would result in the given point projected onto the ray.
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function GetTValue(point : Real3) : Real
> ``` 


---  
 #  Ray : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Ray()
> ``` 


---  
 #  Ray : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[ray](ray.md)| |
> ```TS:Nada
> function Ray(p0 : Ray)
> ``` 


---  
 #  Ray : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |start|[real3](../nada_base_types/real3.md)| |
> |direction|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function Ray(start : Real3, direction : Real3)
> ``` 


---  
 

 
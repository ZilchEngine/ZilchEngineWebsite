 `Geometry`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](plane.md#plane-void)|[ Data](plane.md#data-zilch-engine-documen)| | |
|[ Set](plane.md#set-void)|[ Distance](plane.md#distance-zilch-engine-doc)| | |
| |[ Normal](plane.md#normal-zilch-engine-docum)| | |


 #  Properties


---  
 #  Data : [real4](../nada_base_types/real4.md)

> 
> ```TS:Nada
> var Data : Real4


---  
 #  Distance : [real](../nada_base_types/real.md)

 `read-only`

> 
> ```TS:Nada
> var Distance : Real


---  
 #  Normal : [real3](../nada_base_types/real3.md)

 `read-only`

> 
> ```TS:Nada
> var Normal : Real3


---  
 #  Methods


---  
 #  Plane : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Plane()
> ``` 


---  
 #  Plane : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[plane](plane.md)| |
> ```TS:Nada
> function Plane(p0 : Plane)
> ``` 


---  
 #  Plane : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |normal|[real3](../nada_base_types/real3.md)| |
> |point|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function Plane(normal : Real3, point : Real3)
> ``` 


---  
 #  Plane : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |data|[real4](../nada_base_types/real4.md)| |
> ```TS:Nada
> function Plane(data : Real4)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |normal|[real3](../nada_base_types/real3.md)| |
> |point|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function Set(normal : Real3, point : Real3)
> ``` 


---  
 #  Set : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |data|[real4](../nada_base_types/real4.md)| |
> ```TS:Nada
> function Set(data : Real4)
> ``` 


---  
 

 
 `Physics`

(NOTE) A result from a cast operation on a PhysicsSpace.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](castresult.md#castresult-void)|[ Collider](castresult.md#collider-zilch-engine-doc)| | |
|[ GetLocalPosition](castresult.md#getlocalposition-zilch-en)|[ Distance](castresult.md#distance-zilch-engine-doc)| | |
| |[ Normal](castresult.md#normal-zilch-engine-docum)| | |
| |[ ObjectHit](castresult.md#objecthit-zilch-engine-do)| | |
| |[ WorldPosition](castresult.md#worldposition-zilch-engin)| | |


 #  Properties


---  
 #  Collider : [collider](collider.md)

 `read-only`

> The collider hit by the cast.
> ``` lang=cpp, name=Nada
> var Collider : Collider


---  
 #  Distance : [real](../nada_base_types/real.md)

 `read-only`

> The distance from the ray/segment start to the point of intersection. Invalid on a volume cast.
> ``` lang=cpp, name=Nada
> var Distance : Real


---  
 #  Normal : [real3](../nada_base_types/real3.md)

 `read-only`

> The normal of the object at the intersection point (world space). Invalid on a volume cast.
> ``` lang=cpp, name=Nada
> var Normal : Real3


---  
 #  ObjectHit : [cog](cog.md)

 `read-only`

> The cog hit by the cast.
> ``` lang=cpp, name=Nada
> var ObjectHit : Cog


---  
 #  WorldPosition : [real3](../nada_base_types/real3.md)

 `read-only`

> Returns the world-space position that the object was hit. Invalid on a volume cast.
> ``` lang=cpp, name=Nada
> var WorldPosition : Real3


---  
 #  Methods


---  
 #  CastResult : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function CastResult()
> ``` 


---  
 #  CastResult : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> |rhs|[castresult](castresult.md)| |
> ``` lang=cpp, name=Nada
> function CastResult(rhs : CastResult)
> ``` 


---  
 #  GetLocalPosition : [real3](../nada_base_types/real3.md)

> Returns the local-space position that the object was hit. The point index is used to get the first or last point of intersection. Invalid on volume casts.
> |Name|Type|Description|
> |---|---|---|
> |pointIndex|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function GetLocalPosition(pointIndex : Integer) : Real3
> ``` 


---  
 

 
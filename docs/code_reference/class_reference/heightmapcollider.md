 `Component` `Physics`



(NOTE) Defines collision for a height map.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ClearCachedEdgeAdjacency](heightmapcollider.md#clearcachededgeadjacency)|[ Thickness](heightmapcollider.md#thickness-zilch-engine-do)|[collider](collider.md)| |
|[ Constructor](heightmapcollider.md#heightmapcollider-void)| | | |


 #  Properties


---  
 #  Thickness : [real](../nada_base_types/real.md)

> How thick the surface of the height map is. Used to avoid tunneling problems.
> ```TS:Nada
> var Thickness : Real


---  
 #  Methods


---  
 #  ClearCachedEdgeAdjacency : Void

> Clear the cached information used to avoid catching edges. Typically called internally by physics, but is exposed for manual triggering.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ClearCachedEdgeAdjacency()
> ``` 


---  
 #  HeightMapCollider : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function HeightMapCollider()
> ``` 


---  
 

 
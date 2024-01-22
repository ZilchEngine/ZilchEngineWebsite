 `Physics`

(NOTE) Cast result from performing a sweep test.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](sweepresult.md#sweepresult-void)|[OtherCollider](sweepresult.md#othercollider-zilch-engin)| | |
| |[OtherObject](sweepresult.md#otherobject-zilch-engine)| | |
| |[Penetration](sweepresult.md#penetration-zilch-engine)| | |
| |[Time](sweepresult.md#time-zilch-engine-documen)| | |
| |[WorldNormalTowardsOther](sweepresult.md#worldnormaltowardsother)| | |
| |[WorldNormalTowardsSelf](sweepresult.md#worldnormaltowardsself-z)| | |
| |[WorldPoint](sweepresult.md#worldpoint-zilch-engine-d)| | |


 #  Properties


---  
 #  OtherCollider : [collider](collider.md)

 `read-only`

> The other collider being hit.
> ```TS:Nada
> var OtherCollider : Collider


---  
 #  OtherObject : [cog](cog.md)

 `read-only`

> The other cog being hit.
> ```TS:Nada
> var OtherObject : Cog


---  
 #  Penetration : [real](../nada_base_types/real.md)

 `read-only`

> The amount of overlap with this object. Will typically be zero unless the objects start in contact.
> ```TS:Nada
> var Penetration : Real


---  
 #  Time : [real](../nada_base_types/real.md)

 `read-only`

> The time of impact that this collision first happens.
> ```TS:Nada
> var Time : Real


---  
 #  WorldNormalTowardsOther : [real3](../nada_base_types/real3.md)

 `read-only`

> The contact normal pointing from the sweeping object towards the other object.
> ```TS:Nada
> var WorldNormalTowardsOther : Real3


---  
 #  WorldNormalTowardsSelf : [real3](../nada_base_types/real3.md)

 `read-only`

> The contact normal pointing from the other object towards the sweeping object.
> ```TS:Nada
> var WorldNormalTowardsSelf : Real3


---  
 #  WorldPoint : [real3](../nada_base_types/real3.md)

 `read-only`

> The point of intersection in world-space.
> ```TS:Nada
> var WorldPoint : Real3


---  
 #  Methods


---  
 #  SweepResult : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function SweepResult()
> ``` 


---  
 #  SweepResult : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ||[sweepresult](sweepresult.md)| |
> ```TS:Nada
> function SweepResult( : SweepResult)
> ``` 


---  
 

 
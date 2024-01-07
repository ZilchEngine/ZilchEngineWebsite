 `Physics`

(NOTE) Cast result from performing a sweep test.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sweepresult.md#sweepresult-void)|[ OtherCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sweepresult.md#othercollider-zilch-engin)| | |
| |[ OtherObject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sweepresult.md#otherobject-zilch-engine)| | |
| |[ Penetration](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sweepresult.md#penetration-zilch-engine)| | |
| |[ Time](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sweepresult.md#time-zilch-engine-documen)| | |
| |[ WorldNormalTowardsOther](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sweepresult.md#worldnormaltowardsother)| | |
| |[ WorldNormalTowardsSelf](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sweepresult.md#worldnormaltowardsself-z)| | |
| |[ WorldPoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sweepresult.md#worldpoint-zilch-engine-d)| | |


 #  Properties


---  
 #  OtherCollider : [collider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md)

 `read-only`

> The other collider being hit.
> ``` lang=cpp, name=Nada
> var OtherCollider : Collider


---  
 #  OtherObject : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

 `read-only`

> The other cog being hit.
> ``` lang=cpp, name=Nada
> var OtherObject : Cog


---  
 #  Penetration : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

 `read-only`

> The amount of overlap with this object. Will typically be zero unless the objects start in contact.
> ``` lang=cpp, name=Nada
> var Penetration : Real


---  
 #  Time : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

 `read-only`

> The time of impact that this collision first happens.
> ``` lang=cpp, name=Nada
> var Time : Real


---  
 #  WorldNormalTowardsOther : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

 `read-only`

> The contact normal pointing from the sweeping object towards the other object.
> ``` lang=cpp, name=Nada
> var WorldNormalTowardsOther : Real3


---  
 #  WorldNormalTowardsSelf : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

 `read-only`

> The contact normal pointing from the other object towards the sweeping object.
> ``` lang=cpp, name=Nada
> var WorldNormalTowardsSelf : Real3


---  
 #  WorldPoint : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

 `read-only`

> The point of intersection in world-space.
> ``` lang=cpp, name=Nada
> var WorldPoint : Real3


---  
 #  Methods


---  
 #  SweepResult : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function SweepResult()
> ``` 


---  
 #  SweepResult : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ||[sweepresult](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sweepresult.md)| |
> ``` lang=cpp, name=Nada
> function SweepResult( : SweepResult)
> ``` 


---  
 

 
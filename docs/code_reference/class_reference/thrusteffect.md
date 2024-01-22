 `Component` `Physics`



(NOTE) Applies a directional force at the thrust effect's center. When applied to a rigid body, this will compute a torque if the force's direction does not go through the center of mass. Useful for modeling any sort of a thruster.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](thrusteffect.md#thrusteffect-void)|[ForceDirection](thrusteffect.md#forcedirection-zilch-engi)|[physicseffect](physicseffect.md)| |
| |[ForceStrength](thrusteffect.md#forcestrength-zilch-engin)| | |
| |[LocalSpaceDirection](thrusteffect.md#localspacedirection-zero)| | |
| |[WorldForceDirection](thrusteffect.md#worldforcedirection-zero)| | |


 #  Properties


---  
 #  ForceDirection : [real3](../nada_base_types/real3.md)

> The direction that the force should be applied.
> ```TS:Nada
> var ForceDirection : Real3


---  
 #  ForceStrength : [real](../nada_base_types/real.md)

> The strength of the force being applied in the force direction.
> ```TS:Nada
> var ForceStrength : Real


---  
 #  LocalSpaceDirection : [boolean](../nada_base_types/boolean.md)

> Determines if this force is to be applied in local or world space.
> ```TS:Nada
> var LocalSpaceDirection : Boolean


---  
 #  WorldForceDirection : [real3](../nada_base_types/real3.md)

 `read-only`

> The direction that the force should be applied in world space.
> ```TS:Nada
> var WorldForceDirection : Real3


---  
 #  Methods


---  
 #  ThrustEffect : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ThrustEffect()
> ``` 


---  
 

 
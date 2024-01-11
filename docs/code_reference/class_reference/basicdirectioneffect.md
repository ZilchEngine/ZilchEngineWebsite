 `Component` `Physics`



(NOTE) Common interface for all directional force effects. Used to group together all common logic/variables for the force/gravity variants.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ Direction](basicdirectioneffect.md#direction-zilch-engine-do)|[physicseffect](physicseffect.md)|[forceeffect](forceeffect.md)|
| |[ LocalSpaceDirection](basicdirectioneffect.md#localspacedirection-zero)| |[gravityeffect](gravityeffect.md)|
| |[ Strength](basicdirectioneffect.md#strength-zilch-engine-doc)| | |
| |[ WorldDirection](basicdirectioneffect.md#worlddirection-zilch-engi)| | |


 #  Properties


---  
 #  Direction : [real3](../nada_base_types/real3.md)

> The direction that the effect will be applied in (may be in local or world space depending on the LocalSpaceDirection property).
> ```TS:Nada
> var Direction : Real3


---  
 #  LocalSpaceDirection : [boolean](../nada_base_types/boolean.md)

> Determines if the direction that the effect is applied is in local or world space. This vector is normalized when calculating forces.
> ```TS:Nada
> var LocalSpaceDirection : Boolean


---  
 #  Strength : [real](../nada_base_types/real.md)

> The magnitude of the force to apply.
> ```TS:Nada
> var Strength : Real


---  
 #  WorldDirection : [real3](../nada_base_types/real3.md)

 `read-only`

> The world direction of the effect. If the effect is not in local space then this is the same as Direction.
> ```TS:Nada
> var WorldDirection : Real3


---  
 #  Methods


---  
 

 
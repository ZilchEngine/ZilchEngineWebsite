 `Component` `Physics`



(NOTE) Applies a directional force at the thrust effect's center. When applied to a rigid body, this will compute a torque if the force's direction does not go through the center of mass. Useful for modeling any sort of a thruster.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/thrusteffect.md#thrusteffect-void)|[ ForceDirection](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/thrusteffect.md#forcedirection-zilch-engi)|[physicseffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicseffect.md)| |
| |[ ForceStrength](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/thrusteffect.md#forcestrength-zilch-engin)| | |
| |[ LocalSpaceDirection](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/thrusteffect.md#localspacedirection-zero)| | |
| |[ WorldForceDirection](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/thrusteffect.md#worldforcedirection-zero)| | |


 #  Properties


---  
 #  ForceDirection : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The direction that the force should be applied.
> ``` lang=cpp, name=Nada
> var ForceDirection : Real3


---  
 #  ForceStrength : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The strength of the force being applied in the force direction.
> ``` lang=cpp, name=Nada
> var ForceStrength : Real


---  
 #  LocalSpaceDirection : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Determines if this force is to be applied in local or world space.
> ``` lang=cpp, name=Nada
> var LocalSpaceDirection : Boolean


---  
 #  WorldForceDirection : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

 `read-only`

> The direction that the force should be applied in world space.
> ``` lang=cpp, name=Nada
> var WorldForceDirection : Real3


---  
 #  Methods


---  
 #  ThrustEffect : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ThrustEffect()
> ``` 


---  
 

 
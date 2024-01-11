 `Physics`

(NOTE) A block of information for solving a joint (or constraint) type. This is used to configure how one joint is solved independently of another joint.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ AngularBaumgarte](constraintconfigblock.md#angularbaumgarte-zilch-en)|[safeid32object](safeid32object.md)|[contactblock](contactblock.md)|
| |[ AngularErrorCorrection](constraintconfigblock.md#angularerrorcorrection-z)| |[customjointblock](customjointblock.md)|
| |[ LinearBaumgarte](constraintconfigblock.md#linearbaumgarte-zilch-eng)| |[fixedanglejointblock](fixedanglejointblock.md)|
| |[ LinearErrorCorrection](constraintconfigblock.md#linearerrorcorrection-ze)| |[gearjointblock](gearjointblock.md)|
| |[ PositionCorrectionType](constraintconfigblock.md#positioncorrectiontype-z)| |[linearaxisjointblock](linearaxisjointblock.md)|
| |[ Slop](constraintconfigblock.md#slop-zilch-engine-documen)| |[manipulatorjointblock](manipulatorjointblock.md)|
| | | |[phygunjointblock](phygunjointblock.md)|
| | | |[positionjointblock](positionjointblock.md)|
| | | |[prismaticjoint2dblock](prismaticjoint2dblock.md)|
| | | |[prismaticjointblock](prismaticjointblock.md)|
| | | |[pulleyjointblock](pulleyjointblock.md)|
| | | |[relativevelocityjointblock](relativevelocityjointblock.md)|
| | | |[revolutejoint2dblock](revolutejoint2dblock.md)|
| | | |[revolutejointblock](revolutejointblock.md)|
| | | |[stickjointblock](stickjointblock.md)|
| | | |[universaljointblock](universaljointblock.md)|
| | | |[uprightjointblock](uprightjointblock.md)|
| | | |[weldjointblock](weldjointblock.md)|
| | | |[wheeljoint2dblock](wheeljoint2dblock.md)|
| | | |[wheeljointblock](wheeljointblock.md)|


 #  Properties


---  
 #  AngularBaumgarte : [real](../nada_base_types/real.md)

> The exponential constant for correcting angular error with a penalty impulse.
> ``` lang=cpp, name=Nada
> var AngularBaumgarte : Real


---  
 #  AngularErrorCorrection : [real](../nada_base_types/real.md)

> The max amount of error that can be corrected by the angular portion of any constraint in one frame (only for PostStabilization).
> ``` lang=cpp, name=Nada
> var AngularErrorCorrection : Real


---  
 #  LinearBaumgarte : [real](../nada_base_types/real.md)

> The exponential constant for correcting linear error with a penalty impulse.
> ``` lang=cpp, name=Nada
> var LinearBaumgarte : Real


---  
 #  LinearErrorCorrection : [real](../nada_base_types/real.md)

> The max amount of error that can be corrected by the linear portion of any constraint in one frame (only for PostStabilization).
> ``` lang=cpp, name=Nada
> var LinearErrorCorrection : Real


---  
 #  PositionCorrectionType : [ConstraintPositionCorrection](../enum_reference.md#constraintpositioncorrection)

> What method should be used to fix errors in joints.
> ``` lang=cpp, name=Nada
> var PositionCorrectionType : ConstraintPositionCorrection


---  
 #  Slop : [real](../nada_base_types/real.md)

> The amount of error allowed before position correction takes effect.
> ``` lang=cpp, name=Nada
> var Slop : Real


---  
 #  Methods


---  
 

 
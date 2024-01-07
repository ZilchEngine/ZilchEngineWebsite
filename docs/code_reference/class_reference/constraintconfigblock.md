 `Physics`

(NOTE) A block of information for solving a joint (or constraint) type. This is used to configure how one joint is solved independently of another joint.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ AngularBaumgarte](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/constraintconfigblock.md#angularbaumgarte-zilch-en)|[safeid32object](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/safeid32object.md)|[contactblock](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contactblock.md)|
| |[ AngularErrorCorrection](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/constraintconfigblock.md#angularerrorcorrection-z)| |[customjointblock](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customjointblock.md)|
| |[ LinearBaumgarte](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/constraintconfigblock.md#linearbaumgarte-zilch-eng)| |[fixedanglejointblock](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/fixedanglejointblock.md)|
| |[ LinearErrorCorrection](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/constraintconfigblock.md#linearerrorcorrection-ze)| |[gearjointblock](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gearjointblock.md)|
| |[ PositionCorrectionType](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/constraintconfigblock.md#positioncorrectiontype-z)| |[linearaxisjointblock](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/linearaxisjointblock.md)|
| |[ Slop](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/constraintconfigblock.md#slop-zilch-engine-documen)| |[manipulatorjointblock](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/manipulatorjointblock.md)|
| | | |[phygunjointblock](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/phygunjointblock.md)|
| | | |[positionjointblock](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/positionjointblock.md)|
| | | |[prismaticjoint2dblock](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/prismaticjoint2dblock.md)|
| | | |[prismaticjointblock](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/prismaticjointblock.md)|
| | | |[pulleyjointblock](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/pulleyjointblock.md)|
| | | |[relativevelocityjointblock](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/relativevelocityjointblock.md)|
| | | |[revolutejoint2dblock](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/revolutejoint2dblock.md)|
| | | |[revolutejointblock](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/revolutejointblock.md)|
| | | |[stickjointblock](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/stickjointblock.md)|
| | | |[universaljointblock](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/universaljointblock.md)|
| | | |[uprightjointblock](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uprightjointblock.md)|
| | | |[weldjointblock](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/weldjointblock.md)|
| | | |[wheeljoint2dblock](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/wheeljoint2dblock.md)|
| | | |[wheeljointblock](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/wheeljointblock.md)|


 #  Properties


---  
 #  AngularBaumgarte : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The exponential constant for correcting angular error with a penalty impulse.
> ``` lang=cpp, name=Nada
> var AngularBaumgarte : Real


---  
 #  AngularErrorCorrection : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The max amount of error that can be corrected by the angular portion of any constraint in one frame (only for PostStabilization).
> ``` lang=cpp, name=Nada
> var AngularErrorCorrection : Real


---  
 #  LinearBaumgarte : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The exponential constant for correcting linear error with a penalty impulse.
> ``` lang=cpp, name=Nada
> var LinearBaumgarte : Real


---  
 #  LinearErrorCorrection : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The max amount of error that can be corrected by the linear portion of any constraint in one frame (only for PostStabilization).
> ``` lang=cpp, name=Nada
> var LinearErrorCorrection : Real


---  
 #  PositionCorrectionType : [ConstraintPositionCorrection](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#constraintpositioncorrection)

> What method should be used to fix errors in joints.
> ``` lang=cpp, name=Nada
> var PositionCorrectionType : ConstraintPositionCorrection


---  
 #  Slop : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The amount of error allowed before position correction takes effect.
> ``` lang=cpp, name=Nada
> var Slop : Real


---  
 #  Methods


---  
 

 
 `Component` `Gameplay`



(NOTE) A random object that contains its own unique random state apart from all other instances of this class.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ BellCurve](randomcontext.md#bellcurve-zilch-engine-do)|[ MaxInt](randomcontext.md#maxint-zilch-engine-docum)|[component](component.md)| |
|[ BellCurveDistribution](randomcontext.md#bellcurvedistribution-ze)|[ RandomSeed](randomcontext.md#randomseed-zilch-engine-d)| | |
|[ BellCurveRange](randomcontext.md#bellcurverange-zilch-engi)|[ Seed](randomcontext.md#seed-zilch-engine-documen)| | |
|[ Bool](randomcontext.md#bool-zilch-engine-documen)| | | |
|[ CoinFlip](randomcontext.md#coinflip-zilch-engine-doc)| | | |
|[ DieRoll](randomcontext.md#dieroll-zilch-engine-docu)| | | |
|[ DoubleRange](randomcontext.md#doublerange-zilch-engine)| | | |
|[ DoubleReal](randomcontext.md#doublereal-zilch-engine-d)| | | |
|[ DoubleRealVariance](randomcontext.md#doublerealvariance-zero)| | | |
|[ Float](randomcontext.md#float-zilch-engine-docume)| | | |
|[ FloatVariance](randomcontext.md#floatvariance-zilch-engin)| | | |
|[ Int](randomcontext.md#int-zilch-engine-document)| | | |
|[ IntVariance](randomcontext.md#intvariance-zilch-engine)| | | |
|[ Probability](randomcontext.md#probability-zilch-engine)| | | |
|[ Quaternion](randomcontext.md#quaternion-zilch-engine-d)| | | |
|[ Constructor](randomcontext.md#randomcontext-void)| | | |
|[ Range](randomcontext.md#range-zilch-engine-docume)| | | |
|[ RangeExclusiveMax](randomcontext.md#rangeexclusivemax-zilch-e)| | | |
|[ RangeInclusiveMax](randomcontext.md#rangeinclusivemax-zilch-e)| | | |
|[ Real](randomcontext.md#real-zilch-engine-documen)| | | |
|[ Real2](randomcontext.md#real2-zilch-engine-docume)| | | |
|[ Real3](randomcontext.md#real3-zilch-engine-docume)| | | |
|[ RealVariance](randomcontext.md#realvariance-zilch-engine)| | | |
|[ Rotation](randomcontext.md#rotation-zilch-engine-doc)| | | |
|[ UnitReal2](randomcontext.md#unitreal2-zilch-engine-do)| | | |
|[ UnitReal3](randomcontext.md#unitreal3-zilch-engine-do)| | | |
|[ UnitVector2](randomcontext.md#unitvector2-zilch-engine)| | | |
|[ UnitVector3](randomcontext.md#unitvector3-zilch-engine)| | | |
|[ Vector2](randomcontext.md#vector2-zilch-engine-docu)| | | |
|[ Vector3](randomcontext.md#vector3-zilch-engine-docu)| | | |


 #  Properties


---  
 #  MaxInt : [integer](../nada_base_types/integer.md)

 `read-only`

> The max integer value that can be returned.
> ``` lang=cpp, name=Nada
> var MaxInt : Integer


---  
 #  RandomSeed : [boolean](../nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var RandomSeed : Boolean


---  
 #  Seed : [integer](../nada_base_types/integer.md)

> Seeds the random number generator.
> ``` lang=cpp, name=Nada
> var Seed : Integer


---  
 #  Methods


---  
 #  BellCurve : [real](../nada_base_types/real.md)

> Samples a bell curve with standard normal distribution in the range [0,1] This is equivalent to a Gaussian distribution with standard deviation of 1.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function BellCurve() : Real
> ``` 


---  
 #  BellCurveDistribution : [real](../nada_base_types/real.md)

> Samples a bell curve in the range [center - range, center + range] with the given standard deviation. Around 68% will lie within the 1st standard deviation.
> |Name|Type|Description|
> |---|---|---|
> |center|[real](../nada_base_types/real.md)| |
> |range|[real](../nada_base_types/real.md)| |
> |standardDeviation|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function BellCurveDistribution(center : Real, range : Real, standardDeviation : Real) : Real
> ``` 


---  
 #  BellCurveRange : [real](../nada_base_types/real.md)

> Samples a bell curve with in the range [center - range, center + range] This uses a standard deviation of 1.
> |Name|Type|Description|
> |---|---|---|
> |center|[real](../nada_base_types/real.md)| |
> |range|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function BellCurveRange(center : Real, range : Real) : Real
> ``` 


---  
 #  Bool : [boolean](../nada_base_types/boolean.md)

> Returns a random bool value.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Bool() : Boolean
> ``` 


---  
 #  CoinFlip : [boolean](../nada_base_types/boolean.md)

> Returns true if the coin flips heads.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function CoinFlip() : Boolean
> ``` 


---  
 #  DieRoll : [integer](../nada_base_types/integer.md)

> Randomly rolls a number in the range [1, sides].
> |Name|Type|Description|
> |---|---|---|
> |sides|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function DieRoll(sides : Integer) : Integer
> ``` 


---  
 #  DoubleRange : [doublereal](../nada_base_types/doublereal.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ||[doublereal](../nada_base_types/doublereal.md)| |
> ||[doublereal](../nada_base_types/doublereal.md)| |
> ``` lang=cpp, name=Nada
> function DoubleRange( : DoubleReal,  : DoubleReal) : DoubleReal
> ``` 


---  
 #  DoubleReal : [doublereal](../nada_base_types/doublereal.md)

> Returns a random double real in the range [0,1].
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function DoubleReal() : DoubleReal
> ``` 


---  
 #  DoubleRealVariance : [doublereal](../nada_base_types/doublereal.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ||[doublereal](../nada_base_types/doublereal.md)| |
> ||[doublereal](../nada_base_types/doublereal.md)| |
> ``` lang=cpp, name=Nada
> function DoubleRealVariance( : DoubleReal,  : DoubleReal) : DoubleReal
> ``` 


---  
 #  Float : [real](../nada_base_types/real.md)

> Returns a random float in the range [0,1].
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Float() : Real
> ``` 


---  
 #  FloatVariance : [real](../nada_base_types/real.md)

> Returns a float in the range [base - variance, base + variance].
> |Name|Type|Description|
> |---|---|---|
> |base|[real](../nada_base_types/real.md)| |
> |variance|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function FloatVariance(base : Real, variance : Real) : Real
> ``` 


---  
 #  Int : [integer](../nada_base_types/integer.md)

> Returns a random int in the range of [0, MaxInt].
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Int() : Integer
> ``` 


---  
 #  IntVariance : [integer](../nada_base_types/integer.md)

> Int in the range [base - variance, base + variance].
> |Name|Type|Description|
> |---|---|---|
> |base|[integer](../nada_base_types/integer.md)| |
> |variance|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function IntVariance(base : Integer, variance : Integer) : Integer
> ``` 


---  
 #  Probability : [boolean](../nada_base_types/boolean.md)

> Takes a given probability that we get a true value.
> |Name|Type|Description|
> |---|---|---|
> |probOfTrue|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function Probability(probOfTrue : Real) : Boolean
> ``` 


---  
 #  Quaternion : [quaternion](../nada_base_types/quaternion.md)

> Random unit length quaternion. This is also a unit quaternion.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Quaternion() : Quaternion
> ``` 


---  
 #  RandomContext : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function RandomContext()
> ``` 


---  
 #  Range : [real](../nada_base_types/real.md)

> A random float in the range [min,max].
> |Name|Type|Description|
> |---|---|---|
> |min|[real](../nada_base_types/real.md)| |
> |max|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function Range(min : Real, max : Real) : Real
> ``` 


---  
 #  RangeExclusiveMax : [integer](../nada_base_types/integer.md)

> Int in the range [min, max)
> |Name|Type|Description|
> |---|---|---|
> |min|[integer](../nada_base_types/integer.md)| |
> |max|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function RangeExclusiveMax(min : Integer, max : Integer) : Integer
> ``` 


---  
 #  RangeInclusiveMax : [integer](../nada_base_types/integer.md)

> Int in the range [min, max].
> |Name|Type|Description|
> |---|---|---|
> |min|[integer](../nada_base_types/integer.md)| |
> |max|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function RangeInclusiveMax(min : Integer, max : Integer) : Integer
> ``` 


---  
 #  Real : [real](../nada_base_types/real.md)

> Returns a random real in the range [0,1].
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Real() : Real
> ``` 


---  
 #  Real2 : [real2](../nada_base_types/real2.md)

> Randomly generates a Real2 with its length between min and max.
> |Name|Type|Description|
> |---|---|---|
> |minLength|[real](../nada_base_types/real.md)| |
> |maxLength|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function Real2(minLength : Real, maxLength : Real) : Real2
> ``` 


---  
 #  Real3 : [real3](../nada_base_types/real3.md)

> Randomly generates a Real3 with its length between min and max.
> |Name|Type|Description|
> |---|---|---|
> |minLength|[real](../nada_base_types/real.md)| |
> |maxLength|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function Real3(minLength : Real, maxLength : Real) : Real3
> ``` 


---  
 #  RealVariance : [real](../nada_base_types/real.md)

> Returns a real in the range [base - variance, base + variance].
> |Name|Type|Description|
> |---|---|---|
> |base|[real](../nada_base_types/real.md)| |
> |variance|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function RealVariance(base : Real, variance : Real) : Real
> ``` 


---  
 #  Rotation : [quaternion](../nada_base_types/quaternion.md)

> Random rotation quaternion. This is the same as calling Quaternion()
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Rotation() : Quaternion
> ``` 


---  
 #  UnitReal2 : [real2](../nada_base_types/real2.md)

> Generates a unit length Real2.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function UnitReal2() : Real2
> ``` 


---  
 #  UnitReal3 : [real3](../nada_base_types/real3.md)

> Generates a unit length Real3.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function UnitReal3() : Real3
> ``` 


---  
 #  UnitVector2 : [real2](../nada_base_types/real2.md)

> Generates a unit length Vec2.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function UnitVector2() : Real2
> ``` 


---  
 #  UnitVector3 : [real3](../nada_base_types/real3.md)

> Generates a unit length Vec3.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function UnitVector3() : Real3
> ``` 


---  
 #  Vector2 : [real2](../nada_base_types/real2.md)

> Randomly generates a Vec2 with its length between min and max.
> |Name|Type|Description|
> |---|---|---|
> |minLength|[real](../nada_base_types/real.md)| |
> |maxLength|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function Vector2(minLength : Real, maxLength : Real) : Real2
> ``` 


---  
 #  Vector3 : [real3](../nada_base_types/real3.md)

> Randomly generates a Vec3 with its length between min and max.
> |Name|Type|Description|
> |---|---|---|
> |minLength|[real](../nada_base_types/real.md)| |
> |maxLength|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function Vector3(minLength : Real, maxLength : Real) : Real3
> ``` 


---  
 

 
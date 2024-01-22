 `Core`

(NOTE) Contains utility functions for random generation.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[BellCurve](random.md#bellcurve-zilch-engine-do)|[MaxInteger](random.md#maxinteger-zilch-engine-d)| | |
|[Boolean](random.md#boolean-zilch-engine-docu)|[Seed](random.md#seed-zilch-engine-documen)| | |
|[CoinFlip](random.md#coinflip-zilch-engine-doc)| | | |
|[DieRoll](random.md#dieroll-zilch-engine-docu)| | | |
|[DoubleRange](random.md#doublerange-zilch-engine)| | | |
|[DoubleReal](random.md#doublereal-zilch-engine-d)| | | |
|[Integer](random.md#integer-zilch-engine-docu)| | | |
|[Probability](random.md#probability-zilch-engine)| | | |
|[Quaternion](random.md#quaternion-zilch-engine-d)| | | |
|[Constructor](random.md#random-void)| | | |
|[Range](random.md#range-zilch-engine-docume)| | | |
|[RangeExclusiveMax](random.md#rangeexclusivemax-zilch-e)| | | |
|[RangeInclusiveMax](random.md#rangeinclusivemax-zilch-e)| | | |
|[Real](random.md#real-zilch-engine-documen)| | | |
|[Real2](random.md#real2-zilch-engine-docume)| | | |
|[Real3](random.md#real3-zilch-engine-docume)| | | |
|[Rotation](random.md#rotation-zilch-engine-doc)| | | |
|[UnitReal2](random.md#unitreal2-zilch-engine-do)| | | |
|[UnitReal3](random.md#unitreal3-zilch-engine-do)| | | |
|[Variance](random.md#variance-zilch-engine-doc)| | | |


 #  Properties


---  
 #  MaxInteger : [integer](integer.md)

 `read-only` `static`

> Returns the max integer value that can be returned.
> ```TS:Nada
> var MaxInteger : Integer


---  
 #  Seed : [integer](integer.md)

> The seed controls what random numbers are generated in a sequence (determanistically) The same seed will always generate the same string of random numbers.
> ```TS:Nada
> var Seed : Integer


---  
 #  Methods


---  
 #  BellCurve : [real](real.md)

> Samples a bell curve with standard normal distribution in the range [0,1] This is equivalent to a Gaussian distribution with standard deviation of 1.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function BellCurve() : Real
> ``` 


---  
 #  BellCurve : [real](real.md)

> Samples a bell curve with in the range [center - range, center + range] This uses a standard deviation of 1.
> |Name|Type|Description|
> |---|---|---|
> |center|[real](real.md)| |
> |range|[real](real.md)| |
> ```TS:Nada
> function BellCurve(center : Real, range : Real) : Real
> ``` 


---  
 #  BellCurve : [real](real.md)

> Samples a bell curve in the range [center - range, center + range] with the given standard deviation. Around 68% will lie within the 1st standard deviation.
> |Name|Type|Description|
> |---|---|---|
> |center|[real](real.md)| |
> |range|[real](real.md)| |
> |standardDeviation|[real](real.md)| |
> ```TS:Nada
> function BellCurve(center : Real, range : Real, standardDeviation : Real) : Real
> ``` 


---  
 #  Boolean : [boolean](boolean.md)

> Returns a random boolean value.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Boolean() : Boolean
> ``` 


---  
 #  CoinFlip : [boolean](boolean.md)

> Returns true if the coin flips heads.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function CoinFlip() : Boolean
> ``` 


---  
 #  DieRoll : [integer](integer.md)

> Randomly rolls a number in the range [1, sides].
> |Name|Type|Description|
> |---|---|---|
> |sides|[integer](integer.md)| |
> ```TS:Nada
> function DieRoll(sides : Integer) : Integer
> ``` 


---  
 #  DoubleRange : [doublereal](doublereal.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ||[doublereal](doublereal.md)| |
> ||[doublereal](doublereal.md)| |
> ```TS:Nada
> function DoubleRange( : DoubleReal,  : DoubleReal) : DoubleReal
> ``` 


---  
 #  DoubleReal : [doublereal](doublereal.md)

> Returns a random double real in the range [0,1].
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function DoubleReal() : DoubleReal
> ``` 


---  
 #  Integer : [integer](integer.md)

> Returns a random integer in the range of [0, MaxInt].
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Integer() : Integer
> ``` 


---  
 #  Probability : [boolean](boolean.md)

> Takes a given probability that we get a true value.
> |Name|Type|Description|
> |---|---|---|
> |probOfTrue|[real](real.md)| |
> ```TS:Nada
> function Probability(probOfTrue : Real) : Boolean
> ``` 


---  
 #  Quaternion : [quaternion](quaternion.md)

> Random unit length quaternion. This is also a unit quaternion.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Quaternion() : Quaternion
> ``` 


---  
 #  Random : Void

 `constructor`

> Default constructor (grabs the random seed)
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Random()
> ``` 


---  
 #  Random : Void

 `constructor`

> Construct a random generator with a specific seed.
> |Name|Type|Description|
> |---|---|---|
> |seed|[integer](integer.md)| |
> ```TS:Nada
> function Random(seed : Integer)
> ``` 


---  
 #  Range : [real](real.md)

> A random Real in the range [min,max].
> |Name|Type|Description|
> |---|---|---|
> |min|[real](real.md)| |
> |max|[real](real.md)| |
> ```TS:Nada
> function Range(min : Real, max : Real) : Real
> ``` 


---  
 #  RangeExclusiveMax : [integer](integer.md)

> Integer in the range [min, max].
> |Name|Type|Description|
> |---|---|---|
> |min|[integer](integer.md)| |
> |max|[integer](integer.md)| |
> ```TS:Nada
> function RangeExclusiveMax(min : Integer, max : Integer) : Integer
> ``` 


---  
 #  RangeInclusiveMax : [integer](integer.md)

> Integer in the range [min, max)
> |Name|Type|Description|
> |---|---|---|
> |min|[integer](integer.md)| |
> |max|[integer](integer.md)| |
> ```TS:Nada
> function RangeInclusiveMax(min : Integer, max : Integer) : Integer
> ``` 


---  
 #  Real : [real](real.md)

> Returns a random real in the range [0,1].
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Real() : Real
> ``` 


---  
 #  Real2 : [real2](real2.md)

> Randomly generates a Real2 with its length between min and max.
> |Name|Type|Description|
> |---|---|---|
> |minLength|[real](real.md)| |
> |maxLength|[real](real.md)| |
> ```TS:Nada
> function Real2(minLength : Real, maxLength : Real) : Real2
> ``` 


---  
 #  Real3 : [real3](real3.md)

> Randomly generates a Real3 with its length between min and max.
> |Name|Type|Description|
> |---|---|---|
> |minLength|[real](real.md)| |
> |maxLength|[real](real.md)| |
> ```TS:Nada
> function Real3(minLength : Real, maxLength : Real) : Real3
> ``` 


---  
 #  Rotation : [quaternion](quaternion.md)

> Random rotation quaternion. This is the same as calling Quaternion()
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Rotation() : Quaternion
> ``` 


---  
 #  UnitReal2 : [real2](real2.md)

> Generates a unit length Real2.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function UnitReal2() : Real2
> ``` 


---  
 #  UnitReal3 : [real3](real3.md)

> Generates a unit length Real3.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function UnitReal3() : Real3
> ``` 


---  
 #  Variance : [doublereal](doublereal.md)

> Integer in the range [base - variance, base + variance].
> |Name|Type|Description|
> |---|---|---|
> ||[doublereal](doublereal.md)| |
> ||[doublereal](doublereal.md)| |
> ```TS:Nada
> function Variance( : DoubleReal,  : DoubleReal) : DoubleReal
> ``` 


---  
 #  Variance : [integer](integer.md)

> Integer in the range [base - variance, base + variance].
> |Name|Type|Description|
> |---|---|---|
> |base|[integer](integer.md)| |
> |variance|[integer](integer.md)| |
> ```TS:Nada
> function Variance(base : Integer, variance : Integer) : Integer
> ``` 


---  
 #  Variance : [real](real.md)

> Returns a number in the range [base - variance, base + variance].
> |Name|Type|Description|
> |---|---|---|
> |base|[real](real.md)| |
> |variance|[real](real.md)| |
> ```TS:Nada
> function Variance(base : Real, variance : Real) : Real
> ``` 


---  
 

 
 `Component` `Gameplay`



(NOTE) Defines a new basis for a desired right, up, and forward vector. Provides a bunch of helper functions to change between these spaces and to perform simple look-at behavior.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ComputeSignedAngle](orientation.md#computesignedangle-zero)|[AbsoluteAngle](orientation.md#absoluteangle-zilch-engin)|[component](component.md)| |
|[DebugDrawBases](orientation.md#debugdrawbases-void)|[DefaultOrientationBases](orientation.md#defaultorientationbases)| | |
|[GetLookAtDirectionRotation](orientation.md#getlookatdirectionrotati)|[GlobalUp](orientation.md#globalup-zilch-engine-doc)| | |
|[GetLookAtDirectionWithUpRotation](orientation.md#getlookatdirectionwithup)|[LocalForward](orientation.md#localforward-zilch-engine)| | |
|[GetLookAtPointRotation](orientation.md#getlookatpointrotation-z)|[LocalOrientationBasis](orientation.md#localorientationbasis-ze)| | |
|[GetLookAtPointWithUpRotation](orientation.md#getlookatpointwithuprota)|[LocalRight](orientation.md#localright-zilch-engine-d)| | |
|[LookAtDirection](orientation.md#lookatdirection-void)|[LocalToOrientationRotation](orientation.md#localtoorientationrotati)| | |
|[LookAtDirectionWithUp](orientation.md#lookatdirectionwithup-vo)|[LocalToWorldRotation](orientation.md#localtoworldrotation-zer)| | |
|[LookAtPoint](orientation.md#lookatpoint-void)|[LocalUp](orientation.md#localup-zilch-engine-docu)| | |
|[LookAtPointWithUp](orientation.md#lookatpointwithup-void)|[OrientationForward](orientation.md#orientationforward-zero)| | |
|[Constructor](orientation.md#orientation-void)|[OrientationRight](orientation.md#orientationright-zilch-en)| | |
|[SetLocalLookAtRotation](orientation.md#setlocallookatrotation-v)|[OrientationToLocalRotation](orientation.md#orientationtolocalrotati)| | |
|[SetWorldLookAtRotation](orientation.md#setworldlookatrotation-v)|[OrientationToWorldRotation](orientation.md#orientationtoworldrotati)| | |
| |[OrientationUp](orientation.md#orientationup-zilch-engin)| | |
| |[WorldForward](orientation.md#worldforward-zilch-engine)| | |
| |[WorldRight](orientation.md#worldright-zilch-engine-d)| | |
| |[WorldToLocalRotation](orientation.md#worldtolocalrotation-zer)| | |
| |[WorldToOrientationRotation](orientation.md#worldtoorientationrotati)| | |
| |[WorldUp](orientation.md#worldup-zilch-engine-docu)| | |


 #  Properties


---  
 #  AbsoluteAngle : [real](../nada_base_types/real.md)

 `read-only`

> Get the angle of the object about the up vector.
> ```TS:Nada
> var AbsoluteAngle : Real


---  
 #  DefaultOrientationBases : [OrientationBases](../enum_reference.md#orientationbases)

> 
> ```TS:Nada
> var DefaultOrientationBases : OrientationBases


---  
 #  GlobalUp : [real3](../nada_base_types/real3.md)

> The world-space up vector to use for LookAt operations that don't take an up vector.
> ```TS:Nada
> var GlobalUp : Real3


---  
 #  LocalForward : [real3](../nada_base_types/real3.md)

 `read-only`

> The orientation's forward vector after having been transformed into local space.
> ```TS:Nada
> var LocalForward : Real3


---  
 #  LocalOrientationBasis : [quaternion](../nada_base_types/quaternion.md)

> A local-space basis that represents this orientation. If you build a basis from an up of (0, 1, 0), and a forward of (0, 0, -1) then this should result in the identity rotation.
> ```TS:Nada
> var LocalOrientationBasis : Quaternion


---  
 #  LocalRight : [real3](../nada_base_types/real3.md)

 `read-only`

> The orientation's right vector after having been transformed into local space.
> ```TS:Nada
> var LocalRight : Real3


---  
 #  LocalToOrientationRotation : [quaternion](../nada_base_types/quaternion.md)

 `read-only`

> The rotation that takes an local space vector into orientation space. For example, this transforms LocalRight into OrientationRight.
> ```TS:Nada
> var LocalToOrientationRotation : Quaternion


---  
 #  LocalToWorldRotation : [quaternion](../nada_base_types/quaternion.md)

 `read-only`

> The rotation that transforms a vector from local space into world space. For example, this transforms LocalRight into WorldRight.
> ```TS:Nada
> var LocalToWorldRotation : Quaternion


---  
 #  LocalUp : [real3](../nada_base_types/real3.md)

 `read-only`

> The orientation's up vector after having been transformed into local space.
> ```TS:Nada
> var LocalUp : Real3


---  
 #  OrientationForward : [real3](../nada_base_types/real3.md)

 `read-only`

> The forward vector in orientation space. This is always the vector (0, 0, -1) but is provided for clarity with transformations.
> ```TS:Nada
> var OrientationForward : Real3


---  
 #  OrientationRight : [real3](../nada_base_types/real3.md)

 `read-only`

> The right vector in orientation space. This is always the vector (1, 0, 0) but is provided for clarity with transformations.
> ```TS:Nada
> var OrientationRight : Real3


---  
 #  OrientationToLocalRotation : [quaternion](../nada_base_types/quaternion.md)

 `read-only`

> The rotation that takes an orientation space vector into local space. For example, this transforms OrientationRight into LocalRight.
> ```TS:Nada
> var OrientationToLocalRotation : Quaternion


---  
 #  OrientationToWorldRotation : [quaternion](../nada_base_types/quaternion.md)

 `read-only`

> The rotation that takes an orientation space vector into world space. For example, this transforms OrientationRight into WorldRight.
> ```TS:Nada
> var OrientationToWorldRotation : Quaternion


---  
 #  OrientationUp : [real3](../nada_base_types/real3.md)

 `read-only`

> The up vector in orientation space. This is always the vector (0, 1, 0) but is provided for clarity with transformations.
> ```TS:Nada
> var OrientationUp : Real3


---  
 #  WorldForward : [real3](../nada_base_types/real3.md)

 `read-only`

> The orientation's forward vector after having been transformed into world space.
> ```TS:Nada
> var WorldForward : Real3


---  
 #  WorldRight : [real3](../nada_base_types/real3.md)

 `read-only`

> The orientation's right vector after having been transformed into world space.
> ```TS:Nada
> var WorldRight : Real3


---  
 #  WorldToLocalRotation : [quaternion](../nada_base_types/quaternion.md)

 `read-only`

> The rotation that transforms a vector from world space into local space. For example, this transforms WorldRight into LocalRight.
> ```TS:Nada
> var WorldToLocalRotation : Quaternion


---  
 #  WorldToOrientationRotation : [quaternion](../nada_base_types/quaternion.md)

 `read-only`

> The rotation that takes an world space vector into orientation space. For example, this transforms WorldRight into OrientationRight.
> ```TS:Nada
> var WorldToOrientationRotation : Quaternion


---  
 #  WorldUp : [real3](../nada_base_types/real3.md)

 `read-only`

> The orientation's up vector after having been transformed into world space.
> ```TS:Nada
> var WorldUp : Real3


---  
 #  Methods


---  
 #  ComputeSignedAngle : [real](../nada_base_types/real.md)

> Compute the rotation angle between two vectors (in radians)
> |Name|Type|Description|
> |---|---|---|
> |up|[real3](../nada_base_types/real3.md)| |
> |forward|[real3](../nada_base_types/real3.md)| |
> |newVector|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function ComputeSignedAngle(up : Real3, forward : Real3, newVector : Real3) : Real
> ``` 


---  
 #  DebugDrawBases : Void

> Debug draws the current orientation bases in world space.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function DebugDrawBases()
> ``` 


---  
 #  GetLookAtDirectionRotation : [quaternion](../nada_base_types/quaternion.md)

> Gets the forward to look in the given direction. Keeps the current world up.
> |Name|Type|Description|
> |---|---|---|
> |lookDir|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function GetLookAtDirectionRotation(lookDir : Real3) : Quaternion
> ``` 


---  
 #  GetLookAtDirectionWithUpRotation : [quaternion](../nada_base_types/quaternion.md)

> Same as GetLookAtDirectionRotation but allows the user to specify the up vector.
> |Name|Type|Description|
> |---|---|---|
> |lookDir|[real3](../nada_base_types/real3.md)| |
> |up|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function GetLookAtDirectionWithUpRotation(lookDir : Real3, up : Real3) : Quaternion
> ``` 


---  
 #  GetLookAtPointRotation : [quaternion](../nada_base_types/quaternion.md)

> Get the rotation so that the forward will look at the given point. Keeps the current world up.
> |Name|Type|Description|
> |---|---|---|
> |lookPoint|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function GetLookAtPointRotation(lookPoint : Real3) : Quaternion
> ``` 


---  
 #  GetLookAtPointWithUpRotation : [quaternion](../nada_base_types/quaternion.md)

> Same as GetLookAtPointRotation but allows the user to specify the up vector.
> |Name|Type|Description|
> |---|---|---|
> |lookPoint|[real3](../nada_base_types/real3.md)| |
> |up|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function GetLookAtPointWithUpRotation(lookPoint : Real3, up : Real3) : Quaternion
> ``` 


---  
 #  LookAtDirection : Void

> Sets the forward to look in the given direction. Keeps the current world up.
> |Name|Type|Description|
> |---|---|---|
> |lookDir|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function LookAtDirection(lookDir : Real3)
> ``` 


---  
 #  LookAtDirectionWithUp : Void

> Same as LookAtDirection but allows the user to specify the up vector.
> |Name|Type|Description|
> |---|---|---|
> |lookDir|[real3](../nada_base_types/real3.md)| |
> |up|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function LookAtDirectionWithUp(lookDir : Real3, up : Real3)
> ``` 


---  
 #  LookAtPoint : Void

> Sets the forward to look at the given point. Keeps the current world up.
> |Name|Type|Description|
> |---|---|---|
> |lookPoint|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function LookAtPoint(lookPoint : Real3)
> ``` 


---  
 #  LookAtPointWithUp : Void

> Same as LookAtPoint but allows the user to specify the up vector.
> |Name|Type|Description|
> |---|---|---|
> |lookPoint|[real3](../nada_base_types/real3.md)| |
> |up|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function LookAtPointWithUp(lookPoint : Real3, up : Real3)
> ``` 


---  
 #  Orientation : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Orientation()
> ``` 


---  
 #  SetLocalLookAtRotation : Void

> Set the transform's local rotation such that the orientation's basis vectors will be aligned with the given rotation (assumed to be a look-at rotation constructed from a right, up, and forward)
> |Name|Type|Description|
> |---|---|---|
> |localLookAtRotation|[quaternion](../nada_base_types/quaternion.md)| |
> ```TS:Nada
> function SetLocalLookAtRotation(localLookAtRotation : Quaternion)
> ``` 


---  
 #  SetWorldLookAtRotation : Void

> Set the transform's world rotation such that the orientation's basis vectors will be aligned with the given rotation (assumed to be a look-at rotation constructed from a right, up, and forward)
> |Name|Type|Description|
> |---|---|---|
> |worldLookAtRotation|[quaternion](../nada_base_types/quaternion.md)| |
> ```TS:Nada
> function SetWorldLookAtRotation(worldLookAtRotation : Quaternion)
> ``` 


---  
 

 
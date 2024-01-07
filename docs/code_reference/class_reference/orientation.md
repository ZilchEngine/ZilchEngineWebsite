 `Component` `Gameplay`



(NOTE) Defines a new basis for a desired right, up, and forward vector. Provides a bunch of helper functions to change between these spaces and to perform simple look-at behavior.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ComputeSignedAngle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#computesignedangle-zero)|[ AbsoluteAngle](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#absoluteangle-zilch-engin)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)| |
|[ DebugDrawBases](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#debugdrawbases-void)|[ DefaultOrientationBases](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#defaultorientationbases)| | |
|[ GetLookAtDirectionRotation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#getlookatdirectionrotati)|[ GlobalUp](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#globalup-zilch-engine-doc)| | |
|[ GetLookAtDirectionWithUpRotation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#getlookatdirectionwithup)|[ LocalForward](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#localforward-zilch-engine)| | |
|[ GetLookAtPointRotation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#getlookatpointrotation-z)|[ LocalOrientationBasis](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#localorientationbasis-ze)| | |
|[ GetLookAtPointWithUpRotation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#getlookatpointwithuprota)|[ LocalRight](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#localright-zilch-engine-d)| | |
|[ LookAtDirection](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#lookatdirection-void)|[ LocalToOrientationRotation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#localtoorientationrotati)| | |
|[ LookAtDirectionWithUp](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#lookatdirectionwithup-vo)|[ LocalToWorldRotation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#localtoworldrotation-zer)| | |
|[ LookAtPoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#lookatpoint-void)|[ LocalUp](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#localup-zilch-engine-docu)| | |
|[ LookAtPointWithUp](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#lookatpointwithup-void)|[ OrientationForward](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#orientationforward-zero)| | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#orientation-void)|[ OrientationRight](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#orientationright-zilch-en)| | |
|[ SetLocalLookAtRotation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#setlocallookatrotation-v)|[ OrientationToLocalRotation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#orientationtolocalrotati)| | |
|[ SetWorldLookAtRotation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#setworldlookatrotation-v)|[ OrientationToWorldRotation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#orientationtoworldrotati)| | |
| |[ OrientationUp](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#orientationup-zilch-engin)| | |
| |[ WorldForward](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#worldforward-zilch-engine)| | |
| |[ WorldRight](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#worldright-zilch-engine-d)| | |
| |[ WorldToLocalRotation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#worldtolocalrotation-zer)| | |
| |[ WorldToOrientationRotation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#worldtoorientationrotati)| | |
| |[ WorldUp](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/orientation.md#worldup-zilch-engine-docu)| | |


 #  Properties


---  
 #  AbsoluteAngle : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

 `read-only`

> Get the angle of the object about the up vector.
> ``` lang=cpp, name=Nada
> var AbsoluteAngle : Real


---  
 #  DefaultOrientationBases : [OrientationBases](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#orientationbases)

> 
> ``` lang=cpp, name=Nada
> var DefaultOrientationBases : OrientationBases


---  
 #  GlobalUp : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The world-space up vector to use for LookAt operations that don't take an up vector.
> ``` lang=cpp, name=Nada
> var GlobalUp : Real3


---  
 #  LocalForward : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

 `read-only`

> The orientation's forward vector after having been transformed into local space.
> ``` lang=cpp, name=Nada
> var LocalForward : Real3


---  
 #  LocalOrientationBasis : [quaternion](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/quaternion.md)

> A local-space basis that represents this orientation. If you build a basis from an up of (0, 1, 0), and a forward of (0, 0, -1) then this should result in the identity rotation.
> ``` lang=cpp, name=Nada
> var LocalOrientationBasis : Quaternion


---  
 #  LocalRight : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

 `read-only`

> The orientation's right vector after having been transformed into local space.
> ``` lang=cpp, name=Nada
> var LocalRight : Real3


---  
 #  LocalToOrientationRotation : [quaternion](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/quaternion.md)

 `read-only`

> The rotation that takes an local space vector into orientation space. For example, this transforms LocalRight into OrientationRight.
> ``` lang=cpp, name=Nada
> var LocalToOrientationRotation : Quaternion


---  
 #  LocalToWorldRotation : [quaternion](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/quaternion.md)

 `read-only`

> The rotation that transforms a vector from local space into world space. For example, this transforms LocalRight into WorldRight.
> ``` lang=cpp, name=Nada
> var LocalToWorldRotation : Quaternion


---  
 #  LocalUp : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

 `read-only`

> The orientation's up vector after having been transformed into local space.
> ``` lang=cpp, name=Nada
> var LocalUp : Real3


---  
 #  OrientationForward : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

 `read-only`

> The forward vector in orientation space. This is always the vector (0, 0, -1) but is provided for clarity with transformations.
> ``` lang=cpp, name=Nada
> var OrientationForward : Real3


---  
 #  OrientationRight : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

 `read-only`

> The right vector in orientation space. This is always the vector (1, 0, 0) but is provided for clarity with transformations.
> ``` lang=cpp, name=Nada
> var OrientationRight : Real3


---  
 #  OrientationToLocalRotation : [quaternion](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/quaternion.md)

 `read-only`

> The rotation that takes an orientation space vector into local space. For example, this transforms OrientationRight into LocalRight.
> ``` lang=cpp, name=Nada
> var OrientationToLocalRotation : Quaternion


---  
 #  OrientationToWorldRotation : [quaternion](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/quaternion.md)

 `read-only`

> The rotation that takes an orientation space vector into world space. For example, this transforms OrientationRight into WorldRight.
> ``` lang=cpp, name=Nada
> var OrientationToWorldRotation : Quaternion


---  
 #  OrientationUp : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

 `read-only`

> The up vector in orientation space. This is always the vector (0, 1, 0) but is provided for clarity with transformations.
> ``` lang=cpp, name=Nada
> var OrientationUp : Real3


---  
 #  WorldForward : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

 `read-only`

> The orientation's forward vector after having been transformed into world space.
> ``` lang=cpp, name=Nada
> var WorldForward : Real3


---  
 #  WorldRight : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

 `read-only`

> The orientation's right vector after having been transformed into world space.
> ``` lang=cpp, name=Nada
> var WorldRight : Real3


---  
 #  WorldToLocalRotation : [quaternion](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/quaternion.md)

 `read-only`

> The rotation that transforms a vector from world space into local space. For example, this transforms WorldRight into LocalRight.
> ``` lang=cpp, name=Nada
> var WorldToLocalRotation : Quaternion


---  
 #  WorldToOrientationRotation : [quaternion](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/quaternion.md)

 `read-only`

> The rotation that takes an world space vector into orientation space. For example, this transforms WorldRight into OrientationRight.
> ``` lang=cpp, name=Nada
> var WorldToOrientationRotation : Quaternion


---  
 #  WorldUp : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

 `read-only`

> The orientation's up vector after having been transformed into world space.
> ``` lang=cpp, name=Nada
> var WorldUp : Real3


---  
 #  Methods


---  
 #  ComputeSignedAngle : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Compute the rotation angle between two vectors (in radians)
> |Name|Type|Description|
> |---|---|---|
> |up|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |forward|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |newVector|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function ComputeSignedAngle(up : Real3, forward : Real3, newVector : Real3) : Real
> ``` 


---  
 #  DebugDrawBases : Void

> Debug draws the current orientation bases in world space.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function DebugDrawBases()
> ``` 


---  
 #  GetLookAtDirectionRotation : [quaternion](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/quaternion.md)

> Gets the forward to look in the given direction. Keeps the current world up.
> |Name|Type|Description|
> |---|---|---|
> |lookDir|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function GetLookAtDirectionRotation(lookDir : Real3) : Quaternion
> ``` 


---  
 #  GetLookAtDirectionWithUpRotation : [quaternion](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/quaternion.md)

> Same as GetLookAtDirectionRotation but allows the user to specify the up vector.
> |Name|Type|Description|
> |---|---|---|
> |lookDir|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |up|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function GetLookAtDirectionWithUpRotation(lookDir : Real3, up : Real3) : Quaternion
> ``` 


---  
 #  GetLookAtPointRotation : [quaternion](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/quaternion.md)

> Get the rotation so that the forward will look at the given point. Keeps the current world up.
> |Name|Type|Description|
> |---|---|---|
> |lookPoint|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function GetLookAtPointRotation(lookPoint : Real3) : Quaternion
> ``` 


---  
 #  GetLookAtPointWithUpRotation : [quaternion](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/quaternion.md)

> Same as GetLookAtPointRotation but allows the user to specify the up vector.
> |Name|Type|Description|
> |---|---|---|
> |lookPoint|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |up|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function GetLookAtPointWithUpRotation(lookPoint : Real3, up : Real3) : Quaternion
> ``` 


---  
 #  LookAtDirection : Void

> Sets the forward to look in the given direction. Keeps the current world up.
> |Name|Type|Description|
> |---|---|---|
> |lookDir|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function LookAtDirection(lookDir : Real3)
> ``` 


---  
 #  LookAtDirectionWithUp : Void

> Same as LookAtDirection but allows the user to specify the up vector.
> |Name|Type|Description|
> |---|---|---|
> |lookDir|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |up|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function LookAtDirectionWithUp(lookDir : Real3, up : Real3)
> ``` 


---  
 #  LookAtPoint : Void

> Sets the forward to look at the given point. Keeps the current world up.
> |Name|Type|Description|
> |---|---|---|
> |lookPoint|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function LookAtPoint(lookPoint : Real3)
> ``` 


---  
 #  LookAtPointWithUp : Void

> Same as LookAtPoint but allows the user to specify the up vector.
> |Name|Type|Description|
> |---|---|---|
> |lookPoint|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |up|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function LookAtPointWithUp(lookPoint : Real3, up : Real3)
> ``` 


---  
 #  Orientation : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Orientation()
> ``` 


---  
 #  SetLocalLookAtRotation : Void

> Set the transform's local rotation such that the orientation's basis vectors will be aligned with the given rotation (assumed to be a look-at rotation constructed from a right, up, and forward)
> |Name|Type|Description|
> |---|---|---|
> |localLookAtRotation|[quaternion](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/quaternion.md)| |
> ``` lang=cpp, name=Nada
> function SetLocalLookAtRotation(localLookAtRotation : Quaternion)
> ``` 


---  
 #  SetWorldLookAtRotation : Void

> Set the transform's world rotation such that the orientation's basis vectors will be aligned with the given rotation (assumed to be a look-at rotation constructed from a right, up, and forward)
> |Name|Type|Description|
> |---|---|---|
> |worldLookAtRotation|[quaternion](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/quaternion.md)| |
> ``` lang=cpp, name=Nada
> function SetWorldLookAtRotation(worldLookAtRotation : Quaternion)
> ``` 


---  
 

 
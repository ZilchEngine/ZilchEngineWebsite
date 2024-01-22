 `Component` `Engine`



(NOTE) Transform component class. The transform component provides the position, rotation and scale of an object.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[RotateAnglesLocal](transform.md#rotateangleslocal-void)|[EulerAngles](transform.md#eulerangles-zilch-engine)|[component](component.md)| |
|[RotateAnglesWorld](transform.md#rotateanglesworld-void)|[LocalRotation](transform.md#localrotation-zilch-engin)| | |
|[RotateAround](transform.md#rotatearound-void)|[LocalScale](transform.md#localscale-zilch-engine-d)| | |
|[RotateLocal](transform.md#rotatelocal-void)|[LocalTranslation](transform.md#localtranslation-zilch-en)| | |
|[RotateWorld](transform.md#rotateworld-void)|[Parent](transform.md#parent-zilch-engine-docum)| | |
|[SetEulerAnglesXYZ](transform.md#seteuleranglesxyz-void)|[Rotation](transform.md#rotation-zilch-engine-doc)| | |
|[SetRotationBases](transform.md#setrotationbases-void)|[Scale](transform.md#scale-zilch-engine-docume)| | |
|[Constructor](transform.md#transform-void)|[Translation](transform.md#translation-zilch-engine)| | |
|[TransformNormal](transform.md#transformnormal-zilch-eng)|[WorldMatrix](transform.md#worldmatrix-zilch-engine)| | |
|[TransformNormalInverse](transform.md#transformnormalinverse-z)|[WorldRotation](transform.md#worldrotation-zilch-engin)| | |
|[TransformNormalLocal](transform.md#transformnormallocal-zer)|[WorldScale](transform.md#worldscale-zilch-engine-d)| | |
|[TransformPoint](transform.md#transformpoint-zilch-engi)|[WorldTranslation](transform.md#worldtranslation-zilch-en)| | |
|[TransformPointInverse](transform.md#transformpointinverse-ze)| | | |
|[TransformPointLocal](transform.md#transformpointlocal-zero)| | | |


 #  Properties


---  
 #  EulerAngles : [real3](../nada_base_types/real3.md)

> The rotation of the transform as an Euler angle vector in radians.
> ```TS:Nada
> var EulerAngles : Real3


---  
 #  LocalRotation : [quaternion](../nada_base_types/quaternion.md)

> Local rotation relative to parent.
> ```TS:Nada
> var LocalRotation : Quaternion


---  
 #  LocalScale : [real3](../nada_base_types/real3.md)

> Local Scale relative to parent.
> ```TS:Nada
> var LocalScale : Real3


---  
 #  LocalTranslation : [real3](../nada_base_types/real3.md)

> Local Translation relative to parent.
> ```TS:Nada
> var LocalTranslation : Real3


---  
 #  Parent : [transform](transform.md)

 `read-only`

> 
> ```TS:Nada
> var Parent : Transform


---  
 #  Rotation : [quaternion](../nada_base_types/quaternion.md)

> Local rotation relative to parent.
> ```TS:Nada
> var Rotation : Quaternion


---  
 #  Scale : [real3](../nada_base_types/real3.md)

> Local Scale relative to parent.
> ```TS:Nada
> var Scale : Real3


---  
 #  Translation : [real3](../nada_base_types/real3.md)

> Local Translation relative to parent.
> ```TS:Nada
> var Translation : Real3


---  
 #  WorldMatrix : [real4x4](../nada_base_types/real4x4.md)

 `read-only`

> 
> ```TS:Nada
> var WorldMatrix : Real4x4


---  
 #  WorldRotation : [quaternion](../nada_base_types/quaternion.md)

> Rotation in World Space.
> ```TS:Nada
> var WorldRotation : Quaternion


---  
 #  WorldScale : [real3](../nada_base_types/real3.md)

> Scale in World Space.
> ```TS:Nada
> var WorldScale : Real3


---  
 #  WorldTranslation : [real3](../nada_base_types/real3.md)

> Translation in World Space.
> ```TS:Nada
> var WorldTranslation : Real3


---  
 #  Methods


---  
 #  RotateAnglesLocal : Void

> Rotate object in local space by the given Euler angle vector (in radians).
> |Name|Type|Description|
> |---|---|---|
> |angles|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function RotateAnglesLocal(angles : Real3)
> ``` 


---  
 #  RotateAnglesWorld : Void

> Rotate object in world space by the given Euler angle vector (in radians).
> |Name|Type|Description|
> |---|---|---|
> |angles|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function RotateAnglesWorld(angles : Real3)
> ``` 


---  
 #  RotateAround : Void

> Rotate around a given point with the given rotation.
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](../nada_base_types/real3.md)| |
> |rotation|[quaternion](../nada_base_types/quaternion.md)| |
> ```TS:Nada
> function RotateAround(point : Real3, rotation : Quaternion)
> ``` 


---  
 #  RotateLocal : Void

> Rotate object in local space.
> |Name|Type|Description|
> |---|---|---|
> |rotation|[quaternion](../nada_base_types/quaternion.md)| |
> ```TS:Nada
> function RotateLocal(rotation : Quaternion)
> ``` 


---  
 #  RotateWorld : Void

> Rotate object in world space.
> |Name|Type|Description|
> |---|---|---|
> |rotation|[quaternion](../nada_base_types/quaternion.md)| |
> ```TS:Nada
> function RotateWorld(rotation : Quaternion)
> ``` 


---  
 #  SetEulerAnglesXYZ : Void

> Sets the rotation of the transform by the given Euler angles in radians.
> |Name|Type|Description|
> |---|---|---|
> |xRadians|[real](../nada_base_types/real.md)| |
> |yRadians|[real](../nada_base_types/real.md)| |
> |zRadians|[real](../nada_base_types/real.md)| |
> ```TS:Nada
> function SetEulerAnglesXYZ(xRadians : Real, yRadians : Real, zRadians : Real)
> ``` 


---  
 #  SetRotationBases : Void

> Generates a rotation matrix from the given bases.
> |Name|Type|Description|
> |---|---|---|
> |facing|[real3](../nada_base_types/real3.md)| |
> |up|[real3](../nada_base_types/real3.md)| |
> |right|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function SetRotationBases(facing : Real3, up : Real3, right : Real3)
> ``` 


---  
 #  Transform : Void

 `constructor`

> Constructor / Destructor.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Transform()
> ``` 


---  
 #  TransformNormal : [real3](../nada_base_types/real3.md)

> Transforms a local normal (direction) into world space.
> |Name|Type|Description|
> |---|---|---|
> |normal|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function TransformNormal(normal : Real3) : Real3
> ``` 


---  
 #  TransformNormalInverse : [real3](../nada_base_types/real3.md)

> Transforms a world normal (direction) into local space.
> |Name|Type|Description|
> |---|---|---|
> |normal|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function TransformNormalInverse(normal : Real3) : Real3
> ``` 


---  
 #  TransformNormalLocal : [real3](../nada_base_types/real3.md)

> Transforms a normal by the local matrix (ignores parent's transform) Needed now because there is no quaternion times vector in script.
> |Name|Type|Description|
> |---|---|---|
> |normal|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function TransformNormalLocal(normal : Real3) : Real3
> ``` 


---  
 #  TransformPoint : [real3](../nada_base_types/real3.md)

> Transforms a local point into world space.
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function TransformPoint(point : Real3) : Real3
> ``` 


---  
 #  TransformPointInverse : [real3](../nada_base_types/real3.md)

> Transforms a world point into local space.
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function TransformPointInverse(point : Real3) : Real3
> ``` 


---  
 #  TransformPointLocal : [real3](../nada_base_types/real3.md)

> Transforms a point by the local matrix (ignores parent's transform)
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](../nada_base_types/real3.md)| |
> ```TS:Nada
> function TransformPointLocal(point : Real3) : Real3
> ``` 


---  
 

 
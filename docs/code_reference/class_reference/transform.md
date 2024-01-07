 `Component` `Engine`



(NOTE) Transform component class. The transform component provides the position, rotation and scale of an object.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ RotateAnglesLocal](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md#rotateangleslocal-void)|[ EulerAngles](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md#eulerangles-zilch-engine)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)| |
|[ RotateAnglesWorld](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md#rotateanglesworld-void)|[ LocalRotation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md#localrotation-zilch-engin)| | |
|[ RotateAround](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md#rotatearound-void)|[ LocalScale](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md#localscale-zilch-engine-d)| | |
|[ RotateLocal](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md#rotatelocal-void)|[ LocalTranslation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md#localtranslation-zilch-en)| | |
|[ RotateWorld](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md#rotateworld-void)|[ Parent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md#parent-zilch-engine-docum)| | |
|[ SetEulerAnglesXYZ](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md#seteuleranglesxyz-void)|[ Rotation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md#rotation-zilch-engine-doc)| | |
|[ SetRotationBases](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md#setrotationbases-void)|[ Scale](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md#scale-zilch-engine-docume)| | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md#transform-void)|[ Translation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md#translation-zilch-engine)| | |
|[ TransformNormal](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md#transformnormal-zilch-eng)|[ WorldMatrix](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md#worldmatrix-zilch-engine)| | |
|[ TransformNormalInverse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md#transformnormalinverse-z)|[ WorldRotation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md#worldrotation-zilch-engin)| | |
|[ TransformNormalLocal](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md#transformnormallocal-zer)|[ WorldScale](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md#worldscale-zilch-engine-d)| | |
|[ TransformPoint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md#transformpoint-zilch-engi)|[ WorldTranslation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md#worldtranslation-zilch-en)| | |
|[ TransformPointInverse](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md#transformpointinverse-ze)| | | |
|[ TransformPointLocal](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md#transformpointlocal-zero)| | | |


 #  Properties


---  
 #  EulerAngles : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The rotation of the transform as an Euler angle vector in radians.
> ``` lang=cpp, name=Nada
> var EulerAngles : Real3


---  
 #  LocalRotation : [quaternion](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/quaternion.md)

> Local rotation relative to parent.
> ``` lang=cpp, name=Nada
> var LocalRotation : Quaternion


---  
 #  LocalScale : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Local Scale relative to parent.
> ``` lang=cpp, name=Nada
> var LocalScale : Real3


---  
 #  LocalTranslation : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Local Translation relative to parent.
> ``` lang=cpp, name=Nada
> var LocalTranslation : Real3


---  
 #  Parent : [transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Parent : Transform


---  
 #  Rotation : [quaternion](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/quaternion.md)

> Local rotation relative to parent.
> ``` lang=cpp, name=Nada
> var Rotation : Quaternion


---  
 #  Scale : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Local Scale relative to parent.
> ``` lang=cpp, name=Nada
> var Scale : Real3


---  
 #  Translation : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Local Translation relative to parent.
> ``` lang=cpp, name=Nada
> var Translation : Real3


---  
 #  WorldMatrix : [real4x4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4x4.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var WorldMatrix : Real4x4


---  
 #  WorldRotation : [quaternion](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/quaternion.md)

> Rotation in World Space.
> ``` lang=cpp, name=Nada
> var WorldRotation : Quaternion


---  
 #  WorldScale : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Scale in World Space.
> ``` lang=cpp, name=Nada
> var WorldScale : Real3


---  
 #  WorldTranslation : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Translation in World Space.
> ``` lang=cpp, name=Nada
> var WorldTranslation : Real3


---  
 #  Methods


---  
 #  RotateAnglesLocal : Void

> Rotate object in local space by the given Euler angle vector (in radians).
> |Name|Type|Description|
> |---|---|---|
> |angles|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function RotateAnglesLocal(angles : Real3)
> ``` 


---  
 #  RotateAnglesWorld : Void

> Rotate object in world space by the given Euler angle vector (in radians).
> |Name|Type|Description|
> |---|---|---|
> |angles|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function RotateAnglesWorld(angles : Real3)
> ``` 


---  
 #  RotateAround : Void

> Rotate around a given point with the given rotation.
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |rotation|[quaternion](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/quaternion.md)| |
> ``` lang=cpp, name=Nada
> function RotateAround(point : Real3, rotation : Quaternion)
> ``` 


---  
 #  RotateLocal : Void

> Rotate object in local space.
> |Name|Type|Description|
> |---|---|---|
> |rotation|[quaternion](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/quaternion.md)| |
> ``` lang=cpp, name=Nada
> function RotateLocal(rotation : Quaternion)
> ``` 


---  
 #  RotateWorld : Void

> Rotate object in world space.
> |Name|Type|Description|
> |---|---|---|
> |rotation|[quaternion](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/quaternion.md)| |
> ``` lang=cpp, name=Nada
> function RotateWorld(rotation : Quaternion)
> ``` 


---  
 #  SetEulerAnglesXYZ : Void

> Sets the rotation of the transform by the given Euler angles in radians.
> |Name|Type|Description|
> |---|---|---|
> |xRadians|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |yRadians|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |zRadians|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function SetEulerAnglesXYZ(xRadians : Real, yRadians : Real, zRadians : Real)
> ``` 


---  
 #  SetRotationBases : Void

> Generates a rotation matrix from the given bases.
> |Name|Type|Description|
> |---|---|---|
> |facing|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |up|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> |right|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function SetRotationBases(facing : Real3, up : Real3, right : Real3)
> ``` 


---  
 #  Transform : Void

 `constructor`

> Constructor / Destructor.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Transform()
> ``` 


---  
 #  TransformNormal : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Transforms a local normal (direction) into world space.
> |Name|Type|Description|
> |---|---|---|
> |normal|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function TransformNormal(normal : Real3) : Real3
> ``` 


---  
 #  TransformNormalInverse : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Transforms a world normal (direction) into local space.
> |Name|Type|Description|
> |---|---|---|
> |normal|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function TransformNormalInverse(normal : Real3) : Real3
> ``` 


---  
 #  TransformNormalLocal : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Transforms a normal by the local matrix (ignores parent's transform) Needed now because there is no quaternion times vector in script.
> |Name|Type|Description|
> |---|---|---|
> |normal|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function TransformNormalLocal(normal : Real3) : Real3
> ``` 


---  
 #  TransformPoint : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Transforms a local point into world space.
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function TransformPoint(point : Real3) : Real3
> ``` 


---  
 #  TransformPointInverse : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Transforms a world point into local space.
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function TransformPointInverse(point : Real3) : Real3
> ``` 


---  
 #  TransformPointLocal : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Transforms a point by the local matrix (ignores parent's transform)
> |Name|Type|Description|
> |---|---|---|
> |point|[real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function TransformPointLocal(point : Real3) : Real3
> ``` 


---  
 

 
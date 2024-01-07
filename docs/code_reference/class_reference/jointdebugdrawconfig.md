 `Component` `Physics`



(NOTE) Allows the user to override parameters for debug drawing of joints. Primarily used to debug draw from different object perspectives and to change the size of drawn data.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointdebugdrawconfig.md#jointdebugdrawconfig-voi)|[ Active](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointdebugdrawconfig.md#active-zilch-engine-docum)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)| |
| |[ Detail](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointdebugdrawconfig.md#detail-zilch-engine-docum)| | |
| |[ ObjectAPerspective](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointdebugdrawconfig.md#objectaperspective-zero)| | |
| |[ ObjectBPerspective](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointdebugdrawconfig.md#objectbperspective-zero)| | |
| |[ Size](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointdebugdrawconfig.md#size-zilch-engine-documen)| | |


 #  Properties


---  
 #  Active : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Whether or not this component is active.
> ``` lang=cpp, name=Nada
> var Active : Boolean


---  
 #  Detail : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The amount of detail to use when drawing. For example, the detail on a RevoluteJoint will increase the number of lines used to draw the arc of a circle.
> ``` lang=cpp, name=Nada
> var Detail : Real


---  
 #  ObjectAPerspective : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> If we draw the joint's debug info from the perspective of ObjectA. Typically used when ObjectA is marked as a static object and ObjectB has free movement.
> ``` lang=cpp, name=Nada
> var ObjectAPerspective : Boolean


---  
 #  ObjectBPerspective : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> If we draw the joint's debug info from the perspective of ObjectB. Typically used when ObjectB is marked as a static object and ObjectA has free movement.
> ``` lang=cpp, name=Nada
> var ObjectBPerspective : Boolean


---  
 #  Size : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> A size modifier for the debug drawing. 1 is the base size.
> ``` lang=cpp, name=Nada
> var Size : Real


---  
 #  Methods


---  
 #  JointDebugDrawConfig : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function JointDebugDrawConfig()
> ``` 


---  
 

 
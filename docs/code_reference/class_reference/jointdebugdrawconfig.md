 `Component` `Physics`



(NOTE) Allows the user to override parameters for debug drawing of joints. Primarily used to debug draw from different object perspectives and to change the size of drawn data.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Constructor](jointdebugdrawconfig.md#jointdebugdrawconfig-voi)|[Active](jointdebugdrawconfig.md#active-zilch-engine-docum)|[component](component.md)| |
| |[Detail](jointdebugdrawconfig.md#detail-zilch-engine-docum)| | |
| |[ObjectAPerspective](jointdebugdrawconfig.md#objectaperspective-zero)| | |
| |[ObjectBPerspective](jointdebugdrawconfig.md#objectbperspective-zero)| | |
| |[Size](jointdebugdrawconfig.md#size-zilch-engine-documen)| | |


 #  Properties


---  
 #  Active : [boolean](../nada_base_types/boolean.md)

> Whether or not this component is active.
> ```TS:Nada
> var Active : Boolean


---  
 #  Detail : [real](../nada_base_types/real.md)

> The amount of detail to use when drawing. For example, the detail on a RevoluteJoint will increase the number of lines used to draw the arc of a circle.
> ```TS:Nada
> var Detail : Real


---  
 #  ObjectAPerspective : [boolean](../nada_base_types/boolean.md)

> If we draw the joint's debug info from the perspective of ObjectA. Typically used when ObjectA is marked as a static object and ObjectB has free movement.
> ```TS:Nada
> var ObjectAPerspective : Boolean


---  
 #  ObjectBPerspective : [boolean](../nada_base_types/boolean.md)

> If we draw the joint's debug info from the perspective of ObjectB. Typically used when ObjectB is marked as a static object and ObjectA has free movement.
> ```TS:Nada
> var ObjectBPerspective : Boolean


---  
 #  Size : [real](../nada_base_types/real.md)

> A size modifier for the debug drawing. 1 is the base size.
> ```TS:Nada
> var Size : Real


---  
 #  Methods


---  
 #  JointDebugDrawConfig : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function JointDebugDrawConfig()
> ``` 


---  
 

 
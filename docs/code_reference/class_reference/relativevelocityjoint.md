 `Component` `Physics`



(NOTE) A relative velocity joint defines what the desired relative velocity on three world axes should be between two objects. Relative velocity is defined as v2 - v1. This joint has not been tested with motors or limits in any way.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetAxis](relativevelocityjoint.md#getaxis-zilch-engine-docu)| |[joint](joint.md)| |
|[ GetAxisActive](relativevelocityjoint.md#getaxisactive-zilch-engin)| | | |
|[ GetMaxImpulse](relativevelocityjoint.md#getmaximpulse-zilch-engin)| | | |
|[ GetSpeed](relativevelocityjoint.md#getspeed-zilch-engine-doc)| | | |
|[ Constructor](relativevelocityjoint.md#relativevelocityjoint-vo)| | | |
|[ SetAxis](relativevelocityjoint.md#setaxis-void)| | | |
|[ SetAxisActive](relativevelocityjoint.md#setaxisactive-void)| | | |
|[ SetMaxImpulse](relativevelocityjoint.md#setmaximpulse-void)| | | |
|[ SetSpeed](relativevelocityjoint.md#setspeed-void)| | | |


 #  Properties


---  
 #  Methods


---  
 #  GetAxis : [real3](../nada_base_types/real3.md)

> One of 3 axes to constrain movement on.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function GetAxis(index : Integer) : Real3
> ``` 


---  
 #  GetAxisActive : [boolean](../nada_base_types/boolean.md)

> Whether or not the given axis index is active.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function GetAxisActive(index : Integer) : Boolean
> ``` 


---  
 #  GetMaxImpulse : [real](../nada_base_types/real.md)

> The max impulse for the given axis index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function GetMaxImpulse(index : Integer) : Real
> ``` 


---  
 #  GetSpeed : [real](../nada_base_types/real.md)

> The desired relative speed for the given axis index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function GetSpeed(index : Integer) : Real
> ``` 


---  
 #  RelativeVelocityJoint : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function RelativeVelocityJoint()
> ``` 


---  
 #  SetAxis : Void

> One of 3 axes to constrain movement on.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> |axis|[real3](../nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function SetAxis(index : Integer, axis : Real3)
> ``` 


---  
 #  SetAxisActive : Void

> Whether or not the given axis index is active.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> |active|[boolean](../nada_base_types/boolean.md)| |
> ``` lang=cpp, name=Nada
> function SetAxisActive(index : Integer, active : Boolean)
> ``` 


---  
 #  SetMaxImpulse : Void

> The max impulse for the given axis index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> |maxImpulse|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function SetMaxImpulse(index : Integer, maxImpulse : Real)
> ``` 


---  
 #  SetSpeed : Void

> The desired relative speed for the given axis index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> |speed|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function SetSpeed(index : Integer, speed : Real)
> ``` 


---  
 

 
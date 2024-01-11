 `Engine`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Clone](animationnode.md#clone-zilch-engine-docume)|[ CollapseToPoseOnFinish](animationnode.md#collapsetoposeonfinish-z)|[referencecountedeventobject](referencecountedeventobject.md)|[basicanimation](basicanimation.md)|
|[ CollapseToPose](animationnode.md#collapsetopose-void)|[ Duration](animationnode.md#duration-zilch-engine-doc)| |[dualblendchainnode](dualblendchainnode.md)|
|[ GetNormalizedTime](animationnode.md#getnormalizedtime-zilch-e)|[ Paused](animationnode.md#paused-zilch-engine-docum)| |[dualblendcrossblend](dualblendcrossblend.md)|
|[ IsActive](animationnode.md#isactive-zilch-engine-doc)|[ Time](animationnode.md#time-zilch-engine-documen)| |[dualblenddirectblend](dualblenddirectblend.md)|
|[ PrintNode](animationnode.md#printnode-void)|[ TimeScale](animationnode.md#timescale-zilch-engine-do)| |[dualblendselectivenode](dualblendselectivenode.md)|
|[ SetNormalizedTime](animationnode.md#setnormalizedtime-void)| | |[posenode](posenode.md)|


 #  Properties


---  
 #  CollapseToPoseOnFinish : [boolean](../nada_base_types/boolean.md)

> Whether or not to collapse to a pose node when finished playing.
> ``` lang=cpp, name=Nada
> var CollapseToPoseOnFinish : Boolean


---  
 #  Duration : [real](../nada_base_types/real.md)

> The duration of the node.
> ``` lang=cpp, name=Nada
> var Duration : Real


---  
 #  Paused : [boolean](../nada_base_types/boolean.md)

> Whether or not the node is currently paused.
> ``` lang=cpp, name=Nada
> var Paused : Boolean


---  
 #  Time : [real](../nada_base_types/real.md)

> The current time in the node.
> ``` lang=cpp, name=Nada
> var Time : Real


---  
 #  TimeScale : [real](../nada_base_types/real.md)

> A scalar to dt when updating the node.
> ``` lang=cpp, name=Nada
> var TimeScale : Real


---  
 #  Methods


---  
 #  Clone : [animationnode](animationnode.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Clone() : AnimationNode
> ``` 


---  
 #  CollapseToPose : Void

> Collapses all children to a pose node on the next Update.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function CollapseToPose()
> ``` 


---  
 #  GetNormalizedTime : [real](../nada_base_types/real.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function GetNormalizedTime() : Real
> ``` 


---  
 #  IsActive : [boolean](../nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function IsActive() : Boolean
> ``` 


---  
 #  PrintNode : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |tabs|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function PrintNode(tabs : Integer)
> ``` 


---  
 #  SetNormalizedTime : Void

> A value between [0-1].
> |Name|Type|Description|
> |---|---|---|
> |normalizedTime|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function SetNormalizedTime(normalizedTime : Real)
> ``` 


---  
 

 
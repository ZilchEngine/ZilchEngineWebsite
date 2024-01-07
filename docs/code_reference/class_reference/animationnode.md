 `Engine`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Clone](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationnode.md#clone-zilch-engine-docume)|[ CollapseToPoseOnFinish](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationnode.md#collapsetoposeonfinish-z)|[referencecountedeventobject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/referencecountedeventobject.md)|[basicanimation](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/basicanimation.md)|
|[ CollapseToPose](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationnode.md#collapsetopose-void)|[ Duration](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationnode.md#duration-zilch-engine-doc)| |[dualblendchainnode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/dualblendchainnode.md)|
|[ GetNormalizedTime](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationnode.md#getnormalizedtime-zilch-e)|[ Paused](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationnode.md#paused-zilch-engine-docum)| |[dualblendcrossblend](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/dualblendcrossblend.md)|
|[ IsActive](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationnode.md#isactive-zilch-engine-doc)|[ Time](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationnode.md#time-zilch-engine-documen)| |[dualblenddirectblend](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/dualblenddirectblend.md)|
|[ PrintNode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationnode.md#printnode-void)|[ TimeScale](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationnode.md#timescale-zilch-engine-do)| |[dualblendselectivenode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/dualblendselectivenode.md)|
|[ SetNormalizedTime](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationnode.md#setnormalizedtime-void)| | |[posenode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/posenode.md)|


 #  Properties


---  
 #  CollapseToPoseOnFinish : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Whether or not to collapse to a pose node when finished playing.
> ``` lang=cpp, name=Nada
> var CollapseToPoseOnFinish : Boolean


---  
 #  Duration : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The duration of the node.
> ``` lang=cpp, name=Nada
> var Duration : Real


---  
 #  Paused : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Whether or not the node is currently paused.
> ``` lang=cpp, name=Nada
> var Paused : Boolean


---  
 #  Time : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> The current time in the node.
> ``` lang=cpp, name=Nada
> var Time : Real


---  
 #  TimeScale : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> A scalar to dt when updating the node.
> ``` lang=cpp, name=Nada
> var TimeScale : Real


---  
 #  Methods


---  
 #  Clone : [animationnode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/animationnode.md)

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
 #  GetNormalizedTime : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function GetNormalizedTime() : Real
> ``` 


---  
 #  IsActive : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

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
> |tabs|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function PrintNode(tabs : Integer)
> ``` 


---  
 #  SetNormalizedTime : Void

> A value between [0-1].
> |Name|Type|Description|
> |---|---|---|
> |normalizedTime|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function SetNormalizedTime(normalizedTime : Real)
> ``` 


---  
 

 
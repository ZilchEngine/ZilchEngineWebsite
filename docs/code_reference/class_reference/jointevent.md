 `Event` `Physics`



(NOTE) Sent out when a joint reaches some condition. Currently sent out when a limit is reached or an impulse's limit is exceeded.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ Joint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointevent.md#joint-zilch-engine-docume)|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
| |[ JointCog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointevent.md#jointcog-zilch-engine-doc)| | |
| |[ ObjectA](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointevent.md#objecta-zilch-engine-docu)| | |
| |[ ObjectB](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/jointevent.md#objectb-zilch-engine-docu)| | |


 #  Properties


---  
 #  Joint : [joint](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/joint.md)

 `read-only`

> The Joint that triggered the event.
> ``` lang=cpp, name=Nada
> var Joint : Joint


---  
 #  JointCog : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

 `read-only`

> The Cog of the Joint that signaled the event.
> ``` lang=cpp, name=Nada
> var JointCog : Cog


---  
 #  ObjectA : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

 `read-only`

> ObjectA on the Joint.
> ``` lang=cpp, name=Nada
> var ObjectA : Cog


---  
 #  ObjectB : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

 `read-only`

> ObjectB on the Joint.
> ``` lang=cpp, name=Nada
> var ObjectB : Cog


---  
 #  Methods


---  
 

 
 `Event` `Physics`



(NOTE) Sent out when a joint reaches some condition. Currently sent out when a limit is reached or an impulse's limit is exceeded.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[Joint](jointevent.md#joint-zilch-engine-docume)|[event](event.md)| |
| |[JointCog](jointevent.md#jointcog-zilch-engine-doc)| | |
| |[ObjectA](jointevent.md#objecta-zilch-engine-docu)| | |
| |[ObjectB](jointevent.md#objectb-zilch-engine-docu)| | |


 #  Properties


---  
 #  Joint : [joint](joint.md)

 `read-only`

> The Joint that triggered the event.
> ```TS:Nada
> var Joint : Joint


---  
 #  JointCog : [cog](cog.md)

 `read-only`

> The Cog of the Joint that signaled the event.
> ```TS:Nada
> var JointCog : Cog


---  
 #  ObjectA : [cog](cog.md)

 `read-only`

> ObjectA on the Joint.
> ```TS:Nada
> var ObjectA : Cog


---  
 #  ObjectB : [cog](cog.md)

 `read-only`

> ObjectB on the Joint.
> ```TS:Nada
> var ObjectB : Cog


---  
 #  Methods


---  
 

 
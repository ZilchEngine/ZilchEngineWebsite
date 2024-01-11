 `Component` `Engine`



(NOTE) Forms a link between two positions on two objects. ObjectLinks are used primarily by physics to represent joints, but can also be used by graphics, gameplay, etc... to represent some connection between two objects.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](objectlink.md#objectlink-void)|[ LocalPointA](objectlink.md#localpointa-zilch-engine)|[component](component.md)| |
| |[ LocalPointB](objectlink.md#localpointb-zilch-engine)| | |
| |[ ObjectA](objectlink.md#objecta-zilch-engine-docu)| | |
| |[ ObjectAPath](objectlink.md#objectapath-zilch-engine)| | |
| |[ ObjectB](objectlink.md#objectb-zilch-engine-docu)| | |
| |[ ObjectBPath](objectlink.md#objectbpath-zilch-engine)| | |
| |[ WorldPointA](objectlink.md#worldpointa-zilch-engine)| | |
| |[ WorldPointB](objectlink.md#worldpointb-zilch-engine)| | |


 #  Properties


---  
 #  LocalPointA : [real3](../nada_base_types/real3.md)

> The Point on Object A in local space.
> ```TS:Nada
> var LocalPointA : Real3


---  
 #  LocalPointB : [real3](../nada_base_types/real3.md)

> The Point on Object B in local space.
> ```TS:Nada
> var LocalPointB : Real3


---  
 #  ObjectA : [cog](cog.md)

> The first object that is being connected to. Set this to null to clear the link.
> ```TS:Nada
> var ObjectA : Cog


---  
 #  ObjectAPath : [cogpath](cogpath.md)

> CogPath to object A.
> ```TS:Nada
> var ObjectAPath : CogPath


---  
 #  ObjectB : [cog](cog.md)

> The second object that is being connected to. Set this to null to clear the link.
> ```TS:Nada
> var ObjectB : Cog


---  
 #  ObjectBPath : [cogpath](cogpath.md)

> CogPath to object B.
> ```TS:Nada
> var ObjectBPath : CogPath


---  
 #  WorldPointA : [real3](../nada_base_types/real3.md)

> The point on object A in world space.
> ```TS:Nada
> var WorldPointA : Real3


---  
 #  WorldPointB : [real3](../nada_base_types/real3.md)

> The point on object B in world space.
> ```TS:Nada
> var WorldPointB : Real3


---  
 #  Methods


---  
 #  ObjectLink : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ObjectLink()
> ``` 


---  
 

 
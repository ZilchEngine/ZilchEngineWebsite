 `Component` `Engine`



(NOTE) Forms a link between two positions on two objects. ObjectLinks are used primarily by physics to represent joints, but can also be used by graphics, gameplay, etc... to represent some connection between two objects.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objectlink.md#objectlink-void)|[ LocalPointA](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objectlink.md#localpointa-zilch-engine)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)| |
| |[ LocalPointB](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objectlink.md#localpointb-zilch-engine)| | |
| |[ ObjectA](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objectlink.md#objecta-zilch-engine-docu)| | |
| |[ ObjectAPath](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objectlink.md#objectapath-zilch-engine)| | |
| |[ ObjectB](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objectlink.md#objectb-zilch-engine-docu)| | |
| |[ ObjectBPath](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objectlink.md#objectbpath-zilch-engine)| | |
| |[ WorldPointA](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objectlink.md#worldpointa-zilch-engine)| | |
| |[ WorldPointB](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/objectlink.md#worldpointb-zilch-engine)| | |


 #  Properties


---  
 #  LocalPointA : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The Point on Object A in local space.
> ``` lang=cpp, name=Nada
> var LocalPointA : Real3


---  
 #  LocalPointB : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The Point on Object B in local space.
> ``` lang=cpp, name=Nada
> var LocalPointB : Real3


---  
 #  ObjectA : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> The first object that is being connected to. Set this to null to clear the link.
> ``` lang=cpp, name=Nada
> var ObjectA : Cog


---  
 #  ObjectAPath : [cogpath](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cogpath.md)

> CogPath to object A.
> ``` lang=cpp, name=Nada
> var ObjectAPath : CogPath


---  
 #  ObjectB : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

> The second object that is being connected to. Set this to null to clear the link.
> ``` lang=cpp, name=Nada
> var ObjectB : Cog


---  
 #  ObjectBPath : [cogpath](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cogpath.md)

> CogPath to object B.
> ``` lang=cpp, name=Nada
> var ObjectBPath : CogPath


---  
 #  WorldPointA : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The point on object A in world space.
> ``` lang=cpp, name=Nada
> var WorldPointA : Real3


---  
 #  WorldPointB : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> The point on object B in world space.
> ``` lang=cpp, name=Nada
> var WorldPointB : Real3


---  
 #  Methods


---  
 #  ObjectLink : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ObjectLink()
> ``` 


---  
 

 
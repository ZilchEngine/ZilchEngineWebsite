 `Component` `Engine`



(NOTE) Component used to keep track of what ObjectLinks a cog has. This component is added dynamically whenever a ObjectLink is added to a cog that did not contain an ObjectLink before. This can be used to traverse across linked objects and find the entire "island" of ObjectLinks.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](objectlinkanchor.md#objectlinkanchor-void)|[ ObjectLinks](objectlinkanchor.md#objectlinks-zilch-engine)|[component](component.md)| |


 #  Properties


---  
 #  ObjectLinks : [objectlinkrange](objectlinkrange.md)

 `read-only`

> The range of object link edges connected to this anchor.
> ``` lang=cpp, name=Nada
> var ObjectLinks : ObjectLinkRange


---  
 #  Methods


---  
 #  ObjectLinkAnchor : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ObjectLinkAnchor()
> ``` 


---  
 

 
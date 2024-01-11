 `Resource` `Physics`



(NOTE) A convex mesh meant for use with dynamic rigid bodies. Computes efficient contact information compared to a regular physics mesh. This mesh also defines a volume which means mass properties can be computed.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](convexmesh.md#convexmesh-void)| |[genericphysicsmesh](genericphysicsmesh.md)| |
|[ CreateRuntime](convexmesh.md#createruntime-zilch-engin)| | | |
|[ RuntimeClone](convexmesh.md#runtimeclone-zilch-engine)| | | |


 #  Properties


---  
 #  Methods


---  
 #  ConvexMesh : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ConvexMesh()
> ``` 


---  
 #  CreateRuntime : [convexmesh](convexmesh.md)

 `static`

> Creates a ConvexMesh for run-time modifications.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function CreateRuntime() : ConvexMesh
> ``` 


---  
 #  RuntimeClone : [convexmesh](convexmesh.md)

> Creates a clone of this mesh for run-time modifications.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function RuntimeClone() : ConvexMesh
> ``` 


---  
 

 
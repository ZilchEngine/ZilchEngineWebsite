 `Editor`

(NOTE) Structure bound to the property view for the main editor. Contains the different settings that the user can modify.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AutoCompute](multiconvexmeshpropertyviewinfo.md#autocompute-void)|[ AutoComputeMethod](multiconvexmeshpropertyviewinfo.md#autocomputemethod-zilch-e)|[eventobject](eventobject.md)| |
|[ Constructor](multiconvexmeshpropertyviewinfo.md#multiconvexmeshpropertyv)|[ AutoComputeMode](multiconvexmeshpropertyviewinfo.md#autocomputemode-zilch-eng)| | |
| |[ ClearColor](multiconvexmeshpropertyviewinfo.md#clearcolor-zilch-engine-d)| | |
| |[ DrawMode](multiconvexmeshpropertyviewinfo.md#drawmode-zilch-engine-doc)| | |
| |[ MeshThickness](multiconvexmeshpropertyviewinfo.md#meshthickness-zilch-engin)| | |
| |[ OuterContourColor](multiconvexmeshpropertyviewinfo.md#outercontourcolor-zilch-e)| | |
| |[ SimplificationThreshold](multiconvexmeshpropertyviewinfo.md#simplificationthreshold)| | |
| |[ SpriteSource](multiconvexmeshpropertyviewinfo.md#spritesource-zilch-engine)| | |
| |[ SurfaceLevelThreshold](multiconvexmeshpropertyviewinfo.md#surfacelevelthreshold-ze)| | |


 #  Properties


---  
 #  AutoComputeMethod : [MultiConvexMeshAutoComputeMethod](../enum_reference.md#multiconvexmeshautocomputemethod)

> What method of auto-computing should be used? Most likely 'pixel' is the mode that should be used.
> ```TS:Nada
> var AutoComputeMethod : MultiConvexMeshAutoComputeMethod


---  
 #  AutoComputeMode : [MultiConvexMeshAutoComputeMode](../enum_reference.md#multiconvexmeshautocomputemode)

> Should the auto-computed mesh be calculated from the alpha or the intensity of the sprite?
> ```TS:Nada
> var AutoComputeMode : MultiConvexMeshAutoComputeMode


---  
 #  ClearColor : [real4](../nada_base_types/real4.md)

> The clear color of the viewport used to render.
> ```TS:Nada
> var ClearColor : Real4


---  
 #  DrawMode : [MultiConvexMeshDrawMode](../enum_reference.md#multiconvexmeshdrawmode)

> How should the collection of meshes be drawn?
> ```TS:Nada
> var DrawMode : MultiConvexMeshDrawMode


---  
 #  MeshThickness : [real](../nada_base_types/real.md)

> Since the mesh is on a 2d plane, they need some thickness for their z-depth. This controls how thick the meshes are.
> ```TS:Nada
> var MeshThickness : Real


---  
 #  OuterContourColor : [real4](../nada_base_types/real4.md)

> The color to draw edges with.
> ```TS:Nada
> var OuterContourColor : Real4


---  
 #  SimplificationThreshold : [real](../nada_base_types/real.md)

> A threshold to control when vertices should be removed (simplified). This value is related to the area of a triangle.
> ```TS:Nada
> var SimplificationThreshold : Real


---  
 #  SpriteSource : [spritesource](spritesource.md)

> The sprite source used as a reference for drawing the mesh. Note: this is not always what's visible as the user can drag in archetypes to view as well.
> ```TS:Nada
> var SpriteSource : SpriteSource


---  
 #  SurfaceLevelThreshold : [real](../nada_base_types/real.md)

> When the sprite is sampled using the AutoComputeMode, what value should be used to determine where a surface is.
> ```TS:Nada
> var SurfaceLevelThreshold : Real


---  
 #  Methods


---  
 #  AutoCompute : Void

> Resets the points of the mesh to an approximation for the current sprite.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function AutoCompute()
> ``` 


---  
 #  MultiConvexMeshPropertyViewInfo : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function MultiConvexMeshPropertyViewInfo()
> ``` 


---  
 

 
 `Editor`

(NOTE) Structure bound to the property view for the main editor. Contains the different settings that the user can modify.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AutoCompute](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/multiconvexmeshpropertyviewinfo.md#autocompute-void)|[ AutoComputeMethod](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/multiconvexmeshpropertyviewinfo.md#autocomputemethod-zilch-e)|[eventobject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/eventobject.md)| |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/multiconvexmeshpropertyviewinfo.md#multiconvexmeshpropertyv)|[ AutoComputeMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/multiconvexmeshpropertyviewinfo.md#autocomputemode-zilch-eng)| | |
| |[ ClearColor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/multiconvexmeshpropertyviewinfo.md#clearcolor-zilch-engine-d)| | |
| |[ DrawMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/multiconvexmeshpropertyviewinfo.md#drawmode-zilch-engine-doc)| | |
| |[ MeshThickness](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/multiconvexmeshpropertyviewinfo.md#meshthickness-zilch-engin)| | |
| |[ OuterContourColor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/multiconvexmeshpropertyviewinfo.md#outercontourcolor-zilch-e)| | |
| |[ SimplificationThreshold](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/multiconvexmeshpropertyviewinfo.md#simplificationthreshold)| | |
| |[ SpriteSource](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/multiconvexmeshpropertyviewinfo.md#spritesource-zilch-engine)| | |
| |[ SurfaceLevelThreshold](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/multiconvexmeshpropertyviewinfo.md#surfacelevelthreshold-ze)| | |


 #  Properties


---  
 #  AutoComputeMethod : [MultiConvexMeshAutoComputeMethod](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#multiconvexmeshautocomputemethod)

> What method of auto-computing should be used? Most likely 'pixel' is the mode that should be used.
> ``` lang=cpp, name=Nada
> var AutoComputeMethod : MultiConvexMeshAutoComputeMethod


---  
 #  AutoComputeMode : [MultiConvexMeshAutoComputeMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#multiconvexmeshautocomputemode)

> Should the auto-computed mesh be calculated from the alpha or the intensity of the sprite?
> ``` lang=cpp, name=Nada
> var AutoComputeMode : MultiConvexMeshAutoComputeMode


---  
 #  ClearColor : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

> The clear color of the viewport used to render.
> ``` lang=cpp, name=Nada
> var ClearColor : Real4


---  
 #  DrawMode : [MultiConvexMeshDrawMode](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#multiconvexmeshdrawmode)

> How should the collection of meshes be drawn?
> ``` lang=cpp, name=Nada
> var DrawMode : MultiConvexMeshDrawMode


---  
 #  MeshThickness : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Since the mesh is on a 2d plane, they need some thickness for their z-depth. This controls how thick the meshes are.
> ``` lang=cpp, name=Nada
> var MeshThickness : Real


---  
 #  OuterContourColor : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

> The color to draw edges with.
> ``` lang=cpp, name=Nada
> var OuterContourColor : Real4


---  
 #  SimplificationThreshold : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> A threshold to control when vertices should be removed (simplified). This value is related to the area of a triangle.
> ``` lang=cpp, name=Nada
> var SimplificationThreshold : Real


---  
 #  SpriteSource : [spritesource](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spritesource.md)

> The sprite source used as a reference for drawing the mesh. Note: this is not always what's visible as the user can drag in archetypes to view as well.
> ``` lang=cpp, name=Nada
> var SpriteSource : SpriteSource


---  
 #  SurfaceLevelThreshold : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> When the sprite is sampled using the AutoComputeMode, what value should be used to determine where a surface is.
> ``` lang=cpp, name=Nada
> var SurfaceLevelThreshold : Real


---  
 #  Methods


---  
 #  AutoCompute : Void

> Resets the points of the mesh to an approximation for the current sprite.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function AutoCompute()
> ``` 


---  
 #  MultiConvexMeshPropertyViewInfo : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function MultiConvexMeshPropertyViewInfo()
> ``` 


---  
 

 
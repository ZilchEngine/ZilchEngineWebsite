 `Component` `Graphics`



(NOTE) Base interface for components that require rendering.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ GroupSortValue](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/graphical.md#groupsortvalue-zilch-engi)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)|[basesprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/basesprite.md)|
| |[ LocalAabbCenter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/graphical.md#localaabbcenter-zilch-eng)| |[debuggraphical](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/debuggraphical.md)|
| |[ LocalAabbHalfExtents](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/graphical.md#localaabbhalfextents-zer)| |[heightmapmodel](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/heightmapmodel.md)|
| |[ Material](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/graphical.md#material-zilch-engine-doc)| |[model](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/model.md)|
| |[ OverrideBoundingBox](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/graphical.md#overrideboundingbox-zero)| |[particlesystem](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/particlesystem.md)|
| |[ ShaderInputs](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/graphical.md#shaderinputs-zilch-engine)| |[skinnedmodel](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/skinnedmodel.md)|
| |[ ViewCulling](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/graphical.md#viewculling-zilch-engine)| | |
| |[ VisibilityEvents](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/graphical.md#visibilityevents-zilch-en)| | |
| |[ Visible](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/graphical.md#visible-zilch-engine-docu)| | |
| |[ WorldAabb](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/graphical.md#worldaabb-zilch-engine-do)| | |


 #  Properties


---  
 #  GroupSortValue : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> Can be used by a RenderGroup to define draw order, from lowest to highest.
> ``` lang=cpp, name=Nada
> var GroupSortValue : Integer


---  
 #  LocalAabbCenter : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Center of the bounding box defined in local space, world transform will be applied.
> ``` lang=cpp, name=Nada
> var LocalAabbCenter : Real3


---  
 #  LocalAabbHalfExtents : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Half extents of the bounding box defined in local space, world transform will be applied.
> ``` lang=cpp, name=Nada
> var LocalAabbHalfExtents : Real3


---  
 #  Material : [material](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/material.md)

> The composition of shader fragments that determines how the graphical is rendered.
> ``` lang=cpp, name=Nada
> var Material : Material


---  
 #  OverrideBoundingBox : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Manually set the bounding box that is used for frustum culling.
> ``` lang=cpp, name=Nada
> var OverrideBoundingBox : Boolean


---  
 #  ShaderInputs : [shaderinputs](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/shaderinputs.md)

> List of shader inputs to be manually overridden only on this object.
> ``` lang=cpp, name=Nada
> var ShaderInputs : ShaderInputs


---  
 #  ViewCulling : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> If the graphical should not be drawn when its bounding volume is outside of the view frustum.
> ``` lang=cpp, name=Nada
> var ViewCulling : Boolean


---  
 #  VisibilityEvents : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> If object receives events when entering/exiting the view of an active camera.
> ``` lang=cpp, name=Nada
> var VisibilityEvents : Boolean


---  
 #  Visible : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> If the graphical should be drawn.
> ``` lang=cpp, name=Nada
> var Visible : Boolean


---  
 #  WorldAabb : [aabb](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md)

 `read-only`

> The world space axis aligned bounding volume that is used for frustum culling.
> ``` lang=cpp, name=Nada
> var WorldAabb : Aabb


---  
 #  Methods


---  
 

 
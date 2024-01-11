 `Component` `Graphics`



(NOTE) Base interface for components that require rendering.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ GroupSortValue](graphical.md#groupsortvalue-zilch-engi)|[component](component.md)|[basesprite](basesprite.md)|
| |[ LocalAabbCenter](graphical.md#localaabbcenter-zilch-eng)| |[debuggraphical](debuggraphical.md)|
| |[ LocalAabbHalfExtents](graphical.md#localaabbhalfextents-zer)| |[heightmapmodel](heightmapmodel.md)|
| |[ Material](graphical.md#material-zilch-engine-doc)| |[model](model.md)|
| |[ OverrideBoundingBox](graphical.md#overrideboundingbox-zero)| |[particlesystem](particlesystem.md)|
| |[ ShaderInputs](graphical.md#shaderinputs-zilch-engine)| |[skinnedmodel](skinnedmodel.md)|
| |[ ViewCulling](graphical.md#viewculling-zilch-engine)| | |
| |[ VisibilityEvents](graphical.md#visibilityevents-zilch-en)| | |
| |[ Visible](graphical.md#visible-zilch-engine-docu)| | |
| |[ WorldAabb](graphical.md#worldaabb-zilch-engine-do)| | |


 #  Properties


---  
 #  GroupSortValue : [integer](../nada_base_types/integer.md)

> Can be used by a RenderGroup to define draw order, from lowest to highest.
> ``` lang=cpp, name=Nada
> var GroupSortValue : Integer


---  
 #  LocalAabbCenter : [real3](../nada_base_types/real3.md)

> Center of the bounding box defined in local space, world transform will be applied.
> ``` lang=cpp, name=Nada
> var LocalAabbCenter : Real3


---  
 #  LocalAabbHalfExtents : [real3](../nada_base_types/real3.md)

> Half extents of the bounding box defined in local space, world transform will be applied.
> ``` lang=cpp, name=Nada
> var LocalAabbHalfExtents : Real3


---  
 #  Material : [material](material.md)

> The composition of shader fragments that determines how the graphical is rendered.
> ``` lang=cpp, name=Nada
> var Material : Material


---  
 #  OverrideBoundingBox : [boolean](../nada_base_types/boolean.md)

> Manually set the bounding box that is used for frustum culling.
> ``` lang=cpp, name=Nada
> var OverrideBoundingBox : Boolean


---  
 #  ShaderInputs : [shaderinputs](shaderinputs.md)

> List of shader inputs to be manually overridden only on this object.
> ``` lang=cpp, name=Nada
> var ShaderInputs : ShaderInputs


---  
 #  ViewCulling : [boolean](../nada_base_types/boolean.md)

> If the graphical should not be drawn when its bounding volume is outside of the view frustum.
> ``` lang=cpp, name=Nada
> var ViewCulling : Boolean


---  
 #  VisibilityEvents : [boolean](../nada_base_types/boolean.md)

> If object receives events when entering/exiting the view of an active camera.
> ``` lang=cpp, name=Nada
> var VisibilityEvents : Boolean


---  
 #  Visible : [boolean](../nada_base_types/boolean.md)

> If the graphical should be drawn.
> ``` lang=cpp, name=Nada
> var Visible : Boolean


---  
 #  WorldAabb : [aabb](aabb.md)

 `read-only`

> The world space axis aligned bounding volume that is used for frustum culling.
> ``` lang=cpp, name=Nada
> var WorldAabb : Aabb


---  
 #  Methods


---  
 

 
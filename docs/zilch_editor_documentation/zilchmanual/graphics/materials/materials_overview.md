[Materials](../../../../code_reference/class_reference/material.md), and the parameters found in them, define the shader for drawing objects for any purpose, using any renderer. Their overarching, generalized purpose is to house shader code (pixel, vertex, and geometry) using individual NadaFragments. These NadaFragments added to a Material as MaterialBlocks. These [shader fragments](shaders.md) define how the surface of the object on which it is placed will react to its environment.  [PBR](../physically_based_rendering.md), which is provided for the user as the default [DeferredRenderer](../renderer/deferred_renderer.md#deferred-renderer), is just one instance of how Materials may be used to render objects. To add a new Material, see [Adding a Resource](../../editor/editorcommands/resourceadding.md).

 # Material Templates

When creating a new material, there are six templates from which to choose:

|Template | Description
|--|--
|`ZilchMaterial`| PBR-based material defined by TextureMaps
|`OpaqueFlat`| PBR-based material defined by uniform values
|`EmptyMaterial`| Free of any default MaterialBlocks or references to [RenderGroups](../rendergroups.md)
|`AdditiveSprite`| Used for sprites that require additive blending
|`AlphaCut`| Used for graphicals that should be alpha cut
|`AlphaSprite`| Used for sprites that require alpha blending

Each of these templates has MaterialBlocks and references to RenderGroups pre-added. The ZilchMaterial, for example, has `AlbedoMap`, `NormalMap`, `RoughnessMap`, `MetallicMap`, and `SpecularValue` MaterialBlocks and references `Opaque`, and `ShadowCasters` RenderGroups.

[Albedo](albedo.md), [Normal](normal_map.md), [Metallic](metallic.md), [Roughness](roughness.md), and Specular are the parameters that define how light interacts with the material. Each of these parameters may be defined by a texture map or by a value, with the exception of the Normal parameter which may only be defined by a map.

---

 # Related Materials
 ## Manual
- [rendergroups](../rendergroups.md)
- [model_component](../models/model_component.md)
- [materials](../materials.md)
- [Albedo](albedo.md)
- [Normal](normal_map.md)
- [Metallic](metallic.md)
- [Roughness](roughness.md)
- [shaders](shaders.md)

 ## Code Reference
- [rendergroup](../../../../code_reference/class_reference/rendergroup.md) 
- [model](../../../../code_reference/class_reference/model.md)
- [material](../../../../code_reference/class_reference/material.md) 

 
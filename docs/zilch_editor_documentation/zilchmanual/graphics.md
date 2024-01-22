
 # [PBR Overview](graphics/physically_based_rendering.md)
The #zilch_engine uses physically based rendering techniques (PBR). The PBR overview offers a high level PBR description and resources for learning more about the details of PBR and its implementation in the #zilch_engine.

Components tracked by the graphics engine to represent visual objects, each with different benefits for their intended usage.

 ## [graphical](graphics/graphical.md)

 ## [Models](graphics/models.md)
General way of rendering meshes, such as characters or environment.

 ## [Sprites & Text](graphics/sprites.md)
Efficient rendering for a large amount of 2D art, frame-based animations, UI, and text display.

 ## [Particles](graphics/particles.md)
Creation and animation for a large amount of 2D images for visual effects, without the overhead of each particle being an independent game object.

 # Scene Setup
How to add graphical assets and configure a scene to look the way you want.

 ## [Adding Assets](graphics/adding_assets.md)
Importing textures, meshes, and animations and configuring how these resources are built.

 ## [Materials](graphics/materials.md)
Describe the surface attributes of an object or, more generally, define a shader program for any Graphical.

 ## [RenderGroups](graphics/rendergroups.md)
Categories for Materials that Renderers use to specify a group of objects to be rendered.

 ## [Cameras and CameraViewports](graphics/camerasviewportsrenderers.md)
Control how and from what perspective all rendering is done.

 ## [Lighting](graphics/lighting.md)
Adding and configuring lighting in a scene for the default Renderers provided in Zilch.

 ## [Renderer](graphics/renderer.md)
Nada script components that define the entire rendering pipeline of a scene.
 

 
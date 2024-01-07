  Welcome to ZilchHub, the open source project development hub for the Zilch Engine community. The Zilch Engine is a powerful simulation engine custom built in C++ by [DigiPen](https://www.digipen.edu/) [Research & Development](http://www.digipenresearch.com/), a team of DigiPen graduates.

 #  [Download the Engine](https://downloadlauncher.zeroengine.io )
 - [min_specs.md](https://github.com/ZilchEngine/ZilchDocs/blob/master//Users/beepboopowner/Desktop/AJ/DP/getting_started/min_specs.md)

 # Installing the Zilch Engine (and Zilch Launcher)

Zilch Engine is downloaded through a separate application called the Zilch Launcher, which provides features such as multiple build installation and access, new project creation, and a browser for recent projects.

 - [Learn how to use the Zilch Launcher](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/launcher.md).

 # Zilch Engine Features
The Zilch Engine can be used to make simulations of any kind. Projects range from simple prototypes to professional 2D and 3D games, simple physics or graphics demonstrations to robust, realistic simulations. Versatility of the engine is made possible by the features in the following sections:

 ## [Editor](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor.md)
 - A discrete [launcher](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/launcher.md) that provides access to all project and engine builds
 - [Editor modes](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editmode.md) customized for 2D and 3D projects
 - Full-featured [text editor](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/texteditor.md) with dozens of hotkeys and configuration options 

 ## [Architecture](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/architecture.md)
 - [Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/architecture/components.md)-based architecture applied across the engine in the form of :
  - NadaComponents for game object behaviors 
  - NadaFragment for fragment, vertex, and geometry shaders
  - ContentComponents for [Resources](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/architecture/resources.md) meta data 

 ## [Graphics](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/graphics.md)
 - Fully modifiable, scripted rendering pipeline
  - With a [physically-based renderer](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/graphics/physically_based_rendering.md) provided as the default renderer
 - Dedicated render thread

 ## [Physics](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics.md)
 - Custom-built, three-dimensional, constraint-based physics engine
 - Regions that can apply both pre-defined and user-defined [PhysicsEffects](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/physicseffectsandregions.md)
 - Robust, customizable [joint system](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/joints.md)

 ## [Audio](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio.md)
 - Scripted, [node-based](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundnode.md) DST system
 - 3D sound [positioning](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundemitter.md) and [attenuation](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio/soundattenuator.md)

 ## [Nada](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/nada_in_zero.md)
 - High-level scripting and shader language


 # Learning the Zilch Engine
Not all users have the same level of experience, with Zilch Engine or game engines in general. The following guidelines and recommendations provide recommendations for any level of user with different types of background and experience to become productive in Zilch.

 ## Novice Users
So you have never made a game or even programmed before. No problem! We have a sequence of [ tutorials ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/tutorials.md) and [ manual ](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual.md) pages that will instruct you in the basics of both Zilch and game programming in general. We suggest users of this level take the following steps to get started.

 ### New To Everything
 - The [standard tutorial sequence](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/tutorials/tutorial_sequences.md) will get you up and interacting with the Editor in the shortest amount of time possible. It is an excellent place to start if you want to dive right in.
 - The ZilchManual contains a wealth of information If you find yourself curious about about a certain [major engine system](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual.md), [imported or generated resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/architecture/resources.md), or concept, such as  [components](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/architecture/components.md), [Events](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/scripting/eventsandconnections.md), or [archetypes](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/architecture/archetypes.md).

 ### Some Prior Game Engine Experience
 - If you have some experience with another game engine, you may wish to create a new project and start playing around. The best way to learn is to do and experiment.
 - If you find yourself stuck or curious about a part of the engine you're unfamiliar with, check out the [ZilchManual](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual.md) for detailed coverage of the major systems,  individual elements, and concepts unique to the Zilch Engine. 

Once you've mastered the basics taught in the Basics and Beginner  [tutorial_sequences](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/tutorials/tutorial_sequences.md) and feel comfortable with the Editor UI and essential features, continue down to Intermediate Users.

 ## Intermediate Users
If you have some experience making games and programming, you will be able to pick things up fairly quickly.

 - Start with the [nada_in_zero](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/nada_in_zero.md). You will probably want to jump into scripting pretty quickly.
 - Read the [zilchmanual](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual.md) starting with the [editor](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor.md), [architecture](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/architecture.md), and [gameplay](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/gameplay.md) sections.
 - Browse [physics](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics.md), [editor](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor.md) and [audio](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/audio.md) sections for topics that are applicable to your project.
 - Read the remaining [zilchmanual](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual.md) sections at your own pace.
 - If you are not fully confident in your ability to start operating in the engine, try out some [tutorials](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/tutorials.md).
 - Remember that you can always look things up in the [code_reference](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference.md)
 

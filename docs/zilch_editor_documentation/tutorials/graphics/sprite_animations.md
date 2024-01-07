This lesson covers how to import and use sprite sheets to create sprite animations

 # Learning Objectives
 - Importing sprite sheets
 - Defining each animation frame
 - Sprite animation parameters

 # Level Setup
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ New Project](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#newproject)
 - Create a new project using the {nav icon=clone, name=Empty 2D Project} template
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- In the `Properties Window`
 - Rename Sprite object to `Player`
 - Under [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Scale  to `[2, 2, 2]`
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Renderer object
 - Under `ForwardRenderer`
  - Set ClearColor  to `[R:125, G:255, B:125, A:1.00]`



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/106281.png)


 # Importing a Sprite Sheet

Sprite animations are created out of a sequence of images displayed in quick succession. To accomplish this we use a Sprite Sheet; a image file that contains the sequence of frames corresponding to one or more animations.

- Download the following Sprite Sheet:



![RedPandaSpriteSheet](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/106314.png)


- Import them into the project by dragging and dropping the files into the `Level Window`
- In the `Group Import Options Window`
 - Set ImportImages enum to `Sprites`
 - Press the `Import All` button



![ImportSpriteSheet](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/106316.gif)


 # Creating Sprite Animations

Now that we have imported a sprite sheet, we need to separate the frames into their respective animations. The sheet we just imported has two animations; a walk animation that corresponds to the top 5 frames and a roll animation that corresponds to the remaining 7 frames.



![RedPandaAnimationFrames](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/106388.png)


- In the `Library Window`
 - Under the SpriteSource  tag
  - `Double-Click` the RedPandaSpriteSheet texture resource
- In the `Sprite Source Editor Window`
 - Press the `Convert To Animation` button



![ConvertToAnimation](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/106407.png)


- In the `Sprite Importer Window`
 - Set FramesPerRow  to `5`
 - Set NumberOfRows  to `3`
 - Left-click  frames 0 through 4 to select them
 - If you accidentally select a tile you don't want, right-click  it to deselect it
 - Set Name  to `Walk`
 - Press the `Add and Continue` button
 - Left-click  frames 5 through 11 to select them
 - Set Name  to `Roll`
 - Press the `Add and Close` button

(NOTE) **Frame Size vs. Frame Count:** When you set FramesPerRow , the Sprite Importer automatically calculates the FrameWidth  property, and vice versa. Likewise, when you set NumberOfRows , FrameHeight  is computed automatically, and vice versa. As a result, if you would rather specify the pixel dimensions of each frame in a sprite sheet than the number of frames, that's a perfectly valid option too.



![CreatingAnimations](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/106325.gif)


 # Using Sprite Animations

Now that we've generated the animation resources, we can start using them with sprites.

- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Player object
- In the `Properties Window`
 - Under [Sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md)
 - Set SpriteSource enum to `Walk`

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![WalkAnimatio](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/106332.gif)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

Looking at the [Sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md) component on the property grid we find that the last 4 properties are dedicated to sprite animations. They are:

| Sprite Animation Properties |
|--------------------|-------------------------------------------------------------------------------------|
| AnimationActive checkBox | Whether the animation is playing currently (Both in editor and in game) |
| AnimationSpeed   | Scalar applied to the Frame Rate of the animation resource   |
| StartFrame           | What frame the animation should start from  |
| CurrentFrame      | The current active frame of the animation (cycles as the animation is playing) |

Let's add a component that lets us control the animation.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `PlayerAnimationController`
- In the `PlayerAnimationController` script
 - Update the `PlayerAnimationController` class to the following:

```lang=csharp, name="PlayerAnimationController"
class PlayerAnimationController : NadaComponent
{
  [Dependency] var Sprite : Sprite;
  
  [Property]
  var WalkAnimation : SpriteSource = SpriteSource.Walk;
  
  [Property]
  var RollAnimation : SpriteSource = SpriteSource.Roll;
  
  [Property]
  var RollKey : Keys = Keys.Space;
  
  function Initialize(init : CogInitializer)
  {
    Zilch.Connect(Zilch.Keyboard, Events.KeyDown, this.OnKeyDown);
    Zilch.Connect(this.Space, Events.LogicUpdate, this.OnLogicUpdate);
  }

  function OnKeyDown(event : KeyboardEvent)
  {
    if(event.Key == this.RollKey)
      this.Sprite.SpriteSource = this.RollAnimation;
  }

  function OnLogicUpdate(event : UpdateEvent)
  {
    //If we are playing the roll animation
    if(this.Sprite.SpriteSource == this.RollAnimation)
    {
      //And it reaches its last frame (counted from 0 to 6)
      if(this.Sprite.CurrentFrame == 6)
      {
        //Play the walk animation
        this.Sprite.SpriteSource = this.WalkAnimation;
      }
    }
  }
}
```
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Player object
- In the `Properties Window`
 - [ Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `PlayerAnimationController`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)

- Press `Space`



![WalkAndRoll](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/106395.gif)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

 # Related Materials

 ## Manual
- [Sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/graphics/sprites/sprite.md)
- [Sprite Source Editor](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/graphics/sprites/spritesourceeditor.md)
- [Sprite Importer](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/graphics/sprites/spriteimporter.md)

 ## Code Reference
 ### Classes
- [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
- [Sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md)
- [Cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)
- [spritesource](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spritesource.md)

 ### Commands
- [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
- [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)


 ## Development Task
- T1183
 

 
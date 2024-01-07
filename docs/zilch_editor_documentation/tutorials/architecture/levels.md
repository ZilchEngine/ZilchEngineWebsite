This lesson covers levels in the Zilch Engine.


 #  Learning Objectives


- Creating new levels
- Loading and reloading levels
- Setting the StartingLevel 


 #  Level Setup


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ New Project](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#newproject)
 - Create a new project using the {nav icon=clone, name=Empty 2D Project} template


 #  What is a Level?


A Level resource is a resource that stores a list of objects. These objects are created when the level is **loaded**.


 #  Creating a New Level


Levels are added to the project in basically the same way as any other resource: by [ adding a resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md) using one of the pre-defined resource templates.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/96086.png)


*Zilch's Level templates*


Zilch's built-in Level templates are like shortcuts for creating levels of different kinds: they've already got the important cogs, like renderers and cameras, and they're pre-configured to be suitable for the chosen type of level. The {nav icon=clone, name="2D Level"} template provides a **forward renderer** and an **orthographic camera**, perfect for a simple 2D game.

 - Create a Level resource using the {nav icon=clone, name="2D Level"} template and name it `Level1`
- [ Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Renderer object
- In the `Properties Window`
 - Under `ForwardRenderer`
  - Set ClearColor  to `[R:16, G:78, B:32, A:1.00]`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ CreateSpriteText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createspritetext)
- In the `Properties Window`
 - Rename SpriteText object to `LevelNameText`
 - Under [ Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Translation  to `[0, 5, 0]`
 - Under [ SpriteText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spritetext.md)
  - Set Text  to `- Level 1 -`
  - Set PixelsPerUnit  to `32`



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/96093.png)


*Level 1*


(NOTE) **A Closer Look:**
 Take a look at the `Objects Window`:
 ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/96099.png)
 This is the list of objects in this level. In a sense, this list *is* this level, since a level is basically a list of objects. These objects are stored in the Level resource resource, listed as they are here, each with its properties as set in the `Properties Window`. When the level is loaded, each of these objects is created and initialized.


 ##  Creating a Player


There's no sense in having a level if there's no player, eh?

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `KeyboardMovement`
- Update the `KeyboardMovement` script to the following:

```lang=csharp, name="KeyboardMovement"
class KeyboardMovement : NadaComponent
{
  [Dependency] var Transform : Transform;
  
  [Property]
  var UpKey    : Keys = Keys.Up;
  [Property]
  var DownKey  : Keys = Keys.Down;
  [Property]
  var RightKey : Keys = Keys.Right;
  [Property]
  var LeftKey  : Keys = Keys.Left;
  [Property]
  var Speed : Real = 8;
  [Property]
  var MinBounds : Real3 = Real3(-12, -8, 0.5);
  [Property]
  var MaxBounds : Real3 = Real3( 12,  8, 0.5);
  
  function Initialize(init : CogInitializer)
  {
    Zilch.Connect(this.Space, Events.LogicUpdate, this.OnLogicUpdate);
  }
  
  function OnLogicUpdate(event : UpdateEvent)
  {
    var movement = Real3.Zero;
    
    if (Zilch.Keyboard.KeyIsDown(this.UpKey))
      movement += Real3.YAxis;
    if (Zilch.Keyboard.KeyIsDown(this.DownKey))
      movement -= Real3.YAxis;
    if (Zilch.Keyboard.KeyIsDown(this.RightKey))
      movement += Real3.XAxis;
    if (Zilch.Keyboard.KeyIsDown(this.LeftKey))
      movement -= Real3.XAxis;
    
    var newPosition = this.Transform.LocalTranslation + movement * this.Speed * event.Dt;
    this.Transform.LocalTranslation = Math.Clamp(newPosition, this.MinBounds, this.MaxBounds);
  }
}
```

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- In the `Properties Window`
 - Rename Sprite object to `Player`
 - Under [ Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Translation  to `[0, 0, 0.5]`
 - Under [ Sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md)
  - Set VertexColor  to `[R:64, G:255, B:160, A:1.00]`
  - Set SpriteSource  to `CircleBordered`
 - [ Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `SphereCollider`
 - Under [ SphereCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spherecollider.md)
  - Set Ghost checkBox to `true`
 - [ Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `RigidBody`
 - Under [ RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
  - Set DynamicState enum to `Kinematic`
 - [ Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `KeyboardMovement`

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![Player movement in Level 1](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/96103.gif)


*Player moving around in Level 1*


You can move the player with the arrow keys.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

Now let's make a Level 2 to go to from Level 1.


 ##  Creating Another Level


- In the `Library Window`
 - Under the Level  tag
  - {nav icon=mouse-pointer, name="Right click"} the `Level1` Level resource
   - Select **Duplicate** to create a copy of `Level1`
  - Rename the `Level1Copy1` Level resource to `Level2`
  - Open the `Level2` Level resource

Level 2 should be visually distinct from Level 1.

- [ Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : LevelNameText object
- In the `Properties Window`
 - Under `SpriteText`
  - Set Text  to `- Level 2 -`
- [ Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Renderer object
- In the `Properties Window`
 - Under `ForwardRenderer`
  - Set ClearColor  to `[R:48, G:59, B:84, A:1.00]`



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/96096.png)


*Level 2*


Now let's make some way of going between Level 1 and Level 2.


 #  Loading a Level in the Game


Going from one level to another is as simple as calling the [ space](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md)'s LoadLevel function. Let's make a door: an object that calls that function when the player touches it.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `LoadLevelOnCollisionStarted`
- Update the `LoadLevelOnCollisionStarted` script to the following:

```lang=csharp, name="LoadLevelOnCollisionStarted"
class LoadLevelOnCollisionStarted : NadaComponent
{
  [Property]
  var LevelToLoad : Level;
  
  function Initialize(init : CogInitializer)
  {
    Zilch.Connect(this.Owner, Events.CollisionStarted, this.OnCollisionStarted);
  }
  
  function OnCollisionStarted(event : CollisionEvent)
  {
    // If the other object in this collision has a KeyboardMovement component,
    // then it must be the player
    if (event.OtherObject.KeyboardMovement != null)
      this.Space.LoadLevel(this.LevelToLoad);
  }
}
```

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- In the `Properties Window`
 - Rename Sprite object to `Door`
 - Under [ Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Translation  to `[-5, 3, 0]`
  - Set Scale  to `[2, 3, 1]`
 - Under [ Sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md)
  - Set VertexColor  to `[R:230, G:23, B:57, A:1.00]`
 - [ Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `BoxCollider`
 - Under [ BoxCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md)
  - Set Ghost checkBox to `true`
 - [ Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `LoadLevelOnCollisionStarted`
 - Under `LoadLevelOnCollisionStarted`
  - Set LevelToLoad resource to `Level1`



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/96108.png)


*Level 2 now has a door*


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Copy](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#copy) the Door object
- Open the Level resource named `Level1`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Paste](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#paste) the Door object
- In the `Properties Window`
 - Under [ Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Translation  to `[5, -4, 0]`
 - Under `LoadLevelOnCollisionStarted`
  - Set LevelToLoad resource to `Level2`



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/96106.png)


*Level 1 now has a door*


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![Level switching](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/96112.gif)


If you move the player to the door, the other level is loaded.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

(NOTE) **A Closer Look:**
 When the player touches the door in Level 1, Level 2 is loaded. So what happens to Level 1? When a space's LoadLevel function is called, first, all the objects in that space are destroyed: the player, the door, the camera, the renderer, all of them. Then, all the objects in Level 2 are created. This happens every time a space changes levels.


 #  Reloading a Level


Just as the space has a function to load a level, it also has a function to reload the current level.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `ReloadLevelOnKeyDown`
- Update the `ReloadLevelOnKeyDown` script to the following:

```lang=csharp, name="ReloadLevelOnKeyDown"
class ReloadLevelOnKeyDown : NadaComponent
{
  function Initialize(init : CogInitializer)
  {
    Zilch.Connect(Zilch.Keyboard, Events.KeyDown, this.OnKeyDown);
  }
  
  function OnKeyDown(event : KeyboardEvent)
  {
    if (event.Key == Keys.R && event.CtrlPressed)
      this.Space.ReloadLevel();
  }
}
```

Calling the ReloadLevel function does the same thing as calling the LoadLevel function and passing in the current level.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Select the Space](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#selectspace)
- In the `Properties Window`
 - [ Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `ReloadLevelOnKeyDown`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![Level reloading](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/96114.gif)


You can now reload the level by pressing key `Ctrl + R`.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

(NOTE)**A Closer Look:**
 Reloading a level is just the same as loading it again, so it goes through the same process. First, everything present is destroyed. Then, everything in the level is created anew. This means that all of its objects, and all of their components, are reinitialized. However, this does *not* destroy the space that contains the level, which is only initialized when it is created, and destroyed when the user explicitly destroys it in script (or when the game ends).


 #  Setting a Game's Starting Level


When a Zilch game is [ played in the editor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame), the default game setup loads the level that is currently being edited. When the game is exported, however, this isn't necessarily the first level to be loaded. As a matter of fact, there is a component on the GameSession aptly named [ DefaultGameSetup](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/defaultgamesetup.md), which manages this.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Select the Game](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#selectgame)
- In the `Properties Window`
 - Expand [ DefaultGameSetup](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/defaultgamesetup.md)



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/96116.png)


Here, we can see some useful properties: StartingSpace enum specifies the archetype to use for creating the game's default space. StartingLevel enum determines which level is loaded into that space after it's created. LoadEditingLevel checkBox tells the engine whether it should override the starting level when the game is being run in the editor, and instead load the level that's being edited.

Let's make a new level, a title screen, and set it as the starting level.


 ##  Creating a Title Screen


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a Level resource using the {nav icon=clone, name="2D Level"} template and name it `TitleScreen`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ CreateSpriteText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createspritetext)
- In the `Properties Window`
 - Under [ Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Translation  to `[0, 3, 0]`
 - Under [ SpriteText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spritetext.md)
  - Set Text  to `Azomarith's Revenge 2: Shadows of the Fallen`
  - Set PixelsPerUnit  to `32`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ CreateSpriteText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createspritetext)
- In the `Properties Window`
 - Under [ Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Translation  to `[0, 2, 0]`
 - Under [ SpriteText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spritetext.md)
  - Set Text  to `Game of the Year Edition`
  - Set FontSize  to `24`
  - Set PixelsPerUnit  to `32`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ CreateSpriteText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createspritetext)
- In the `Properties Window`
 - Under [ Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Translation  to `[0, -3, 0]`
 - Under [ SpriteText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spritetext.md)
  - Set Text  to `Press Enter`
  - Set FontSize  to `18`
  - Set PixelsPerUnit  to `32`



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/96118.png)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Select the Game](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#selectgame)
- In the `Properties Window`
 - Under [ DefaultGameSetup](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/defaultgamesetup.md)
  - Set StartingLevel enum to `TitleScreen`
  - Set LoadEditingLevel checkBox to `false`
- Open the Level resource named `Level1`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)

Even though we're editing Level 1, the editor loads the title screen, thanks to how the DefaultGameSetup has been configured.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

Next, we need a component to load Level 1 from the title screen.

- Open the Level resource named `TitleScreen`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `LoadLevelOnKeyDown`
- Update the `LoadLevelOnKeyDown` script to the following:

```lang=csharp, name="LoadLevelOnKeyDown"
class LoadLevelOnKeyDown : NadaComponent
{
  [Property]
  var LevelToLoad : Level = Level.Level1;
  [Property]
  var Key : Keys = Keys.Enter;
  
  function Initialize(init : CogInitializer)
  {
    Zilch.Connect(Zilch.Keyboard, Events.KeyDown, this.OnKeyDown);
  }
  
  function OnKeyDown(event : KeyboardEvent)
  {
    if (event.Key == this.Key)
      this.Space.LoadLevel(this.LevelToLoad);
  }
}
```

- [ Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : LevelSettings object
- In the `Properties Window`
 - [ Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `LoadLevelOnKeyDown`
- Open the Level resource named `Level1`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![Level sequence](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/96125.gif)


*The game starts with the title screen, then goes to Level 1*


Now the game always starts with the title screen, and from there goes into Level 1 via the `Enter` key.

 #  Related Materials
 ##  Manual
- [launchernewproject](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/launchernewproject.md)
- [commands](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md)
- [resourceadding](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
- [selectobject](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md)
- [addremovecomponent](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md)

 ##  Reference
 ###  Classes
- [transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
- [spritetext](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spritetext.md)
- [sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md)
- [spherecollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spherecollider.md)
- [boxcollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md)
- [rigidbody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
- [space](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/space.md)
- [defaultgamesetup](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/defaultgamesetup.md)

 ###  Commands
- [ CreateSpriteText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createspritetext)
- [ CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
- [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)
- [ Paste](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#paste)
- [ SelectSpace](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#selectspace)
- [ SelectGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#selectgame)

 ##  Development Task
- {T1172} 

 
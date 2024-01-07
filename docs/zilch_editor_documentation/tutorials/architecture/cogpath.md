[CogPaths](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cogpath.md) provide the best way to get a reference to any [Cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md) before running the game. Often you will find situations where a component needs to be aware of a paticular object when the game starts. While CogPaths are not limited to only working at load time this is where they are most useful.


 #  Learning Objectives


- CogPath properties
- Accessing components on other objects


 #  Level Setup


First we will make the ground and player objects.
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ New Project](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#newproject)
 - Create a new project using the {nav icon=clone, name=Empty 2D Project} template
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : LevelSettings object
 - [Remove component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [gravityeffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gravityeffect.md)

- [Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [Add resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `PlayerController`
- Update `PlayerController` script to the following code block:

```name=PlayerController, lang=csharp
class PlayerController : NadaComponent
{
  [Property]
  var Speed : Real = 5.0;
  
  function Initialize(init : CogInitializer)
  {
    Zilch.Connect(this.Space, Events.LogicUpdate, this.OnLogicUpdate);
  }

  function OnLogicUpdate(event : UpdateEvent)
  {
    var direction = Real3();
    
    if(Zilch.Keyboard.KeyIsDown(Keys.Right))
      direction.X += 1.0;
    
    if(Zilch.Keyboard.KeyIsDown(Keys.Left))
      direction.X += -1.0;
    
    if(Zilch.Keyboard.KeyIsDown(Keys.Up))
      direction.Y += 1.0;
    
    if(Zilch.Keyboard.KeyIsDown(Keys.Down))
      direction.Y += -1.0;
    
    this.Owner.RigidBody.Velocity = direction * this.Speed;
  }
}
```
- [Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- In the `name=Properties Window, icon=window-restore`
 - Rename Sprite object to `Player`
 - [Add component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [rigidbody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
 - [Add component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [boxcollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md)
 - [Add component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `PlayerController`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
 - Press `Left`, `Right`, `Up` and `Down`



![simpleinput](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/90208.gif)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

 # The Follower

- [Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [Add resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `FollowerController`
- Update `FollowerController` script to the following code block:

```name=FollowerController, lang=csharp
class FollowerController : NadaComponent
{
  [Property]
  var PlayerCogPath : CogPath = CogPath();
  
  var Speed : Real = 5.0;
  
  function Initialize(init : CogInitializer)
  {
    Zilch.Connect(this.Space, Events.LogicUpdate, this.OnLogicUpdate);
  }

  function OnLogicUpdate(event : UpdateEvent)
  {
    var targetPos = this.PlayerCogPath.Cog.Transform.Translation;
    var myPos = this.Owner.Transform.Translation;
    var direction = Math.Normalize(targetPos - myPos);
    this.Owner.RigidBody.Velocity = direction * this.Speed;
  }
}
```

In the script above the position of the player and the position of the follower are used to calculate a unit vector which defines the 3D direction from the follower to the player. By multiplying it with `this.Speed` a velocity is defined which can be applyed to move the follower object.

(NOTE)**Initializing a CogPath Property**: Notice that a CogPath constructor was acutally called in the definition of the `PlayerCogPath` property. CogPath's are one of the few types that require a manual construction where as Nada value types can have their initial value infered: i.e. `var MemberVariable : Real;` in this case `MemberVariable` will have the default type value of `0`.

- [Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- In the `name=Properties Window, icon=window-restore`
 - Set `name=Name, icon=pencil-square-o` to: `Follower`
 - [Add component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [boxcollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md)
 - [Add component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `FollowerController`
 - Under [sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md)
   - Set `name=VertexColor, icon=eyedropped` to: `[0,0,1,1]`
 - Under [transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
   - Set `name=Translation, icon=pencil-square-o` to: `[-5,0,0]`

 ##  Setting a CogPath
 - Under `FollowController`

  ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/90210.png)

This is the CogPath Property GUI. To select which object the CogPath points add you simple click on the Crosshairs and drag them to the target object.



![SetCogPath](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/90218.gif)


  - Set `name=PlayerCogPath, icon=pencil-square-o` to reference the Player object

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
 - Press `Left`, `Right`, `Up` and `Down`



![Follower](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/90220.gif)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

 # CogPaths and Hierarchies

- [Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- In the `name=Properties Window, icon=window-restore`
 - Set `name=Name, icon=pencil-square-o` to: `Child`
 - Under [transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
   - Set `name=Translation, icon=pencil-square-o` to: `[2,0,0]`
   - Set `name=Scale, icon=pencil-square-o` to: `[0.5,0.5,0.5]`
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Child object
 - Drag and drop it on the Player object object

  ![ChildToPlayer](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/90222.gif)

- [Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- In the `name=Properties Window, icon=window-restore`
 - Set `name=Name, icon=pencil-square-o` to: `Parent`
 - Under [transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
   - Set `name=Translation, icon=pencil-square-o` to: `[0,2,0]`
   - Set `name=Scale, icon=pencil-square-o` to: `[0.5,0.5,0.5]`
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Player object
 - Drag and drop it on the Parent object object

  ![PlayerToParent](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/90364.gif)

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
 - Press `Left`, `Right`, `Up` and `Down`

 ![TestChildPlayer](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/90230.gif)

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

It can be seen that the Player object moves independently of its parent object do to it having its own RigidBody. However, you may be wondering why the follower no longer goes to the same position as the Player object. If you remember from [Hierarchies I](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/tutorials/architecture/hierarchies.md), Player object is now a child object meaning its `name=Translation, icon=pencil-square-o` is measured relative to it's paren object. Since the `FollowerController` was not changed to use the explicit `name=WorldTranslation, icon=pencil-square-o` of the Player object, the Follower object moves to the same offset of the Player object as it starts with its Parent object.

- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) the Follower object object
 - Under `FollowerController`
  - Examine the text of the `name=PlayerCogPath, icon=pencil-square-o` property

Notice that the CogPath text has not changed despite the fact that the player hierarchy order has changed.

  - Set `name=PlayerCogPath, icon=pencil-square-o` to reference the Player object

 ![ResetCogPath](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/90232.gif)

Notice that the text of `name=PlayerCogPath, icon=pencil-square-o` changes from `:/Player` to the correct path of `:/Parent/Player`. You may be wondering why it worked when the project was run last. When CogPath properties are set they capture a reference at that moment as opposed to waiting for the level to be loaded into the game. When the path to an object targeted by a CogPath changes it does not lose that direct reference to the object, but instead the Path becomes inaccurate. You should not depend on this behavior and you should always reset your CogPath properties to have the correct path when possible. If you wish to learn more about the complex behaviors of the direct cog reference visit the [CogPaths Manual Page](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/cogpathsmanual.md).


- In the `FollowerController` script update `OnLogicUpdate` to this code block

```name=FollowerController OnLogicUpdate, lang=csharp
function OnLogicUpdate(event : UpdateEvent)
{
  var targetPos = this.PlayerCogPath.Cog.Transform.WorldTranslation;
  var myPos = this.Owner.Transform.Translation;
  var direction = Math.Normalize(targetPos - myPos);
  this.Owner.RigidBody.Velocity = direction * this.Speed;
}
```

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)

 - Press `Left`, `Right`, `Up` and `Down`

 ![FollowWorldTrans](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/90366.gif)

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

Now the Follower object follows the Player object `name=WorldTranslation, icon=pencil-square-o` correctly.

 # Related Materials
 # Manual
- [CogPaths](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/cogpathsmanual.md)
- [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)

 # Tutorials
- [hierarchies](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/tutorials/architecture/hierarchies.md)

 # Reference
 ### Classes
- [CogPaths](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cogpath.md)
- [gravityeffect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/gravityeffect.md)
- [rigidbody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
- [boxcollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/boxcollider.md)
- [transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)

 ### Commands
- [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
- [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)
- [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)


 # Tasks
- T864
 

 
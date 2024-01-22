This lesson covers how to create archetypes from a script at game runtime.


 # Learning Objectives
 - Creating archetypes from a script
 - Modifing dynamically created objects

 # Level Setup
- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [New Project](../../../code_reference/command_reference.md#newproject)
 - Create a new project using the {nav icon=clone, name=Empty 2D Project} template
- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](../../../code_reference/command_reference.md#createsprite)
- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [Add Resource](../../zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `MovementLogic`
- In the `MovementLogic` script
 - Replace the script's contents with the following:

```TS:MovementLogic
class MovementLogic : NadaComponent
{
  var Speed : Real = 5.0;
  
  function Initialize(init : CogInitializer)
  {
    Zilch.Connect(this.Space, Events.LogicUpdate, this.OnLogicUpdate);
  }

  function OnLogicUpdate(event : UpdateEvent)
  {
    var dir : Real3 = Real3(0,0,0);
    
    if(Zilch.Keyboard.KeyIsDown(Keys.A))
    {
      dir -= Real3.XAxis;
    }
    
    if(Zilch.Keyboard.KeyIsDown(Keys.D))
    {
      dir += Real3.XAxis;
    }
    
    this.Owner.RigidBody.Velocity = dir * this.Speed;
  }
}
```

- [Select](../../zilchmanual/editor/editorcommands/selectobject.md) : LevelSettings object
- In the `Properties Window`
 - [Remove Component](../../zilchmanual/editor/addremovecomponent.md) : [GravityEffect](../../../code_reference/class_reference/gravityeffect.md)
 - [Remove Component](../../zilchmanual/editor/addremovecomponent.md) : [DragEffect](../../../code_reference/class_reference/drageffect.md)

- [Select](../../zilchmanual/editor/editorcommands/selectobject.md) : Sprite object 
- In the `Properties Window`
 - Rename Sprite object  to `Player`
 - [Add Component](../../zilchmanual/editor/addremovecomponent.md) : `MovementLogic`

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [Play the Game](../../zilchmanual/editor/editorcommands/runthegame.md)
 -  Press key `A` and `D`



![Movement](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/90547.gif)


- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [Stop Game](../../zilchmanual/editor/editorcommands/stopgame.md)

 # Archetype Creation

Before we can spawn objects from script, we need to create the archetype from which the instances (objects) will be created.

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](../../../code_reference/command_reference.md#createsprite)
- In the `Properties Window`
 - Rename it to `Bullet`
 - Under [Sprite](../../../code_reference/class_reference/sprite.md)
  - Set the SpriteSource texture to `Cricle`
  - Set the VertexColor  to `Red [R:255, G:0, B:0, A:1.00]`
 - Under [Transform](../../../code_reference/class_reference/transform.md)
  - Set Scale  to `[0.5, 0.5, 0.5]`
 - [Add Component](../../zilchmanual/editor/addremovecomponent.md) : [RigidBody](../../../code_reference/class_reference/rigidbody.md)
 - Set `name=Archetype, icon=pencil-square-o` to `BulletArchetype` and click the UploadToArchetype button button.



![BulletArchetype](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/90549.gif)


 - Delete the Bullet object

 # Spawning Archetypes

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [Add Resource](../../zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `ShootingLogic`
- In the `ShootingLogic`
 - Replace the script's contents with the following:

```TS:ShootingLogic
class ShootingLogic : NadaComponent
{
  
  var BulletSpeed : Real = 10.0;
  
  var ShotCooldown : Real = 0.4;
  
  var Timer : Real = 0.0;
  
  function Initialize(init : CogInitializer)
  {
    Zilch.Connect(this.Space, Events.LogicUpdate, this.OnLogicUpdate);
  }

  function OnLogicUpdate(event : UpdateEvent)
  {
    this.Timer += event.Dt;
    
    if(Zilch.Keyboard.KeyIsDown(Keys.Space) && this.Timer > this.ShotCooldown)
    {
      var bullet = this.Space.CreateAtPosition(Archetype.BulletArchetype, this.Owner.Transform.Translation);
      bullet.RigidBody.Velocity = Real3(0, this.BulletSpeed, 0);
      this.Timer = 0.0;
    }
  }
}
```

- [Select](../../zilchmanual/editor/editorcommands/selectobject.md) : Player object
- In the `Properties Window`
 - [Add Component](../../zilchmanual/editor/addremovecomponent.md) : `ShootingLogic` component
- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [Play the Game](../../zilchmanual/editor/editorcommands/runthegame.md)
 - Press key `A` and `D` keys to move
 - Press key `Space` key to shoot



![Shooting](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/90561.gif)


- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [Stop the Game](../../zilchmanual/editor/editorcommands/stopgame.md)

Let's take a closer look inside the `ShootingLogic`'s LogicUpdate function:

> `this.Timer += event.Dt;` 
> Increases our `Timer` variable by time elapsed since last frame.

> `if(Zilch.Keyboard.KeyIsDown(Keys.Space) && this.Timer > this.ShotCooldown)` 
> Checks whether `Space` is pressed and if `Timer` is greater than `ShotCooldown`

> `var bullet = this.Space.CreateAtPosition(Archetype.BulletArchetype, this.Owner.Transform.Translation);`
> Creates an Instance of the `BulletArchetype` at the owner's position and stores it in a local variable


> `bullet.RigidBody.Velocity = Real3(0, this.BulletSpeed, 0);`
> Uses the local variable to access the newly created object and sets its velecity

> `this.Timer = 0.0;`
> Resets the `Timer`


 # Related Materials

 ## Manual
- [COGs](../../zilchmanual/architecture/cogs/gameobjectsconcept.md)
- [Archetypes](../../zilchmanual/architecture/archetypes.md)
- [Play the Game](../../zilchmanual/editor/editorcommands/runthegame.md)
- [Stop the Game](../../zilchmanual/editor/editorcommands/stopgame.md)
- [Add Resource](../../zilchmanual/editor/editorcommands/resourceadding.md)

 ## Reference
 ### Classes
- [Transform](../../../code_reference/class_reference/transform.md)
- [Sprite](../../../code_reference/class_reference/sprite.md)
- [Cog](../../../code_reference/class_reference/cog.md)
- [Sprite](../../../code_reference/class_reference/sprite.md)
- [RigidBody](../../../code_reference/class_reference/rigidbody.md)
- [GravityEffect](../../../code_reference/class_reference/gravityeffect.md)
- [DragEffect](../../../code_reference/class_reference/drageffect.md)

 ### Commands
- [CreateSprite](../../../code_reference/command_reference.md#createsprite)

 ## Task
- T888 

 
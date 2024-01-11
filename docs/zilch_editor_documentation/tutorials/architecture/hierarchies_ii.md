This lesson covers how to manipulate object hierarchies in Nada.


 #  Learning Objectives


- Parenting / unparenting objects at runtime
- Accessing objects through the hierarchy in code


 #  Level Setup


- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [ New Project](../../../code_reference/command_reference.md#newproject)
 - Create a new project using the {nav icon=clone, name=Empty 2D Project} template
- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](../../../code_reference/command_reference.md#createsprite)
- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [Add Resource](../../../code_reference/command_reference.md#add)
 - Create a NadaScript resource using the Component template template and name it `SquareLogic`
- [Select](../../zilchmanual/editor/editorcommands/selectobject.md) : Sprite object
- In the `Properties Window`
 - Rename Sprite object to `Square`
 - [Add Component](../../zilchmanual/editor/addremovecomponent.md) : `SquareLogic`
- Update the `SquareLogic` script to the following:
```lang=csharp, name="SquareLogic"
class SquareLogic : NadaComponent
{
  [Dependency] var Transform : Transform;
  
  [Property]
  var RotateSpeed : Real = 5.0;
  
  function Initialize(init : CogInitializer)
  {
    Zilch.Connect(this.Space, Events.LogicUpdate, this.OnLogicUpdate);
  }

  function OnLogicUpdate(event : UpdateEvent)
  {
    var vel = this.RotateSpeed * event.Dt;
    this.Transform.RotateAnglesWorld(Real3(0.0, 0.0, vel));
  }
}
```

- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](../../../code_reference/command_reference.md#playgame)



![HierarchiesSetup](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/96155.gif)


*The Square object rotates*


- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [ StopGame](../../../code_reference/command_reference.md#stopgame)


 #  Parenting at Runtime


Let's create an archetype that can be used later to spawn child cogs at runtime.

- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](../../../code_reference/command_reference.md#createsprite)
- In the `Properties Window`
 - Rename Sprite object to `Circle`
 - Under [Sprite](../../../code_reference/class_reference/sprite.md)
  - Set SpriteSource enum to `Circle`
 - Set Archetype  to `CircleArchetype`
- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [Delete](../../../code_reference/command_reference.md#delete)

Now let's modify the `SquareLogic` component to spawn circles and parent them to the Square object

- Update the `SquareLogic` script to the following:

```lang=csharp, name=Square Logic
class SquareLogic : NadaComponent
{
  [Dependency] var Transform : Transform;

  [Property]
  var RotateSpeed : Real = 5.0;
  
  [Property]
  var ArchetypeToSpawn : Archetype = Archetype.CircleArchetype;
  
  [Property]
  var SpawnLocation : Real3 = Real3(0.0, 2.0, 0.0);
  
  function Initialize(init : CogInitializer)
  {
    Zilch.Connect(this.Space, Events.LogicUpdate, this.OnLogicUpdate);
  }

  function OnLogicUpdate(event : UpdateEvent)
  {
    var vel = this.RotateSpeed * event.Dt;
    this.Transform.RotateAnglesWorld(Real3(0.0, 0.0, vel));
    
    if(Zilch.Keyboard.KeyIsPressed(Keys.Space))
    {
      var obj = this.Space.CreateAtPosition(this.ArchetypeToSpawn, this.SpawnLocation);
      obj.AttachTo(this.Owner);
    }
  }
}
```

- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](../../../code_reference/command_reference.md#playgame)
 - Press key the `Space` key



![HierarchiesAttach](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/96165.gif)


*The `Space` bar spawns child Circle object objects*


- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [ StopGame](../../../code_reference/command_reference.md#stopgame)

Notice that the Circle object is attached to the Square object object as soon as it is created. That is done through invoking the [AttachTo](../../../code_reference/class_reference/cog.md#attachto-zilch-engine-doc) function on [ Cog](../../../code_reference/class_reference/cog.md), which takes a designated parent cog as its only parameter.

Similarly, you can call the [Detach](../../../code_reference/class_reference/cog.md#detach-void) function to unparent any object from its hierarchy:

- Add the following to the end of `OnLogicUpdate` function in the `SquareLogic` component:

```lang=csharp, name=Detaching
if(Zilch.Keyboard.KeyIsPressed(Keys.D))
{
   this.Owner.Children.Current.Detach();
}
```

- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](../../../code_reference/command_reference.md#playgame)
 - Press key the `Space` key a few times
 - Press key the `D` key a few times



![HierarchiesDettach](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/96252.gif)


*The `D` key detaches the child Circle object objects*


- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [ StopGame](../../../code_reference/command_reference.md#stopgame)

NOTE: Zilch also sends the [ Attached](../../../code_reference/event_reference.md#attached) and [ Detached](../../../code_reference/event_reference.md#detached) events to cogs when the respective operation is performed on them. Additionally, you can connect to the [ ChildAttached](../../../code_reference/event_reference.md#childattached) and [ ChildDetached](../../../code_reference/event_reference.md#childdetached) events on a parent objecct if you want to perform some logic upon acquiring or losing a child.


 #  Traversing Hierarchies at Runtime


Within a script, you can easily access a cog's parent:

- Add the following to the `SquareLogic` class:

```lang=csharp, name=Growth Property
[Property]
var Growth : Real = 1.1;
```

- In the `SquareLogic` class
 - In the `OnLogicUpdate` function
  - Below the line, `obj.AttachTo(this.Owner);`
   - Add the following code:

```lang=csharp, name=Accessing Parent
obj.Parent.Transform.Scale *= this.Growth;
```

- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](../../../code_reference/command_reference.md#playgame)
 - Press key the `Space` key



![HierarchiesParentAccess](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/96244.gif)


*The `Space` bar now also grows the parent Square object object*


- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [ StopGame](../../../code_reference/command_reference.md#stopgame)

You can also get a range containing all immediate children. Let's implement an addition to our previous script.

- Add the following to `OnLogicUpdate` function in the `SquareLogic` component:

```lang=csharp, name=Accessing Children
    if(Zilch.Keyboard.KeyIsPressed(Keys.Enter))
    {
      foreach(var child in this.Owner.Children)
      {
        child.Sprite.VertexColor = Colors.Red;
      }
    }
```

- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](../../../code_reference/command_reference.md#playgame)
 - Press key the `Space` key a few times
 - Press key the `Enter` key



![HierarchiesChildren](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/96250.gif)


*The `Enter` key now turns the child Circle object objects red*


- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [ StopGame](../../../code_reference/command_reference.md#stopgame)


 #  Related Materials
 ##  Tutorials
- [hierarchies](hierarchies.md)

 ##  Manual
- [gameobjectsconcept](../../zilchmanual/architecture/cogs/gameobjectsconcept.md)
- [archetype_basics](../../zilchmanual/architecture/archetypes/archetype_basics.md)

 ##  Reference
 ###  Classes
- [cog](../../../code_reference/class_reference/cog.md)
- [transform](../../../code_reference/class_reference/transform.md)
- [sprite](../../../code_reference/class_reference/sprite.md)

 ###  Events
- [ Attached](../../../code_reference/event_reference.md#attached)
- [ Detached](../../../code_reference/event_reference.md#detached)
- [ ChildAttached](../../../code_reference/event_reference.md#childattached)
- [ ChildDetached](../../../code_reference/event_reference.md#childdetached)

 ###  Commands
- [ CreateSprite](../../../code_reference/command_reference.md#createsprite)
- [ PlayGame](../../../code_reference/command_reference.md#playgame)
- [ StopGame](../../../code_reference/command_reference.md#stopgame)
- [ Delete](../../../code_reference/command_reference.md#delete)

 ##  Development Task
- T1189 

 
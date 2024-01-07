This lesson covers how to manipulate object hierarchies in Nada.


 #  Learning Objectives


- Parenting / unparenting objects at runtime
- Accessing objects through the hierarchy in code


 #  Level Setup


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ New Project](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#newproject)
 - Create a new project using the {nav icon=clone, name=Empty 2D Project} template
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#add)
 - Create a NadaScript resource using the Component template template and name it `SquareLogic`
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Sprite object
- In the `Properties Window`
 - Rename Sprite object to `Square`
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `SquareLogic`
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

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![HierarchiesSetup](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/96155.gif)


*The Square object rotates*


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)


 #  Parenting at Runtime


Let's create an archetype that can be used later to spawn child cogs at runtime.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- In the `Properties Window`
 - Rename Sprite object to `Circle`
 - Under [Sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md)
  - Set SpriteSource enum to `Circle`
 - Set Archetype  to `CircleArchetype`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [Delete](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#delete)

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

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
 - Press key the `Space` key



![HierarchiesAttach](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/96165.gif)


*The `Space` bar spawns child Circle object objects*


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

Notice that the Circle object is attached to the Square object object as soon as it is created. That is done through invoking the [AttachTo](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#attachto-zilch-engine-doc) function on [ Cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md), which takes a designated parent cog as its only parameter.

Similarly, you can call the [Detach](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md#detach-void) function to unparent any object from its hierarchy:

- Add the following to the end of `OnLogicUpdate` function in the `SquareLogic` component:

```lang=csharp, name=Detaching
if(Zilch.Keyboard.KeyIsPressed(Keys.D))
{
   this.Owner.Children.Current.Detach();
}
```

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
 - Press key the `Space` key a few times
 - Press key the `D` key a few times



![HierarchiesDettach](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/96252.gif)


*The `D` key detaches the child Circle object objects*


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

NOTE: Zilch also sends the [ Attached](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/event_reference.md#attached) and [ Detached](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/event_reference.md#detached) events to cogs when the respective operation is performed on them. Additionally, you can connect to the [ ChildAttached](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/event_reference.md#childattached) and [ ChildDetached](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/event_reference.md#childdetached) events on a parent objecct if you want to perform some logic upon acquiring or losing a child.


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

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
 - Press key the `Space` key



![HierarchiesParentAccess](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/96244.gif)


*The `Space` bar now also grows the parent Square object object*


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

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

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
 - Press key the `Space` key a few times
 - Press key the `Enter` key



![HierarchiesChildren](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/96250.gif)


*The `Enter` key now turns the child Circle object objects red*


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)


 #  Related Materials
 ##  Tutorials
- [hierarchies](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/tutorials/architecture/hierarchies.md)

 ##  Manual
- [gameobjectsconcept](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/architecture/cogs/gameobjectsconcept.md)
- [archetype_basics](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/architecture/archetypes/archetype_basics.md)

 ##  Reference
 ###  Classes
- [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)
- [transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
- [sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md)

 ###  Events
- [ Attached](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/event_reference.md#attached)
- [ Detached](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/event_reference.md#detached)
- [ ChildAttached](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/event_reference.md#childattached)
- [ ChildDetached](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/event_reference.md#childdetached)

 ###  Commands
- [ CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
- [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)
- [ Delete](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#delete)

 ##  Development Task
- T1189 

 
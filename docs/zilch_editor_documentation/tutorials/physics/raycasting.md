This lesson covers how to cast rays using Physics and interpret the results.


 # Learning Objectives

- Understanding rays, lines, and line segments
- Learning how to cast various geometric primitives
- Learning how to interpret and use the results of a cast

 # Level Setup

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ New Project](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#newproject)
 - Create a new project using the {nav icon=clone, name=Empty 2D Project} template
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- In the `Properties Window`
 - Rename Sprite object to `Square`
 - Under [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Translation  to `[-4, 0, 0]`

 - Create three sprite objects with the following properties:

| Name | `Transform>Translation` | `Sprite>VertexColor` | `Sprite>SpriteSource` |
|------------|---|---|---|
| RedCircle object     | `[-1.5, 0, 0]`| `[R:255, G:0, B:0, A:1.00]`| `Circle` |
| GreenCircle object  | `[0, 0, 0]`| `[R:0, G:255, B:0, A:1.00]` | `Circle` |
| BlueCircle object  | `[1.5, 0, 0]`| `[R:0, G:0, B:255, A:1.00]` | `Circle` |



![RaycastSetup](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/104850.png)


*The property values should look like this*


- - [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `MoveUpAndDown`
- In the `MoveUpAndDown` script
 - Update the `MoveUpAndDown` class to the following:

```lang=csharp, name="MoveUpAndDown"
class MoveUpAndDown : NadaComponent
{
  [Dependency] var Transform : Transform;
  
  [Property] 
  var StartPosition : Real3 = Real3(0,1,0);
  
  [Property] 
  var EndPosition : Real3 = Real3(0,-1,0);
  
  [Property]
  var MoveDuration : Real = 1.0;
  
  function Initialize(init : CogInitializer)
  {
    this.Transform.Translation = this.StartPosition;
    this.MoveToEnd();
  }
  
  function MoveToEnd()
  {
    var seq = Actions.Sequence(this.Owner.Actions);
    Actions.Property(seq, @this.Transform.Translation, this.EndPosition, this.MoveDuration, Ease.Linear);
    Actions.Call(seq, this.MoveToStart);
  }
  
  function MoveToStart()
  {
    var seq = Actions.Sequence(this.Owner.Actions);
    Actions.Property(seq, @this.Transform.Translation, this.StartPosition, this.MoveDuration, Ease.Linear);
    Actions.Call(seq, this.MoveToEnd);
  }
}
```

- For each Circle object
 - [ Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [spherecollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spherecollider.md)
 - [ Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [rigidbody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
 - Under [rigidbody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
  - Set DynamicState enum to `Kinematic`
 - [ Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `MoveUpAndDown`
 - Under `MoveUpAndDown`
  - Set the properties to the following:

|  Name |  StartPosition |  EndPosition |  MoveDuration  |
|--------|---------------|---------------|-----------------|
| RedCircle object | `[-1.5, 1, 0]` | `[-1.5, -1, 0]` | `1` |
| GreenCricle object | `[0, 1, 0]` | `[0, -1, 0]` | `2` |
| BlueCircle object | `[1.5, 1, 0]` | `[1.5, -1, 0]` | `3` |


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![RaycastSetup](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/105498.gif)

 *The circles should move like this*

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)


 # Rays

A ray is a portion of a line that starts at a given location and extends infinitely far in a given direction. In Zilch Engine, you can create rays and cast them in order to find what it intersects with. This can be used for a variety of applications, including:

 - Simulating laser beams
 - Simulating high velocity projectiles
 - Checking for line of sight
 - Detecting walls
 - Detecting distance to an object

NOTE:
  It's worth noting the difference between rays, segments and lines. Rays are infinitely long, defined by a start point and a direction. Segments are defined by a start and end point. Lines are defined by two points and extend infinitely.
  ![Ray](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/104865.gif) ![Segment](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/104867.gif) ![Line](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/104869.gif)

 # Creating and Casting

The first step to raycasting is to build the ray with the desired parameters. Let's take a look.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `RayCasterLogic`
- In the `RayCasterLogic` script
 - Update the `RayCasterLogic` class to the following:

```lang=csharp, name="Ray Casting"
class RayCasterLogic : NadaComponent
{
  [Dependency] var Transform : Transform;
  
  [Property]
  var Direction : Real3 = Real3(1.0, 0.0, 0.0);
  
  [Property]
  var DebugDrawOn : Boolean = true;
  
  [Property]
  var MaxDebugLineLength : Real = 8.0;
  
  function Initialize(init : CogInitializer)
  {
    Zilch.Connect(this.Space, Events.LogicUpdate, this.OnLogicUpdate);
  }

  function OnLogicUpdate(event : UpdateEvent)
  {
    this.FindFirstObject();
  }
  
  function FindFirstObject()
  {
    //Create ray
    var ray = Ray();
    ray.Start = this.Transform.Translation;
    ray.Direction = this.Direction;
    
    //Cast ray
    var result = this.Space.PhysicsSpace.CastRayFirst(ray);
    
    //Interpret results
    if(result.ObjectHit != null)
    {
      //Set our owner's color to match the color of the object we hit
      this.Owner.Sprite.VertexColor = result.ObjectHit.Sprite.VertexColor;
      Console.WriteLine("Ray found: `result.ObjectHit.Name`");
    }
    else
    {
      //If no objects were hit, set our owner's color to white
      this.Owner.Sprite.VertexColor = Colors.White;
      Console.WriteLine("No object found!");
    }
    
    //Visual Debug
    if(this.DebugDrawOn)
    {
      var debugRay = DebugLine();
      debugRay.Start = ray.Start;
      debugRay.End = ray.Start + Real3.XAxis * Math.Min(result.Distance, this.MaxDebugLineLength);
      debugRay.HeadSize = 0.2;
      DebugDraw.Add(debugRay);
    }   
  }
}
```
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Square object
- In the `Properties Window`
 - [ Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `RaycasterLogic`

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![RaycastFirst](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/105501.gif)


*We can see the ray starting at the Square object and extending to the right. Upon intersecting with one of the circles, the color of the square is changed to match it.*


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)



Raycasting always consists of 3 steps:

1. Create the [Ray](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ray.md)
2. Request the [PhysicsSpace](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md) to cast it (storing the results)
3. Interpret the [CastResult](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castresult.md)

If the ray intersects an object, you can retrieve the following information from the [CastResult](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castresult.md):

|CastResult |
|------------|
| Collider | The collider intersected by the ray |
| Distance | Distance from the ray start to the point of intersection|
| ObjectHit | The cog hit by the cast|
| Normal | The normal of the surface at the intersection point |
| WorldPosition |World-space position where the object was hit|

 # Multiple Results

It is also possible to cast a Ray and retrieve the resulting intersections with multiple objects by using the [ PhysicsSpace.CastRay()](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md) function instead.

- Add the following function to the `RayCasterLogic` class:

```lang=csharp, name="Multiple Results"
  function FindSeveralObjects()
  {
    //Create Ray
    var ray = Ray();
    ray.Start = this.Transform.Translation;
    ray.Direction = this.Direction;
    
    //Cast Ray
    var results = this.Space.PhysicsSpace.CastRay(ray, 3);
    
    this.Owner.Sprite.VertexColor = Real4(0,0,0,1);
    
    //Interpret Results
    foreach(var result in results)
    {
      //If the object has a sprite component
      if(result.ObjectHit.Sprite != null)
      {
        //Add that object's color to our owner's color
        this.Owner.Sprite.VertexColor += result.ObjectHit.Sprite.VertexColor;
      }
    }
    
    //Visual Debug
    if(this.DebugDrawOn)
    {
      var debugRay = DebugLine();
      debugRay.Start = ray.Start;
      debugRay.End = ray.Start + Real3.XAxis * this.MaxDebugLineLength;
      debugRay.HeadSize = 0.2;
      DebugDraw.Add(debugRay);
    }
  }
```

- Replace the `OnLogicUpdate` function in the `RayCasterLogic` class with the following:

```lang=csharp, name="New Logic Update"
  function OnLogicUpdate(event : UpdateEvent)
  {
      //this.FindFirstObject();
      this.FindSeveralObjects();
  }
```

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![RaycastMultiple](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/105983.gif)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

The [ CastRay](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md) function allows you to specify the ray and a maximum number of objects to detect. It returns a range of [ CastResults](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castresult.md) that contains all of the objects intersected (up to the specified number) in order of distance (closest to farthest).

 # Cast Filters

[ CastFilters](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castfilter.md) allow you to customize which objects the raycast process should hit and which should be ignored. The filter can then be passed as an optional third parameter to the `CastRay` function.

- Replace the `FindSeveralObjects` function in the `RayCasterLogic` class with the following :

```lang=csharp, name="Filter Example"
  function FindSeveralObjects()
  {
    //Create Filter
    var filter = CastFilter();
    filter.IgnoreGhost = true;
    
    //Create Ray
    var ray = Ray();
    ray.Start = this.Transform.Translation;
    ray.Direction = this.Direction;
    
    //Cast Ray
    var results = this.Space.PhysicsSpace.CastRay(ray, 3, filter);
    
    this.Owner.Sprite.VertexColor = Real4(0,0,0,1);
    
    //Interpret Results
    foreach(var result in results)
    {
      //If the object has a sprite component
      if(result.ObjectHit.Sprite != null)
      {
        //Add that object's color to our owner's color
        this.Owner.Sprite.VertexColor += result.ObjectHit.Sprite.VertexColor;
      }
    }
    
    //Visual Debug
    if(this.DebugDrawOn)
    {
      var debugRay = DebugLine();
      debugRay.Start = ray.Start;
      debugRay.End = ray.Start + Real3.XAxis * this.MaxDebugLineLength;
      debugRay.HeadSize = 0.2;
      DebugDraw.Add(debugRay);
    }
  }
```

- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : GreenCircle object
- In the `Properties Window`
 - Under [SphereCollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spherecollider.md)
  - Set  Ghost checkBox to `true`

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![RaycastMultipleFiltered](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/105986.gif)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

Here are some useful properties you can set on the [CastFilter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castfilter.md) that allow you to further customize which objects to ignore.

|Cast Filter|
|-----------|
|IgnoreCog| [Cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)| A given specific Cog to ignore |
|IgnoreDynamic| [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)| Ignores all objects marked as [Dynamic](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#rigidbodydynamicstate)|
|IgnoreGhost| [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)| Ignores all objects marked as [Ghost](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md#ghost)|
|IgnoreKinematic| [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)| Ignores all objects marked as [Kinematic](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#rigidbodydynamicstate)|
|IgnoreStatic| [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)| Ignores all objects marked as [Static](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#rigidbodydynamicstate)|
|CollisionGroup| [collisiongroup](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisiongroup.md)| Makes the Ray behave as part of a collision group, using the current [collisiontable](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisiontable.md) |



 # Other Types of Casting

In addition to Rays, Zilch Engine allows you to cast other types of shapes, including:

- [Segment](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/segment.md)
- [Sphere](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sphere.md)
- [Aabb](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md)
- [Frustum](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/frustum.md)
- [Collider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md)

They all follow the same basic steps described in this tutorial: define the shape, request [PhysicsSpace](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md) to cast it (with the optional inclusion of a [CastFilter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castfilter.md)) and then interpret the results. You can read more about them in the [ PhysicsCasting](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/physicscasting.md) Manual Page.


 # Related Materials

 ## Manual
- [ PhysicsCasting](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/physicscasting.md)
- [ Colliders](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/colliders.md)
- [ Collision Groups and Tables](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/physics/collisionoverview/collisiongroupsandtables.md)

 ## Tutorial
- [collisiongroups](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/tutorials/physics/collision/collisiongroups.md)


 ## Code Reference
 ### Classes
- [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
- [Sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md)
- [Cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)
- [spherecollider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spherecollider.md)
- [Ray](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ray.md)
- [Segment](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/segment.md)
- [CastFilter](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castfilter.md)
- [CastResult](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/castresult.md)
- [PhysicsSpace](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/physicsspace.md)
- [Collider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md)
- [collisiongroup](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisiongroup.md)
- [collisiontable](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisiontable.md)
- [sphere](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sphere.md)
- [aabb](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/aabb.md)
- [frustum](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/frustum.md)

 ## Enums
- [RigidBodyDynamicState](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#rigidbodydynamicstate)

 ### Commands
- [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
- [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)


 ## Development Task
- T1188 

 
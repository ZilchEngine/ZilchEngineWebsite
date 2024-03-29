This lesson covers how to cast rays using Physics and interpret the results.


 # Learning Objectives

- Understanding rays, lines, and line segments
- Learning how to cast various geometric primitives
- Learning how to interpret and use the results of a cast

 # Level Setup

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [New Project](../../../code_reference/command_reference.md#newproject)
 - Create a new project using the {nav icon=clone, name=Empty 2D Project} template
- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](../../../code_reference/command_reference.md#createsprite)
- In the `Properties Window`
 - Rename Sprite object to `Square`
 - Under [Transform](../../../code_reference/class_reference/transform.md)
  - Set Translation  to `[-4, 0, 0]`

 - Create three sprite objects with the following properties:

| Name | `Transform>Translation` | `Sprite>VertexColor` | `Sprite>SpriteSource` |
|------------|---|---|---|
| RedCircle object     | `[-1.5, 0, 0]`| `[R:255, G:0, B:0, A:1.00]`| `Circle` |
| GreenCircle object  | `[0, 0, 0]`| `[R:0, G:255, B:0, A:1.00]` | `Circle` |
| BlueCircle object  | `[1.5, 0, 0]`| `[R:0, G:0, B:255, A:1.00]` | `Circle` |



![RaycastSetup](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/104850.png)


*The property values should look like this*


- - [Command](../../zilchmanual/editor/editorcommands/commands.md) : [Add Resource](../../zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `MoveUpAndDown`
- In the `MoveUpAndDown` script
 - Update the `MoveUpAndDown` class to the following:

```TS:"MoveUpAndDown"
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
 - [Add Component](../../zilchmanual/editor/addremovecomponent.md) : [spherecollider](../../../code_reference/class_reference/spherecollider.md)
 - [Add Component](../../zilchmanual/editor/addremovecomponent.md) : [rigidbody](../../../code_reference/class_reference/rigidbody.md)
 - Under [rigidbody](../../../code_reference/class_reference/rigidbody.md)
  - Set DynamicState enum to `Kinematic`
 - [Add Component](../../zilchmanual/editor/addremovecomponent.md) : `MoveUpAndDown`
 - Under `MoveUpAndDown`
  - Set the properties to the following:

|  Name |  StartPosition |  EndPosition |  MoveDuration  |
|--------|---------------|---------------|-----------------|
| RedCircle object | `[-1.5, 1, 0]` | `[-1.5, -1, 0]` | `1` |
| GreenCricle object | `[0, 1, 0]` | `[0, -1, 0]` | `2` |
| BlueCircle object | `[1.5, 1, 0]` | `[1.5, -1, 0]` | `3` |


- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [PlayGame](../../../code_reference/command_reference.md#playgame)



![RaycastSetup](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/105498.gif)

 *The circles should move like this*

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [StopGame](../../../code_reference/command_reference.md#stopgame)


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

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [Add Resource](../../zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `RayCasterLogic`
- In the `RayCasterLogic` script
 - Update the `RayCasterLogic` class to the following:

```TS:"Ray Casting"
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
- [Select](../../zilchmanual/editor/editorcommands/selectobject.md) : Square object
- In the `Properties Window`
 - [Add Component](../../zilchmanual/editor/addremovecomponent.md) : `RaycasterLogic`

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [PlayGame](../../../code_reference/command_reference.md#playgame)



![RaycastFirst](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/105501.gif)


*We can see the ray starting at the Square object and extending to the right. Upon intersecting with one of the circles, the color of the square is changed to match it.*


- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [StopGame](../../../code_reference/command_reference.md#stopgame)



Raycasting always consists of 3 steps:

1. Create the [Ray](../../../code_reference/class_reference/ray.md)
2. Request the [PhysicsSpace](../../../code_reference/class_reference/physicsspace.md) to cast it (storing the results)
3. Interpret the [CastResult](../../../code_reference/class_reference/castresult.md)

If the ray intersects an object, you can retrieve the following information from the [CastResult](../../../code_reference/class_reference/castresult.md):

|CastResult |
|------------|
| Collider | The collider intersected by the ray |
| Distance | Distance from the ray start to the point of intersection|
| ObjectHit | The cog hit by the cast|
| Normal | The normal of the surface at the intersection point |
| WorldPosition |World-space position where the object was hit|

 # Multiple Results

It is also possible to cast a Ray and retrieve the resulting intersections with multiple objects by using the [PhysicsSpace.CastRay()](../../../code_reference/class_reference/physicsspace.md) function instead.

- Add the following function to the `RayCasterLogic` class:

```TS:"Multiple Results"
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

```TS:"New Logic Update"
  function OnLogicUpdate(event : UpdateEvent)
  {
      //this.FindFirstObject();
      this.FindSeveralObjects();
  }
```

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [PlayGame](../../../code_reference/command_reference.md#playgame)



![RaycastMultiple](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/105983.gif)


- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [StopGame](../../../code_reference/command_reference.md#stopgame)

The [CastRay](../../../code_reference/class_reference/physicsspace.md) function allows you to specify the ray and a maximum number of objects to detect. It returns a range of [CastResults](../../../code_reference/class_reference/castresult.md) that contains all of the objects intersected (up to the specified number) in order of distance (closest to farthest).

 # Cast Filters

[CastFilters](../../../code_reference/class_reference/castfilter.md) allow you to customize which objects the raycast process should hit and which should be ignored. The filter can then be passed as an optional third parameter to the `CastRay` function.

- Replace the `FindSeveralObjects` function in the `RayCasterLogic` class with the following :

```TS:"Filter Example"
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

- [Select](../../zilchmanual/editor/editorcommands/selectobject.md) : GreenCircle object
- In the `Properties Window`
 - Under [SphereCollider](../../../code_reference/class_reference/spherecollider.md)
  - Set  Ghost checkBox to `true`

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [PlayGame](../../../code_reference/command_reference.md#playgame)



![RaycastMultipleFiltered](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/105986.gif)


- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [StopGame](../../../code_reference/command_reference.md#stopgame)

Here are some useful properties you can set on the [CastFilter](../../../code_reference/class_reference/castfilter.md) that allow you to further customize which objects to ignore.

|Cast Filter|
|-----------|
|IgnoreCog| [Cog](../../../code_reference/class_reference/cog.md)| A given specific Cog to ignore |
|IgnoreDynamic| [boolean](../../../code_reference/nada_base_types/boolean.md)| Ignores all objects marked as [Dynamic](../../../code_reference/enum_reference.md#rigidbodydynamicstate)|
|IgnoreGhost| [boolean](../../../code_reference/nada_base_types/boolean.md)| Ignores all objects marked as [Ghost](../../../code_reference/class_reference/collider.md#ghost)|
|IgnoreKinematic| [boolean](../../../code_reference/nada_base_types/boolean.md)| Ignores all objects marked as [Kinematic](../../../code_reference/enum_reference.md#rigidbodydynamicstate)|
|IgnoreStatic| [boolean](../../../code_reference/nada_base_types/boolean.md)| Ignores all objects marked as [Static](../../../code_reference/enum_reference.md#rigidbodydynamicstate)|
|CollisionGroup| [collisiongroup](../../../code_reference/class_reference/collisiongroup.md)| Makes the Ray behave as part of a collision group, using the current [collisiontable](../../../code_reference/class_reference/collisiontable.md) |



 # Other Types of Casting

In addition to Rays, Zilch Engine allows you to cast other types of shapes, including:

- [Segment](../../../code_reference/class_reference/segment.md)
- [Sphere](../../../code_reference/class_reference/sphere.md)
- [Aabb](../../../code_reference/class_reference/aabb.md)
- [Frustum](../../../code_reference/class_reference/frustum.md)
- [Collider](../../../code_reference/class_reference/collider.md)

They all follow the same basic steps described in this tutorial: define the shape, request [PhysicsSpace](../../../code_reference/class_reference/physicsspace.md) to cast it (with the optional inclusion of a [CastFilter](../../../code_reference/class_reference/castfilter.md)) and then interpret the results. You can read more about them in the [PhysicsCasting](../../zilchmanual/physics/physicscasting.md) Manual Page.


 # Related Materials

 ## Manual
- [PhysicsCasting](../../zilchmanual/physics/physicscasting.md)
- [Colliders](../../zilchmanual/physics/colliders.md)
- [Collision Groups and Tables](../../zilchmanual/physics/collisionoverview/collisiongroupsandtables.md)

 ## Tutorial
- [collisiongroups](collision/collisiongroups.md)


 ## Code Reference
 ### Classes
- [Transform](../../../code_reference/class_reference/transform.md)
- [Sprite](../../../code_reference/class_reference/sprite.md)
- [Cog](../../../code_reference/class_reference/cog.md)
- [spherecollider](../../../code_reference/class_reference/spherecollider.md)
- [Ray](../../../code_reference/class_reference/ray.md)
- [Segment](../../../code_reference/class_reference/segment.md)
- [CastFilter](../../../code_reference/class_reference/castfilter.md)
- [CastResult](../../../code_reference/class_reference/castresult.md)
- [PhysicsSpace](../../../code_reference/class_reference/physicsspace.md)
- [Collider](../../../code_reference/class_reference/collider.md)
- [collisiongroup](../../../code_reference/class_reference/collisiongroup.md)
- [collisiontable](../../../code_reference/class_reference/collisiontable.md)
- [sphere](../../../code_reference/class_reference/sphere.md)
- [aabb](../../../code_reference/class_reference/aabb.md)
- [frustum](../../../code_reference/class_reference/frustum.md)

 ## Enums
- [RigidBodyDynamicState](../../../code_reference/enum_reference.md#rigidbodydynamicstate)

 ### Commands
- [CreateSprite](../../../code_reference/command_reference.md#createsprite)
- [PlayGame](../../../code_reference/command_reference.md#playgame)
- [StopGame](../../../code_reference/command_reference.md#stopgame)


 ## Development Task
- T1188 

 
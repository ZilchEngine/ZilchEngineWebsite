The `SAMPLECHARACTERCONTROLLERS[1.0]` package on the [ Zilch Market](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/tutorials/external_zilch_engine_tools/the_market.md) contains 2D and 3D input scripts that work with the `SweptController` component also included in the package. The `SweptController` is a generic kinematic character controller that is useful when prototyping many 2D and 3D game concepts.


 #  Learning Objectives


- Character controller explanation
- Kinematic vs Dynamic
- SweptController usage


 #  Level Setup


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ New Project](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#newproject)
 - Create a new project using the {nav icon=clone, name=Empty 2D Project} template
- Click  the market button in the top right of the editor window
  ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/106205.png)
- Click  the `Sample Character Controller` package
  ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/106207.png)
- Click  the download link for the `SAMPLECHARACTERCONTROLLERS[1.0].ZEROPACK`
  ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/106209.png)
- Click  the Import button button
  ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/106211.png)
- Close the `Market Browser`

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ CreateCube](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createcube)
- In the `Properties Window`
 - Under [ Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Scale  to `[50,1,1]`
 - Under [ RigidBody](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/rigidbody.md)
  - Set DynamicState enum to [Static](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#rigidbodydynamicstate)
- In the `Library Window`
 - Under Archetype 
  - `Click and drag` {nav icon=wrench, name=SweptPlayer2_5D} into the `Level Window`
    ![SweptArchetype](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/106215.gif)
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)

 - Move left with `A` and right with `D`
 - Jump with `Space`



![Swept2DMoving](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/106217.gif)


*The Player object moving and jumping*


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)


 #  SweptInput


Let's take a look at the `SweptInput2D` component.

```name=SweptInput2D, lang=csharp
class SweptInput2D : NadaComponent
{
  [Dependency] var SweptController : SweptController;
  
  [Property] var LeftKey : Keys = Keys.A;
  [Property] var RightKey : Keys = Keys.D;
  [Property] var JumpKey : Keys = Keys.Space;
  
  function Initialize(init : CogInitializer)
  {
    Zilch.Connect(this.Space, Events.LogicUpdate, this.OnLogicUpdate);
  }

  function OnLogicUpdate(event : UpdateEvent)
  {
    var movement = Real3(0, 0, 0);
    
    // Check for left/right movment
    if(Zilch.Keyboard.KeyIsDown(this.LeftKey))
      movement.X = -1;
    if(Zilch.Keyboard.KeyIsDown(this.RightKey))
      movement.X = 1;
    
    if(Zilch.Keyboard.KeyIsPressed(this.JumpKey))
    {
      this.SweptController.Jump();
    }
    
    this.SweptController.Update(movement, event.Dt);
  }
}
```

Very similar to our dynamic character controller from the [first input tutorial](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/tutorials/gameplay/input1.md), we need to calculate a direction in which to move and whether the character should jump. Using the input properties, we can configure which inputs drive the `SweptController`.

The important line to note in `SweptInput2D` is `this.SweptController.Update(movement, event.Dt);`. `SweptController.Update` must be called every frame on which the character should be moving. This function handles much of the behavior of the SweptController and should always be called at the end of the input detection update function in order to apply any changes that were made to SweptController properties that frame.


 #  Swept Controller Properties


Because the SweptCharacter uses a `Kinematic` object, it must handle its own gravity behavior. The strength of this gravitational acceleration can be adjusted per object.

- In the `Properties Window` for Player object
 - Under `SweptController`
  - Set Gravity  to `50`

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
 - Jump with `Space`



![SweptGravity](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/99693.gif)


*The Player object jumping with increased Gravity *


Notice that the acceleration of gravity is now more powerful. 

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

The jump velocity is also adjustable. 

- In the `Properties Window`
 - Under `SweptController`
  - Set JumpSpeed  to `25`

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![SweptJumpSpeed](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/99695.gif)


*The Player object jumping with increased Gravity  and increased JumpSpeed *


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

Using these values alongside MaxFallSpeed  allows you determine how fast your character rises and falls with each jump.


 ##  In-Air Control


When the swept character is in the air, it has slight control by default. The SweptController allows you to modify the strength of that control.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
 - Jump and then move side to side while in the air



![air_control_default](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/103377.gif)


*The Player object jumping and moving with default AirAcceleration *


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

Now let's try increasing the air control.

 - In the `Properties Window`
  - Under `SweptController`
   - Set AirAcceleration  to `25`

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
 - Jump and then move side to side while in the air



![air_control_High](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/103379.gif)


*The Player object jumping and moving with increased AirAcceleration *


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

In addition to changing the rate of acceleration in the air, you can also modify the GroundAcceleration  to similarly affect the SweptCharacter's acceleration when not in the air.


 #  Max Ground Slope


Something you may not have thought about yet is how the `SweptController` detects whether it is *on ground// or not. There are certain behaviors, such as jumping, that should only occur when the object is //on ground//. This //ground detection* is done through a technique called //swept collision//, which is too advanced to cover in this tutorial. The final step of ground detection, though, is to check the angle of the slope that the character is on. If the slope is too steep, the SweptController will cause the character to slide down it instead of being able to move up it.

- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Cube object
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [Duplicate](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#duplicate)

- In the `Properties Window`
 - Under [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Translation  to `[5,0,0]`
  - Set Rotation  to `[0,0,25]`

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [Duplicate](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#duplicate)
- In the `Properties Window`
 - Under [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
  - Set Translation  to `[-5,0,0]`
  - Set Rotation  to `[0,0,-50]`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
 - Attempt to move onto all 3 platforms



![ground_angle](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/106219.gif)


*Platforms both above and below the MaxGroundSlope *


Notice how the Player object object can move freely on the platform with a rotation of `[0,0,25]`, but when it attempts to move onto the platform with a rotation of `[0,0,-50]`, it slides off. This is due to the Z-Axis rotation of the lefthand platform having a greater magnitude than the MaxGroundSlope  of the Player object's SweptController.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)


 #  Swept Collision


Collision events were covered in [the events tutorial](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/tutorials/scripting/events.md#collision-events). Now let's take a look at how they interact with the SweptController.


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `CollisionDetector`
- Update the `CollisionDetector` script to the following:

```lang=csharp, name="CollisionDetector"
class CollisionDetector : NadaComponent
{
  function Initialize(init : CogInitializer)
  {
    Zilch.Connect(this.Owner, Events.CollisionStarted, this.OnCollisionStarted);
  }

  function OnCollisionStarted(event : CollisionEvent)
  {
    Console.WriteLine("`this.Owner` collided with `event.OtherObject`");
  }
}
```
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Player object
 - [ Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `CollisionDetector`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Console](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#console)
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)

```name=Console Output
---------------- Begin Game ----------------
Loaded level 0.00s
Level 'Level' was loaded.
Loaded level 0.00s
----------------  End Game  ----------------
```
Notice how our print statement from the `CollisionDetector` component is not executed. This is due to the fact that no standard collision is actually occurring here. The SweptController moves the player by predicting collision based on input and then translating to the correct point to simulate collision resolution. The result is that the kinematic collider of the Player object never actually touches the static colliders of the platforms.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)
- In the `Properties Window`
 - Under `SweptController`
  - Set ForwardEvents checkBox to `true`


![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/105946.png)

- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Player object
 - [ Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [customcollisioneventtracker](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customcollisioneventtracker.md)

The [customcollisioneventtracker](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customcollisioneventtracker.md) detects circumstances where standard [CollisionEvents](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisionevent.md) would be sent out and dispatches them when a [collider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collider.md) component would be involved in a standard collision.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)

```name="Console Output"
---------------- Begin Game ----------------
Loaded level 0.00s
Level 'Level' was loaded.
Loaded level 0.00s
<Cog 'Player' (SweptPlayer2D) [2035]> collided with <Cog 'Cube' [2034]>
----------------  End Game  ----------------
```

Now we can detect and react to the [CollisionEvents](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/collisionevent.md) sent by the [customcollisioneventtracker](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customcollisioneventtracker.md).

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)


 #  Related Materials
 ##  Tutorials
- [input1](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/tutorials/gameplay/input1.md)
- [#collision-events](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/tutorials/scripting/events.md#collision-events)

 ##  Manual
- [commands](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md)
- [selectobject](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md)

 ##  Reference
 ### Commands
- [ NewProject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#newproject)
- [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
- [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)
- [ CreateCube](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createcube)
- [ Duplicate](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#duplicate)

 ###  Classes
- [transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
- [customcollisioneventtracker](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/customcollisioneventtracker.md)

 ###  Events
- [ CollisionStarted](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/event_reference.md#collisionstarted)

 ###  Enums
- [ RigidBodyDynamicState.Static](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#rigidbodydynamicstate)

 ## Tasks
- T1181 

 
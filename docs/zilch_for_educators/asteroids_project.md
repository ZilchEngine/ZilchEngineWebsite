This page outlines the steps need to create a basic version of the classic game Asteroids. You should make sure you understand the content of the #basic_tutorials tagged with #beginner_iii before beginning this project.

NOTE: Like other project pages this tutorial does not cover every tiny step the user must complete and instead summarizes. This requires the reader to understand basic concepts from preceeding tutorials to complete the project.

 # Learning Objectives

- Reaffirm the learning objectives of #beginner_iii tutorials.

 # Level Setup

- [ Command](../zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ New Project](../code_reference/command_reference.md#newproject)
- [Remove ](../zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) the [GravityEffect](../code_reference/class_reference/gravityeffect.md) from the LevelSettings object.
- [Remove ](../zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) the [DragEffect](../code_reference/class_reference/drageffect.md) from the LevelSettings object.

 # The Player
 ## Player Archetype
- [ Command](../zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](../zilch_editor_documentation/zilchmanual/editor/editorcommands/createobject.md)
 - Rename the new sprite to `Player`
- [Add component](../zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) [RigidBody](../code_reference/class_reference/rigidbody.md) to the Player object
- [Add component](../zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) [Orientation](../code_reference/class_reference/orientation.md) to the Player object
 - Set [Orientation.DefaultOrienationBases](../code_reference/class_reference/orientation.md#defaultorientationbases) to [ForwardZUpY](../code_reference/enum_reference.md#orientationbases)
- Upload the Player object to a new archetype called `Player`

 ## Player Movement
- [ Command](../zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](../zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
- Create a NadaScript resource using the Component template template and name it `PlayerMovement`
 - [Add component](../zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) `PlayerMovement` to the Player object
- Upload the Player object to a new archetype called `Player`

 ### Properties
- Define properties of type [Keys](../code_reference/enum_reference.md#keys) in `PlayerMovement` for the forward, backward, left, right, and shoot keys for the player
- Define properties of type [Real](../code_reference/nada_base_types/real.md) called `Speed` and `RotationSpeed`

 ### Moving
- Connect to [LogicUpdate](../code_reference/event_reference.md#logicupdate) in the `PlayerMovement` component.
- In `PlayerMovement` in `OnLogicUpdate`
 - Declare a local `movement` variable
 - Check if the `Forward` and `Backward` input keys defined above are down using [Zilch.Keyboard.KeyIsDown()](../code_reference/class_reference/keyboard.md#keyisdown-zilch-engine-do)
 - If the `Forward` is down add [Orientation.WorldForward](../code_reference/class_reference/orientation.md#worldforward-zilch-engine) to `movement`
 - If the `Backward` is down subtract [Orientation.WorldForward](../code_reference/class_reference/orientation.md#worldforward-zilch-engine) to `movement`
 - [Normalize](../code_reference/nada_base_types/math.md#normalize-zilch-engine-do) `movement`
 - Set [RigidBody.Velocity](../code_reference/class_reference/rigidbody.md#velocity-zilch-engine-doc) to `movement * this.Speed`

 ### Rotating
- In `PlayerMovement` in `OnLogicUpdate`
 - Declare a local `rotation` variable
- Check if the `Left` and `Right` input keys defined above are down using [Zilch.Keyboard.KeyIsDown()](../code_reference/class_reference/keyboard.md#keyisdown-zilch-engine-do)
 - If the `Left` is down add [Orientation.WorldUp](../code_reference/class_reference/orientation.md#worldup-zilch-engine-docu) to `rotation`
 - If the `Right` is down subtract [Orientation.WorldUp](../code_reference/class_reference/orientation.md#worldup-zilch-engine-docu) to `rotation`
- Declare a local variable `rotationSpeedRadians` and initialize it to `RotationSpeed` converted [to radians](../code_reference/nada_base_types/math.md#toradians-zilch-engine-do).
- Use [Transform.RotateWorld()](../code_reference/class_reference/transform.md#rotateworld-void) to rotate the object by `rotation * rotationSpeedRadians * event.Dt`

 ## Player Shooting
- [ Command](../zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](../zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
- Add a NadaScript resource using the Component template template and name it `ObjectSpawner`
 - [Add component](../zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) `ObjectSpawner` to the Player object
- [ Command](../zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](../zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
- Add a NadaScript resource using the Component template template and name it `CreateOnInput`
 - [Add component](../zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) `CreateOnInput` to the Player object
- Upload the Player object to a new archetype called `Player`

 ### Properties
- In `ObjectSpawner`
 - Define a property of type [Archetype](../code_reference/class_reference/archetype.md) named `ArchetypeToSpawn`
 - Define a property of type [Real](../code_reference/nada_base_types/real.md) named `InitialVelocity`
 - Define a property of type [Boolean](../code_reference/nada_base_types/boolean.md) named `UseRandomDirection` (defaulting to `false`)

- In `CreateOnInput`
 - Define a property of type [Keys](../code_reference/enum_reference.md#keys) in `ObjectSpawner` named `SpawnKey`

 ### Spawning Projectiles
- In the `ObjectSpawner` component
 - Create a new function named `SpawnObject()`
 - In `SpawnObject()`
  - [Create](../code_reference/class_reference/space.md#createatposition-zilch-en) a `ArchetypeToSpawn` object at the [position](../code_reference/class_reference/transform.md#worldtranslation-zilch-en) of the Player object
  - If `ObjectSpawner.UseRandomDirection` is true then get a normalized random direction, or if `UseRandomDirection` is false use `Orientation.WorldForward` for the direction of the object's inital velocity.
  - Set the initial velocity of the object.


- In the `CreateOnInput` component.
 - Connect to [LogicUpdate](../code_reference/event_reference.md#logicupdate)
 - In `OnLogicUpdate`
  - Check if `SpawnKey` is down using [Zilch.Keyboard.KeyIsDown()](../code_reference/class_reference/keyboard.md#keyisdown-zilch-engine-do)
  - If `SpawnKey` is down then call `ObjectSpawner.SpawnObject()`

 - Set the [velocity](../code_reference/class_reference/rigidbody.md#velocity-zilch-engine-doc) of the newly created Projectile object to `this.InitialVelocity * this.Owner.Orientation.WorldForward`


 # The Projectile
- [ Command](../zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](../zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
- Create a NadaScript resource using the Component template template and name it `DestroyOnCollision`
 - [Add component](../zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) `DestroyOnCollision` to the Projectile object
- Under the `Sprite` component change the `VertexColor`
- Upload the Projectile object to a new archetype called `Projectile`

 ## DestroyOnCollision
 ### Properties
- In `DestroyOnCollision`
 - Define a property of type [Boolean](../code_reference/nada_base_types/boolean.md) named `DestroyOwner` (defaulting to `false`)
 - Define a property of type [Boolean](../code_reference/nada_base_types/boolean.md) named `DestroyOther` (defaulting to `false`)

 ### Destroying On Collision
- In `DestroyOnCollision`
 - Connect to the `CollisionStarted` event
 - In `OnCollisionStarted`
  - If `DestroyOther` is true call `event.OtherObject.Destroy()`
  - If `DestroyOwner` is true call `this.Owner.Destroy()`

- Play the game
 - At this point the ship should be able to move, rotate, and shoot.

 # Astroids
- [ Command](../zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](../zilch_editor_documentation/zilchmanual/editor/editorcommands/createobject.md)
 - Rename the new sprite to `Asteroid`
- [Add component](../zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) [RigidBody](../code_reference/class_reference/rigidbody.md) to the Asteroid object
- [Add component](../zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) [BoxCollider](../code_reference/class_reference/boxcollider.md) to the Asteroid object
- [Add component](../zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) `DestroyOnCollision` to the Asteroid object
- Upload the `Asteroid` archetype

 ## Spawning Asteroids
- [ Command](../zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](../zilch_editor_documentation/zilchmanual/editor/editorcommands/createobject.md)
 - Rename the new sprite to `AsteroidSpawner`
- [Add component](../zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) [Orientation](../code_reference/class_reference/orientation.md) to the AsteroidSpawner object
- [Add component](../zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) `ObjectSpawner` to the AsteroidSpawner object

 ### CreateOnInterval Component
- Add a NadaScript resource using the Component template template and name it `CreateOnInterval`
 - [Add component](../zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) `CreateOnInterval` to the AsteroidSpawner object
- Move the AsteroidSpawner object outside the viewport so the GameCamera object can not see it
- Upload the AsteroidSpawner object to a new archetype called `AsteroidSpawner`

 ### Properties
- In `CreateOnInterval`
 - Define a property of type [Real](../code_reference/nada_base_types/real.md) in `CreateOnInterval` named `SpawnRate`
 - Define a property of type [Boolean](../code_reference/nada_base_types/boolean.md) in `CreateOnInterval` named `StartOnInit` defaulting to `true`
 - Define a non-property member variable of type [ActionsSet](../code_reference/class_reference/actionset.md) in `CreateOnInterval` named `SpawnSequence`

 ### Interval Spawning
- In `CreateOnInterval`
 - Declare a function named `StartSpawnSequence`
 - In `StartSpawnSequence`
  - Construct a new ActionSequence using `this.Owner.Actions` and assign it to the member variable `SpawnSequence`
   - Construct a `Delay` action using `SpawnSequence` and `SpawnRate`
   - Construct a `Call` action using `SpawnSequence` and `ObjectSpawner.SpawnObject`
   - Construct a `Call` action using `SpawnSequence` and `StartSpawnSequence`
 - In the `Initialize` function
  - If `StartOnInit` is `true`
   - Call `StartSpawnSequence`

 # The ScreenWrap Component
- Add a NadaScript resource using the Component template template and name it `ScreenWrap`
 - [Add component](../zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) `ScreenWrap` to the Asteroid resource and Player resource archetypes

 ## ScreenWrapping

- The `ScreenWrap` component should look like this

```name=ScreenWrap, lang=csharp
class ScreenWrap : NadaComponent
{
  [Dependency] var Transform : Transform;
  
  [Property]
  var Camera : CogPath = CogPath();
  
  function Initialize(init : CogInitializer)
  {
    Zilch.Connect(this.Space, Events.LogicUpdate, this.OnLogicUpdate);
  }

  function OnLogicUpdate(event : UpdateEvent)
  {
    //Get the viewport component
    var viewport = this.Camera.Cog.CameraViewport;
    
    //prevent dividing by zero when the viewport resolution is (0,0) on game close
    if(Math.LengthSq(viewport.ViewportResolution) == 0.0)
      return;
      
    //get the normalized viewport
    var worldPos = this.Transform.WorldTranslation;
    var screenPos = viewport.WorldToScreen(worldPos);
    var viewportPos = viewport.ScreenToViewport(screenPos);
    var normalizedViewportPos = viewportPos / viewport.ViewportResolution;
    
    //screen wrap in normalized viewport space
    if(normalizedViewportPos.X > 1.0)
      normalizedViewportPos.X = 0.0;
    else if(normalizedViewportPos.X < 0.0)
      normalizedViewportPos.X = 1.0;
    
    if(normalizedViewportPos.Y > 1.0)
      normalizedViewportPos.Y = 0.0;
    else if(normalizedViewportPos.Y < 0.0)
      normalizedViewportPos.Y = 1.0;
    
    //convert the wrapped viewport position to world space
    viewportPos = normalizedViewportPos * viewport.ViewportResolution;
    screenPos = viewport.ViewportToScreen(viewportPos);
    worldPos = viewport.ScreenToWorldZPlane(screenPos, worldPos.Z);
    
    //set the object's position
    this.Transform.WorldTranslation = worldPos;
  }
}
```

- Drag and drop an instance of the Asteroid Asteroid resource and Player resource in the level
- Under ObjectSpawner
 - Set the `Camera` CogPath property to reference the Gamecamera object



![Asteroids](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/94409.zip)


At this point you should have a small ship navigating the screen, shooting, screenwrapping, and destroying asteroids. 

 
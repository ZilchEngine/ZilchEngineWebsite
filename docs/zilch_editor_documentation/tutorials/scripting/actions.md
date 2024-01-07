Actions are a handy way to animate properties with just a few lines of code. They can also be a way to call a function or dispatch an event after a delay. You can make actions happen in a paticular order, all at the same time, or some combination of the two. Let's take a look.


 #  Learning Objectives


- Property Actions
- Delay Actions
- Call Actions
- ActionSequences
- ActionGroups
- Looped Actions


 #  Level Setup


- [Create a New 2D Project](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/launchernewproject.md)

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `SpriteFader`


- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : GameCamera object
- In the `Properties Window`
 - Under [Camera](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/camera.md)
  - Set Size  to `5`
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#createsprite)
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Sprite object
- In the `Properties Window`
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : [Area](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/area.md)
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `SpriteFader`

 # What Are Actions
Often in games we find that we wish to smoothly transition a property from its existing value to another target value. This is often done by calculating interpolated values on logic update between an the existing value and the target value using a function such as [Math.Lerp](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/math.md#lerp-zilch-engine-documen). While there are times when it is advantageous to perform these operations in an update function it is more common to want to begin an interpolation operation and have it finish on its own. Actions can do this and more and act as a generic structure to organize in game *actions* that need to occur in sequence or parrallel.


 # Property Actions
The first and most common action type is a Property Action which allows us to interpolate a property from its current value to a target value, over a specific duration, at a rate defined by an easing function. We can break down the construction of a property action parameter by parameter.

```name=Example Property Action, lang=csharp
Actions.Property(this.Owner.Actions,
                 @this.Area.Size,
                 this.TargetSize,
                 this.Duration,
                 Ease.Linear);
```

| Action Property Parameters | | |
| **Example Value** | **Paremeter Type** |**Description** |
| `this.Owner.Actions` | [ActionSet](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/actionset.md) | The ActionSet which will update this action |
|`@this.Area.Size` |[ PropertyDelegate](https://github.com/ZilchEngine/ZilchDocs/blob/master//zilch_editor_documentation/zilchmanual/nada_in_zero/property_delegates.md) | Delegate of the property to be modified by the action |
| `this.TargetValue` | Property type of the [ PropertyDelegate](https://github.com/ZilchEngine/ZilchDocs/blob/master//zilch_editor_documentation/zilchmanual/nada_in_zero/property_delegates.md) passed into the previous parameter (**i.e.** [Real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md) in this example) | Value to which the action will interpolate the given property |
| `this.Duration` | [Real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md) | The duration over which the action will be completed |
| `Ease.Linear` | [Ease](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#ease) | The [Ease](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#ease) function used to calculate the rate of interpolation |

 ## Using a Property Action
Now that we've covered the basics of what a property action is let's try using one:
- Update the `SpriteFader` script:
``` lang=csharp, name=SpriteFader 
class SpriteFader : NadaComponent
{
  [Dependency] var Sprite : Sprite;
  [Dependency] var Area : Area;
  
  //Target scale to interpolate towards  
  [Property]
  var TargetSize : Real2 = Real2(2, 2);
  
  //Duration of the interpolation
  [Property]
  var Duration : Real = 1.0;
  
  function Initialize(init : CogInitializer)
  {
    //Call the animate function
    this.Animate();
  }
  
  //Interpolate the object's scale to a target value over a duration
  function Animate()
  {
    Actions.Property(this.Owner.Actions,
                     @this.Area.Size,
                     this.TargetSize,
                     this.Duration,
                     Ease.Linear);
  }
}
```
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![ScaleOnly](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/93871.gif)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

Here you can see the property action interpolating the title scale over the given period of one second.

 # Action Sequences
You may already be wondering how to chain actions together, well this is the purpose of an [ActionSequence](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/actionsequence.md).

- Add the following property to `SpriteFader`:
```name=Color, lang=csharp
  [Property]
  var TargetColor : Real4 = Real4(1,0,0,1);
```
- Update the `Animate` function in `SpriteFader` script:
``` lang=csharp, name=SpriteFader Action Sequence
  function Animate()
  {
    //create a sequence driven by the object
    var actionSequence = Actions.Sequence(this.Owner.Actions);
    //put the scaling property action first in the sequence
    Actions.Property(actionSequence,
                     @this.Area.Size,
                     this.TargetSize,
                     this.Duration,
                     Ease.Linear);
    //put the color interpolation property action second in the sequence
    Actions.Property(actionSequence,
                     @this.Sprite.VertexColor,
                     this.TargetColor,
                     this.Duration,
                     Ease.Linear);
  }
```

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![ScaleThenColor](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/93873.gif)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

Here we can see sequences allow up to play actions in a linear order. This is very helpful, but what if we want to make these actions happen at the same time?

 # Action Groups
Similiar to how an [ActionSequence](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/actionsequence.md) will let us perform actions in sequence an [ActionGroup](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/actiongroup.md) will let us perform actions in parallel (at the same time).

- Update the `Animate` function in `SpriteFader` script:
``` lang=csharp, name=SpriteFader Action Group
  function Animate()
  {
    //Create a group driven by the object
    var actionGroup = Actions.Group(this.Owner.Actions);
    //Put the scaling property  in the group
    Actions.Property(actionGroup,
                     @this.Area.Size,
                     this.TargetSize,
                     this.Duration,
                     Ease.Linear);
    //Put the color interpolation property action the group
    Actions.Property(actionGroup,
                     @this.Sprite.VertexColor,
                     this.TargetColor,
                     this.Duration,
                     Ease.Linear);
  }
```
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![ScaleAndColor](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/93875.gif)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

Now that the property actions are in a `group` instead of in a `sequence` they happen at the same time.

 # Combining Sequences and Groups
So far we have seen sequences and groups working seperately but what if we wanted to combine them. That would mean we could make sequences of grouped actions, or groups of sequenced actions. We can use the `SpriteFader` component to test this.

- Add the following variables to `SpriteFader`:
```name=Original Value Variables, lang=csharp
  var OriginalSize : Real2;
  
  var OriginalColor : Real4;
```

- Update the `Initialize` function in `SpriteFader`:
```name=SpriteFader.Initialize(), lang=csharp
  function Initialize(init : CogInitializer)
  {
    //Capture original values
    this.OriginalSize = this.Area.Size;
    this.OriginalColor = this.Sprite.VertexColor;
    
    //Call the animate function
    this.Animate();
  }
```

- Update the `Animate` function in `SpriteFader`:
```name=SpriteFader Grouped Sequences, lang=csharp
  function Animate()
  {
    //Create a group driven by the object
    var actionGroup = Actions.Group(this.Owner.Actions);
    //Create the sequence to the text up and down
    var scaleSequence = Actions.Sequence(actionGroup);
    //Put the scale up property action in the sequence
    Actions.Property(scaleSequence,
                     @this.Area.Size,
                     this.TargetSize,
                     this.Duration,
                     Ease.Linear);
    //Put the scale down property action in the sequence
    Actions.Property(scaleSequence,
                     @this.Area.Size,
                     this.OriginalSize,
                     this.Duration,
                     Ease.Linear);
    
    //Create the sequence to interpolate
    var colorSequence = Actions.Sequence(actionGroup);
    //Put the interpolate to black property action in the color sequence
    Actions.Property(colorSequence,
                     @this.Sprite.VertexColor,
                     this.TargetColor,
                     this.Duration,
                     Ease.Linear);
    //Put the interpolate to white property action in the color sequence
    Actions.Property(colorSequence,
                     @this.Sprite.VertexColor,
                     this.OriginalColor,
                     this.Duration,
                     Ease.Linear);
  }
```

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![GroupedSequences](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/93877.gif)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

It should be noted that `this.Owner.Actions` is an [ActionGroup](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/actiongroup.md) so in this simple case we could have just passed it to the constructor for the action sequences. We could also invert the group and sequence nesting to achieve the same affect from a different approach.

- Update the `Animate` function in `SpriteFader`:
```name=SpriteFader Sequenced Groups, lang=csharp
  function Animate()
  {
    //Create a group driven by the object
    var actionSequence = Actions.Sequence(this.Owner.Actions);
    //Create the group to scale up and black out the text
    var scaleUpGroup = Actions.Group(actionSequence);
    //Put the scaling property  in the group
    Actions.Property(scaleUpGroup,
                     @this.Area.Size,
                     this.TargetSize,
                     this.Duration,
                     Ease.Linear);
    //Put the color interpolation property action the group
    Actions.Property(scaleUpGroup,
                     @this.Sprite.VertexColor,
                     this.TargetColor,
                     this.Duration,
                     Ease.Linear);
    
    //Create the group to scale down and white out the text
    var scaleDownGroup = Actions.Group(actionSequence);
    Actions.Property(scaleDownGroup,
                     @this.Area.Size,
                     this.OriginalSize,
                     this.Duration,
                     Ease.Linear);
    //Put the color interpolation property action the group
    Actions.Property(scaleDownGroup,
                     @this.Sprite.VertexColor,
                     this.OriginalColor,
                     this.Duration,
                     Ease.Linear);
  }
```

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![SequencedGroups](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/93879.gif)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

Now we can see both property actions in the `scaleUpGroup` complete and then the two actions in the `scaleDownGroup` run. 

 # Call Actions
Another type of action is the call option. This allows you to put calls to functions in your sequences or groups. Test this out by printing at the beginning and end of the title animation sequences.

- Add the following `Print` function to `SpriteFader`:
```name=Print
  function Print(str : String)
  {
    Console.WriteLine(str);
  }
```

- Update the `Animate` function in `SpriteFader`:
```name=SpriteFader with printing, lang=csharp
  function Animate()
  {
    //Create a group driven by the object
    var actionSequence = Actions.Sequence(this.Owner.Actions);
    Actions.Call(actionSequence, this.Print, "Animation sequence started");
    
    //Create the group to scale up and black out the text
    var scaleUpGroup = Actions.Group(actionSequence);
    //Put the scaling property  in the group
    Actions.Property(scaleUpGroup,
                     @this.Area.Size,
                     this.TargetSize,
                     this.Duration,
                     Ease.Linear);
    //Put the color interpolation property action the group
    Actions.Property(scaleUpGroup,
                     @this.Sprite.VertexColor,
                     this.TargetColor,
                     this.Duration,
                     Ease.Linear);
    
    //Create the group to scale down and white out the text
    var scaleDownGroup = Actions.Group(actionSequence);
    Actions.Property(scaleDownGroup,
                     @this.Area.Size,
                     this.OriginalSize,
                     this.Duration,
                     Ease.Linear);
    //Put the color interpolation property action the group
    Actions.Property(scaleDownGroup,
                     @this.Sprite.VertexColor,
                     this.OriginalColor,
                     this.Duration,
                     Ease.Linear);
    
    Actions.Call(actionSequence, this.Print, "Animation sequence complete");
  }
```

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![SequencedGroupsWithPrint](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/93881.gif)


*`SpriteFader` scaling up and changing the color of the menu title at the same time using a group in a sequence then reversing the actions with another group. The animation is followed by the following console output*


```name=Console Output
Animation sequence started
Animation sequence complete
```

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

Now you can see the print function executed at the beginning and end of the sequence. This can be very helpful with debugging the behaviors of actions but it also has a slightly more complex application.

(NOTE)**Call Action Function Parameters**: `Action.Call` is overloaded to take multiple parameters for the function passed to it. As seen above you pass the values that should be passed to the given function as parameters to the call action constructor itself.

 ## Action Loops

- Add the following property to `SpriteFader`:
```name=Action Sequence Storage, lang=csharp
  var LoopedSequence : ActionSet;
```

- Update the `Animate` function in `SpriteFader`:
```name=SpriteFader with printing, lang=csharp
  function Animate()
  {
    if(this.LoopedSequence != null)
      this.LoopedSequence.Cancel();
    
    //Create a seqeunce driven by the object
    this.LoopedSequence = Actions.Sequence(this.Owner.Actions);
    Actions.Call(this.LoopedSequence, this.Print, "Animation sequence started");
    
    //Create the group to scale up and black out the text
    var scaleUpGroup = Actions.Group(this.LoopedSequence);
    //Put the scaling property  in the group
    Actions.Property(scaleUpGroup,
                     @this.Area.Size,
                     this.TargetSize,
                     this.Duration,
                     Ease.Linear);
    //Put the color interpolation property action the group
    Actions.Property(scaleUpGroup,
                     @this.Sprite.VertexColor,
                     this.TargetColor,
                     this.Duration,
                     Ease.Linear);
    
    //Create the group to scale down and white out the text
    var scaleDownGroup = Actions.Group(this.LoopedSequence);
    Actions.Property(scaleDownGroup,
                     @this.Area.Size,
                     this.OriginalSize,
                     this.Duration,
                     Ease.Linear);
    //Put the color interpolation property action the group
    Actions.Property(scaleDownGroup,
                     @this.Sprite.VertexColor,
                     this.OriginalColor,
                     this.Duration,
                     Ease.Linear);
    
    //Call animate at the end of the sequence to loop
    Actions.Call(this.LoopedSequence, this.Print, "Animation sequence complete");
    Actions.Call(this.LoopedSequence, this.Animate);
  }
```
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)




![Looped](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/93883.gif)


*`SpriteFader` scaling up and changing the color of the menu title at the same time using a group in a sequence then reversing the actions with another group, then looping the sequence*


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

Now we can see the action sequence call the function that originally set it up. This create a loop in the sequence of actions which will repeat. You should also notice that we started storing the action sequence in a member variable of `SpriteFader` instead of a local variable. This does not change the behavior of the action sequence, but it does allow us to examine, pause, and cancel the sequence while it is running. This usually good practice for all action sets. We actually already introduced a small example of how one may use an [ ActionSet](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/actionset.md) member variable when we introduced these two lines at the top of `animate`.

```name=Checking Looped Sequence for duplicate, lang=csharp
  if(this.LoopedSequence != null)
      this.LoopedSequence.Cancel();
```

By checking if `this.LoopedSequence` is not `null` we can determine if there is already a sequence in existence intended to animate the sprite. If the `Animate` function were to be called elsewhere without this check it could result in multiple sequence performing the same scaling and color interpolation operations on the same object independently and simultainiously. This can result in so very undesirable bugs where actions overlap each other in unintended ways. By cancelling any existing `LoopedSequence` before we start another we can avoid this issue almost entirely.

 # Delay Actions
Delay actions allow the insertion of a time based delay in an action sequence. When put in a group they can prevent the group completing but will not keep other actions in the group from running.

- Update the `Animate` function in `SpriteFader`:
```name=SpriteFader with printing, lang=csharp
  function Animate()
  {
    if(this.LoopedSequence != null)
      this.LoopedSequence.Cancel();
    
    //Create a group driven by the object
    this.LoopedSequence = Actions.Sequence(this.Owner.Actions);
    Actions.Call(this.LoopedSequence, this.Print, "Animation sequence started");
    
    //Create the group to scale up and black out the text
    var scaleUpGroup = Actions.Group(this.LoopedSequence);
    //Put the scaling property  in the group
    Actions.Property(scaleUpGroup,
                     @this.Area.Size,
                     this.TargetSize,
                     this.Duration,
                     Ease.Linear);
    //Put the color interpolation property action the group
    Actions.Property(scaleUpGroup,
                     @this.Sprite.VertexColor,
                     this.TargetColor,
                     this.Duration,
                     Ease.Linear);
    
    //Create the group to scale down and white out the text
    var scaleDownGroup = Actions.Group(this.LoopedSequence);
    Actions.Property(scaleDownGroup,
                     @this.Area.Size,
                     this.OriginalSize,
                     this.Duration,
                     Ease.Linear);
    //Put the color interpolation property action the group
    Actions.Property(scaleDownGroup,
                     @this.Sprite.VertexColor,
                     this.OriginalColor,
                     this.Duration,
                     Ease.Linear);
    
    Actions.Call(this.LoopedSequence, this.Print, "Animation sequence complete");
    //Delay the animation loop
    Actions.Delay(this.LoopedSequence, this.Duration);
    Actions.Call(this.LoopedSequence, this.Print, "Animation loop delay complete");
    Actions.Call(this.LoopedSequence, this.Animate);
  }
```
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)




![LoopedDelayed](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/93885.gif)


*`SpriteFader` scaling up and changing the color of the menu title at the same time using a group in a sequence then reversing the actions with another group, then looping the sequence after a short delay*


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

Now we have the title animating in a loop with a short delay in the sequence before the next itteration of the loop.

 # Event Actions
The final action type is the event action. This allows you to instantiate an even object as if you were about to dispatch it, but instead it pass it to the action to be dispatched later.


- Add the following in the `SpriteFader` class within `SpriteFader`:
```name=Event Registration, lang=csharp
  sends SpriteFaded : NadaEvent;
```

- Update the `Initialize` function in `SpriteFader`:
```name=SpriteFader with event actions, lang=csharp
  function Initialize(init : CogInitializer)
  {
    //Capture original values
    this.OriginalSize = this.Area.Size;
    this.OriginalColor = this.Sprite.VertexColor;
    
    Zilch.Connect(this.Space, Events.SpriteFaded, this.OnSpriteFaded);
    
    //Call the animate function
    this.Animate();
  }
```

- Add the following function to `SpriteFader`:
```name=Event Response Function, lang=csharp
  function OnSpriteFaded(event : NadaEvent)
  {
    Console.WriteLine("Sprite Faded");
  }
```

- Update the `Initialize` function in `SpriteFader`:
```name=Animate With Event Action, lang=csharp
  function Animate()
  {
    if(this.LoopedSequence != null)
      this.LoopedSequence.Cancel();
    
    //Create a group driven by the object
    this.LoopedSequence = Actions.Sequence(this.Owner.Actions);
    Actions.Call(this.LoopedSequence, this.Print, "Animation sequence started");
    
    //Create the group to scale up and black out the text
    var scaleUpGroup = Actions.Group(this.LoopedSequence);
    //Put the scaling property  in the group
    Actions.Property(scaleUpGroup,
                     @this.Area.Size,
                     this.TargetSize,
                     this.Duration,
                     Ease.Linear);
    //Put the color interpolation property action the group
    Actions.Property(scaleUpGroup,
                     @this.Sprite.VertexColor,
                     this.TargetColor,
                     this.Duration,
                     Ease.Linear);
    
    //Create the group to scale down and white out the text
    var scaleDownGroup = Actions.Group(this.LoopedSequence);
    Actions.Property(scaleDownGroup,
                     @this.Area.Size,
                     this.OriginalSize,
                     this.Duration,
                     Ease.Linear);
    //Put the color interpolation property action the group
    Actions.Property(scaleDownGroup,
                     @this.Sprite.VertexColor,
                     this.OriginalColor,
                     this.Duration,
                     Ease.Linear);
    
    //Delay the animation loop
    Actions.Delay(this.LoopedSequence, this.Duration);
    Actions.Event(this.LoopedSequence, this.Space, Events.SpriteFaded, NadaEvent());
    Actions.Call(this.LoopedSequence, this.Animate);
  }
```
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)




![LoopedDelayedEvents](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/93888.gif)


*`SpriteFader` scaling up and changing the color of the menu title at the same time using a group in a sequence then reversing the actions with another group, then looping the sequence after a short delay*


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)


 # Related Materials

 ## Manual
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md)
- [ PropertyDelegate](https://github.com/ZilchEngine/ZilchDocs/blob/master//zilch_editor_documentation/zilchmanual/nada_in_zero/property_delegates.md)

 ## Reference
 ### Classes
- [action](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/action.md)
- [actions](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/actions.md)
- [actiondelay](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/actiondelay.md)
- [actiongroup](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/actiongroup.md)
- [actionsequence](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/actionsequence.md)
- [actionset](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/actionset.md)
- [Ease](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#ease)

 ### Nada Base Types
- [Real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)
- [Real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)
- [Math.Lerp](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/math.md#lerp-zilch-engine-documen)

 ### Commands
- [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
- [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

 ## Tasks
- T782 

 
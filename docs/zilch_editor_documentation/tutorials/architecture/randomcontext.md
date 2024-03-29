[RandomContext](../../../code_reference/class_reference/randomcontext.md) is a component that contains methods for pseudo-random number generation.


 #  Learning Objectives


- Understanding random number generators
- Die roll simulation
- Using random seeds
- Random distribution


 #  Level Setup


- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [New Project](../../../code_reference/command_reference.md#newproject)
 - Create a new project using the {nav icon=clone, name=Empty 2D Project} template
- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [CreateTransform](../../../code_reference/command_reference.md#createtransform)
- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [Add Resource](../../zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `NumberGenerator`
- [Select](../../zilchmanual/editor/editorcommands/selectobject.md) : Transform object
- In the `Properties Window`
 - [Add Component](../../zilchmanual/editor/addremovecomponent.md) : [RandomContext](../../../code_reference/class_reference/randomcontext.md)
 - [Add Component](../../zilchmanual/editor/addremovecomponent.md) : `NumberGenerator`


 #  RandomContext


RandomContext is a component for creating unique scenarios, such as when a random number of enemies are created, or a random amount of gold is given to a player.


 #  Using Int


[Int](../../../code_reference/class_reference/randomcontext.md#int-zilch-engine-document) is a function that returns a pseudo-random number between `0` and [MaxInt](../../../code_reference/class_reference/randomcontext.md#maxint-zilch-engine-docum).

- In the `NumberGenerator` script
 - Update the `NumberGenerator` class to the following:
```TS:"NumberGenerator Script"
class RandomGenerator : NadaComponent
{
  [Dependency] var RandomContext : RandomContext;

  function Initialize(init : CogInitializer)
  {
    var number = this.RandomContext.Int();
    Console.WriteLine("Random Number: `number`");
  }
}
```

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [Console](../../../code_reference/command_reference.md#console)
- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [PlayGame](../../../code_reference/command_reference.md#playgame)

```name=Console Output
---------------- Begin Game ----------------
Random Number: 26581
Level 'Level' was loaded.
Loaded level 0.00s
```

Notice how a random positive integer is returned.

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [StopGame](../../../code_reference/command_reference.md#stopgame)


 #  Using the Modulo Operator


[Modulo](../../zilchmanual/nada_in_zilch/operators_precedence_chart.md) is represented by the `%` operator. Using modulo returns the remainder when a number is divided by another number.


- In the `NumberGenerator` script
 - Update the `NumberGenerator` class to the following:

```TS:"NumberGenerator Script"
class RandomGenerator : NadaComponent
{
  [Dependency] var RandomContext : RandomContext;
    
  function Initialize(init : CogInitializer)
  {
    var number = this.RandomContext.Int();
    Console.WriteLine("Number: `number`");
    Console.WriteLine("Mod 10: \t`number % 10`");
    Console.WriteLine("Mod 100: \t`number % 100`");
    Console.WriteLine("Mod 1000: \t`number % 1000`");
    Console.WriteLine("Mod 10000: \t`number % 10000`");
  }
}
```

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [PlayGame](../../../code_reference/command_reference.md#playgame)

```name = Console Output
---------------- Begin Game ----------------
Number: 30796
Mod 10:   6
Mod 100:  96
Mod 1000:   796
Mod 10000:  796
Level 'Level' was loaded.
Loaded level 0.00s
```

Notice how the random integer given is then divided by various powers of 10 and the remainder is printed out. This is how a pseudo-random value can be constrained to a range starting at 0 and ending one before the applied value.

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [StopGame](../../../code_reference/command_reference.md#stopgame)


 #  Using Range


[Range](../../../code_reference/class_reference/randomcontext.md#range-zilch-engine-docume) is a function that returns a [Real](../../../code_reference/nada_base_types/real.md) number between the lower number given (inclusive) and the higher number (exclusive).

- In the `NumberGenerator` script
 - Update the `NumberGenerator` class to the following:

```TS:"NumberGenerator Script"
class NumberGenerator : NadaComponent
{
  [Dependency] var RandomContext : RandomContext;
  
  var EnemyCount : Integer;
  
  function Initialize(init : CogInitializer)
  {
    // This will pick a random number between 1 and 10
    var randomEnemyCount = this.RandomContext.Range(1, 11) as Integer;
    
    // Loop to create enemies based on the random counter
    for(var i= 0; i < randomEnemyCount; ++i)
    {
      Console.WriteLine("Spawned An Enemy");
      this.EnemyCount += 1;
    }
    
    // Display how many enemies were spawned
    Console.WriteLine("Spawned `this.EnemyCount` enemies");
  }
}
```

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [PlayGame](../../../code_reference/command_reference.md#playgame)

```name=Console Output
---------------- Begin Game ----------------
Spawned An Enemy
Spawned An Enemy
Spawned 2 enemies
Level 'Level' was loaded.
Loaded level 0.00s
```

Notice how the output displays a random number of enemies created each time you start the game. In this example, a pseudo-random number is found between `1` and `10`, but another scenario could include finding between `1` and `5` enemies, and then adding `5` to it. That way, the end result will be between `6` and `10`. However, this could just be accomplished by finding a Range value between `6` and `10`.

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [StopGame](../../../code_reference/command_reference.md#stopgame)


 #  Seeding


Rolling a six-sided die should generally result in a random value in the range `[1, 6]`. However, if that die is thrown under the same conditions every time, then theoretically the die should always result in the same value, removing randomness.

This is accomplished in code by setting a [Seed](../../../code_reference/class_reference/randomcontext.md#seed-zilch-engine-documen). All projects already have a seed pseudo-randomly assigned at run-time, but applying a custom seeded value ensures all further randomness can instead be predicted.

- In the `NumberGenerator` script
 - Update the `NumberGenerator` class to the following:

```TS:"NumberGenerator Script"
class NumberGenerator : NadaComponent
{
  [Dependency] var RandomContext : RandomContext;
  
  var EnemyCount : Integer;
  
  function Initialize(init : CogInitializer)
  {
    this.RandomContext.Seed = 54321;
    
    // Find four pseudo-random numbers and print to console.
    for(var i = 0; i < 4; ++i)
    {
      // This will pick a random number between 1 and 5
      var randomNumber = this.RandomContext.Range(1, 6) as Integer;
      
      // Display how many enemies were spawned
      Console.WriteLine("Number: `randomNumber`");
    }
  }
}
```

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [PlayGame](../../../code_reference/command_reference.md#playgame)

```name=Console Output
---------------- Begin Game ----------------
Number: 3
Number: 2
Number: 5
Number: 5
Level 'Level' was loaded.
Loaded level 0.00s
```

Notice the number sequence that is printed.

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [StopGame](../../../code_reference/command_reference.md#stopgame)
- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [PlayGame](../../../code_reference/command_reference.md#playgame)

```name=Console Output
---------------- Begin Game ----------------
Number: 3
Number: 2
Number: 5
Number: 5
Level 'Level' was loaded.
Loaded level 0.00s
```

Notice how the number sequence was exactly the same as the first time.

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [StopGame](../../../code_reference/command_reference.md#stopgame)
- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [PlayGame](../../../code_reference/command_reference.md#playgame)

```name=Console Output
---------------- Begin Game ----------------
Number: 3
Number: 2
Number: 5
Number: 5
Level 'Level' was loaded.
Loaded level 0.00s
```

Notice that once again the number sequence was exactly the same. Continue this process to your heart's content.

- [Command](../../zilchmanual/editor/editorcommands/commands.md) : [StopGame](../../../code_reference/command_reference.md#stopgame)

Due to how the seed was set to `54321`, the pattern was the same throughout. However, it was not the same number repeated each time. This is due to how RandomContent is still referred to for a unique value.

Seeding is important in many different video games to recreate previous experiences. Games that rely upon seeding for Procedural Generation to create a level or determine gameplay sometimes also inform the player the seed used, allowing them to input that seed later and replay the exact same scenario.


 #  Convenience Functions


 ##  Die Roll


[DieRoll](../../../code_reference/class_reference/randomcontext.md#dieroll) is a simple function that returns an integer between 1 and a specified number of sides. It is intended for novice users, as it functions the same as the [Range](../../../code_reference/class_reference/randomcontext.md#range) function, except that:
- The value returned is inclusive of the maximum value
- The lowest value possible is `1` instead of `0`
- The value returned is an [Integer](../../../code_reference/nada_base_types/integer.md) rather than a Real that must be [cast into an Integer](../../zilchmanual/nada_in_zilch/casting.md)


 ##  Coin Flip


[CoinFlip](../../../code_reference/class_reference/randomcontext.md#coinflip) is a simple function that returns `true` or `false`.


 #  Related Materials
 ##  Manual
- [commands](../../zilchmanual/editor/editorcommands/commands.md)
- [resourceadding](../../zilchmanual/editor/editorcommands/resourceadding.md)
- [selectobject](../../zilchmanual/editor/editorcommands/selectobject.md)
- [addremovecomponent](../../zilchmanual/editor/addremovecomponent.md)
- [nada_in_zilch](../../zilchmanual/nada_in_zilch.md)
- [operators_precedence_chart](../../zilchmanual/nada_in_zilch/operators_precedence_chart.md)
- [variables_and_data_types](../../zilchmanual/nada_in_zilch/variables_and_data_types.md)
- [casting](../../zilchmanual/nada_in_zilch/casting.md)

 ##  Reference
 ###  Commands
- [NewProject](../../../code_reference/command_reference.md#newproject)
- [CreateTransform](../../../code_reference/command_reference.md#createtransform)
- [Console](../../../code_reference/command_reference.md#console)
- [PlayGame](../../../code_reference/command_reference.md#playgame)
- [StopGame](../../../code_reference/command_reference.md#stopgame)

 ###  Classes
- [randomcontext](../../../code_reference/class_reference/randomcontext.md) 

 
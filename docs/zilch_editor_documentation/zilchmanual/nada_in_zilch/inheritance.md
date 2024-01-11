Inheritance allows a *child// [class](classes.md) to automatically receive all of the data and functionality defined within the //base* class.

```TS:Feline,
class Feline
{
  constructor() { }
}
```

```TS:Lion,
// A colon designates an identifier for a base class follows.
class Lion : Feline
{
  // a constructor is not necessary when one is inherited from the base class.  
}
```
```TS:Using Feline & Lion
var cat = new Feline();
var simba = new Lion(); // Instantiated from the inherited constructor
```

In the above example the variable `simba` can be instantiated as a `Lion` using the constructor from `Feline`.

 # The **base** Keyword
The **base** [keyword](keywords.md) is for use when defining an inherited class; it allows you to call the constructor of the base class being inherited from before running an explicitly defined constructor.

```TS:Animal,
class Animal
{
  var Legs : Integer = 4;
  
  constructor() { }
  constructor(legs : Integer)
  {
      this.Legs = legs;
  }

  function ToString() : String
  {
    var builder = new StringBuilder();
    builder.Write("Legs: ");
    builder.Write(this.Legs);
    return builder.ToString();
  }
}
```
The class animal defines a **non-default** constructor which takes a number of legs for the animal as a parameter.

```TS:Human,
class Human : Animal
{
  constructor() : base(2) { }
}
```
The class `Human` which inherits from `Animal` can use `Animal`'s constructor by using the `base` keyword. In this situation either the default or non-default constructor from `Animal` could be called using based. Which constructor is called is determined by the parameters passed to the `()` after the`base` keyword. Because `2` is passed to the `base` keyword the **non-default** constructor of `Animal` is called before any implementation within the defined **default** constructor of `Human`.

```TS:Using Animal & Human
var animal : Animal = new Animal();
Console.WriteLine(animal.ToString()); // Legs: 4

var jerry = new Human();
Console.WriteLine(jerry.ToString());  // Legs: 2
```
In this runtime example both `Animal` and `Human` are instantiated using their default constructor.

```TS:Console Output
---------------- Begin Game ---------------
Legs: 4
Legs: 2
```
As can be seen in the console output the `Human` **default** constructor calls the **non-default** constructor of `Animal` and passes it `2`.

 # Classes & Structs
Although Nada currently does not throw an error, erratic and unexpected behavior will result from having a class inherit from a struct and vice versa. **i.e.**

```TS:Incompatible Inheritance
// Mismatching the struct/class between parent and child
struct MyBaseStruct
{
  constructor()
  {
  }
}
class MyClass : MyBaseStruct
{
  constructor() : base()
  {
  }
}
```
```name=Console WriteLine
// Leads to issues such as the inability to cast to the base class type. 
var incompatible: MyClass = new MyClass();
Console.WriteLine(typeid(incompatible).Name);                 // MyClass
Console.WriteLine(typeid(incompatible as MyBaseStruct).Name); // This won't compile.
```

 # The Virtual Keyword

Virtual is used to give Base classes the ability to determine some functions as being able to be *overridden* by its derived classes. The new `Speak` function defined in `Animal` will serve as an example:

```TS:Applying Virtual to a Function
class Animal
{
  var Legs:Integer = 4;

  constructor() { }
  
  constructor(legs : Integer)
  {
    this.Legs = legs;
  }
  
  function ToString() : String
  {
    var builder = new StringBuilder();
    builder.Write("Legs: ");
    builder.Write(this.Legs);
    return builder.ToString();
  }
  
  [Virtual]
  function Speak() : String
  {
    return "...";
  }
}
```

By default, animals don't say anything, so a string that says `...` is returned. It is known that there are animals that do speak, so the `[Virtual]` attribute is added to the function to let other developers know that if a class is is **derived** from `Animal`, the functionality of `Speak` may be overridden.


```TS:Animal,
class Human : Animal
{
  constructor() : base(2) { }
  
  [Override]
  function Speak() : String
  {
    return "Hello";
  }
}
```
Humans do speak, so changeing the funcitonality of `Human.Speak` to say something other than `...` makes perfect sense. The `[Override]` attribute applied to `Speak` marks this implementation of the `Speak` function to replace `Animal.Speak` which is marked as `[Virtual]`.

This can also be extended to other classes like a Cat:

```TS:Cat,
class Cat : Animal
{
  // Cats have 4 legs, so let's update the constructor
  constructor() : base(4) { }
  
  [Override]
  function Speak() : String
  {
    return "Meow";
  }
}
```

Now, this is great in the fact that we can now do something like the following:

```TS:Using Overridden Functions
var animal = Animal();
Console.WriteLine(animal.Speak());

var human = Human();
Console.WriteLine(human.Speak());

var cat = Cat();
Console.WriteLine(cat.Speak());
```

```name=Console Output
...
Hello
Meow
```

The real magic of inheritance comes in the idea that a class of a **derived** class can be stored in a variable that matches the type of the **base** class.

```TS
var humanIsAnAnimal : Animal = Human();
Console.WriteLine(humanIsAnAnimal.Speak());
```

Even though the variable is of type Animal, the Human version of the function is called:

```name=Console Output
Hello
```

This is because whenever a virtual method is called, the run-time type of the object is checked for an **overriding member**. The overriding member in the most derived class will then be called, which might be the original function if the derived class(es) have not overridden it.

This can be quite useful with an array of Animals.

```TS:Array of Animals
var a : Animal = Animal();
var b : Human = Human();
var c : Animal = Human();
var d : Cat = Cat();

var array : Array[Animal] = Array[Animal](){a,b,c,d};

foreach (var animal in array)
{
  Console.WriteLine(animal.Speak());
}
```


```TS:Console Output
...
Hello
Hello
Meow
```

 # Calling Parent Functions

It's also possible to call the parent version of a function from a child class. In order to do this, the object must be cast to the base type and then use the non-virtual operator (~>) to call the base version:

```TS:Calling **base** Function from Derived
var d : Cat = Cat();
(d as Animal)~>Speak();
```
```TS:Console Output
...
```

 # Related Materials
 ## Manual
- [attributes](attributes.md) 

 
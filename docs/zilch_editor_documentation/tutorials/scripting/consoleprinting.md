This lesson covers the basics of using the Console Window and Debugging in [Nada](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/nada_in_zero.md).

 # Learning Objectives

- Reading and Writing to the `Console Window`
- Basics of print debugging
- Learn the basics of String manipulation

 # Level Setup

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ New Project](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#newproject)
 - Create a new project using the {nav icon=clone, name=Empty 2D Project} template
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/createobject.md)
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)
 - Create a NadaScript resource using the Component template template and name it `MyBehavior`
- [Select](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/selectobject.md) : Sprite object
- In the `Properties Window`
 - Rename it to `Square`
 - [Add Component](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/addremovecomponent.md) : `MyBehavior`

 # Console Window

The `Console Window` is where the engine and your game may print messages to help you keep track of the logic being performed. It serves as a very helpful tool in identifying when and where the game performs differently than intended. Let's examine it:

- With the Zilch Editor in focus
- Press  : ```

NOTE: ``` is right under `Esc`

By default, you'll notice the `Console Window` sliding up from the bottom; it will display information provided by the engine regarding loading of the project, [running the game](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/runthegame.md) and more.



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/81527.png)


 # Printing to Console

Displaying messages on the `Console Window` is not exclusive to the editor; users are also able to print messages to aid in keeping track of the logic performed by the game and verify that it is following intended behavior.

 - Add the following code to the Initialize scope of the MyBehavior resource NadaScript:

```lang=csharp, name=Console Printing
Console.WriteLine("Hello World!");
```

`Console.` - Accessing a globally visible [ Console](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/console.md) class.
`WriteLine()` - Invoking a function that lets us print to the console on a new line.
`"Hello World!"` - Literal string of characters that will be printed to the console.
`;` - Indicates that we're done with instructions on this line of code.

By adding this line of code we can see our message printed to the console when we [play the game](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/runthegame.md).

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/81552.png)


NOTE: Within Console, you'll also find the function `Write()` which behaves similarly but does not display the following message on a new line.

In addition to literals, we can also print variable values or even convert those values into string form to create more complex messages.

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

 # Printing Literals

 - Add the following lines to the Initialize function in the MyBehavior resource NadaScript.

```lang=csharp, name=Literal String Printing
Console.WriteLine("This is a String");
```
```lang=csharp, name=Literal Integer Printing
Console.WriteLine(3);
```
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/88674.png)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

 # Printing Variables

 - Replace the previous lines of code with the following:

```lang=csharp, name=External Variable Printing
Console.WriteLine(this.Owner.Transform.Translation);
```

```lang=csharp, name= Local Variable Printing
var lives : Integer = 3;

Console.WriteLine(lives);
```
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/88676.png)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

In this case, Zilch will convert the variable into a string and then print it to the console.

 # Printing Compound Statements

We can also get more informative messages by using compound console print statements:

 - Replace the previous lines of code with the following:

```lang=csharp, name=Compound Print Statements
var lives : Integer = 3;

Console.Write("Current value of lives: ");
Console.WriteLine(lives);
```
- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/88678.png)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

 # String Interpolation

We can simplify the code from the previous example by using String Interpolation:

 - Replace the previous lines of code with the following:

```lang=csharp, name=String Interpolation
var lives : Integer = 3;

Console.WriteLine("Current value of lives: `lives`");
```

- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/88678.png)


- [ Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

By putting a variable within grates ``` we indicate that we want to convert the variable's value to a string and print it at the specified location.

 # Debugging

One of the most common uses of console printing is to aid in finding problems with your code (commonly referred to debugging). While the use cases are countless, these are the most common ones:

- Identifying whether a variable has the intended value
- Notifying you when the code reaches an unintended state
- Assessing whether a function is getting invoked
- Verifying return values from functions

Verifying that your code behaves as intended is a critical part of programming and its importance can hardly be understated. Make sure to familiarize yourself and get plenty of practice applying these techniques.

 # Related Materials

 ## Manual
- [Components](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/architecture/components.md)
- [ Nada User Documentation](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/nada_in_zero.md)
- [ Functions](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/nada_in_zero/functions.md)
- [ Strings](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/nada_in_zero/strings.md)
- [running the game](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/runthegame.md)

 ## Reference
 ### Classes
- [Transform](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/transform.md)
- [Sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md)
- [NadaScript](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/nadascript.md)
- [ Console](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/console.md)
- [ Add Resource](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/resourceadding.md)

 ### Commands
- [ PlayGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#playgame)
- [ StopGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#stopgame)

 ##  Tutorials
- [CustomComponents](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/tutorials/scripting/customcomponents.md)
- [Variables](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/tutorials/scripting/variables.md)
- [Functions](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/tutorials/scripting/functions.md)
 

 
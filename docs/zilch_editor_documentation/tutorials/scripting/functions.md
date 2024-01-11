This lesson covers the basics of using Functions in [Nada](../../zilchmanual/nada_in_zilch.md).


 # Learning Objectives

- Defining & calling functions
- Function parameters and return types
- Calling functions from different components 

 # Level Setup

- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [ New Project](../../../code_reference/command_reference.md#newproject)
 - Create a new project using the {nav icon=clone, name=Empty 2D Project} template
- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [CreateSprite](../../../code_reference/command_reference.md#createsprite)
- [ Command](../../zilchmanual/editor/editorcommands/commands.md) : [Add Resource](../../../code_reference/command_reference.md#add)
 - Create a NadaScript resource using the Component template template and name it `MyBehavior`
- In the `Object Window`
 - [Select](../../zilchmanual/editor/editorcommands/selectobject.md) : Sprite object
- In the `Properties Window`
 - Rename Sprite object to `Square`
 - [Add Component](../../zilchmanual/editor/addremovecomponent.md) : `MyBehavior`

 # Custom Functions

Functions are a sequence of logic statements that take a set of input variables with the goal of performing some operation. Functions are one of two main constructs within a class�the other being variables.

 ## Declaration

Start declaring by typing `function` followed by a name and a pair parentheses:


```TS:Function Declaration
function Square()
```

 ## Parameters

An important feature of functions is their ability to take literals and variables as input, referred to as **parameters**. These parameters are passed into the function to supply the data needed to complete the intended operation. They are declared within the function's parentheses by giving each a parameter name, followed by a type (`ParamName` : `ParamType`).

```TS:Parameters
function Square( number : Real )
```

NOTE: Functions can have any number of parameters (including none), each separated by a comma. These scenarios will be covered later.

 ## Scope

Just like classes, functions have a defined scope within which all of its functionality is outlined. We denote the scope by adding a pair of curly braces.

```TS:Scope
function Square( number : Real )
{

}
```

 ## Return Value

Some functions may provide a final result that can be returned back to the scope where it was invoked. These are called Return Types and are declared after the function's parentheses by typing colon `:` followed by the type to be returned.

```TS:Return Value
function Square( number : Real ) : Real
{

}
```

NOTE: It is not necessary for a function to return anything, in such cases no return type needs to be specified.

 ## Body

The body contains all the logic to be performed when the function is invoked. If the function has a Return Type, it is required to include a `return` statement within our function.

```TS:Function Body
function Square( number : Real ) : Real
{
    return number * number;
}
```

 - Add the previous code block inside the `MyBehavior` class.

Your code should look like this:



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/67019.png)


 # Invoking Functions

Now that we have created a function, it can be invoked elsewhere in code whenever the computations it provides are required.

When invoking a function that exists within the same class you can simply type:

```TS:Invoking Functions Within the Same Class
this.Square(2.0);
```

Similar to accessing variables, when invoking an external function we must first reference the class to whom it belongs:

```TS:Invoking Functions from Other Classes
//Syntax used by an external code trying to invoke our function
this.Owner.MyBehavior.Square(2.0);
```

Inside the parentheses, we must then pass either a literal, a variable or an expression which evaluates to the required type of the parameter (as outlined by the function definition). If a function takes multiple parameters, they must each be passed to the function in order, separated by a comma.

 # Return Values

Once a function is invoked, all of the instructions outlined within its scope are invoked in sequence. Once a function reaches the end of its scope or a return statement, it will return control to the scope that invoked it along with the Return Value (if one was specified).

Example:

```TS:Return Values
var pi : Real = 3.1415926;

var piSquare : Real = this.Square(pi);

//Print values to the console
Console.WriteLine("Pi: `pi`");
Console.WriteLine("Pi Square: `piSquare`");
```

WARNING: Functions may use conditionals; however, when a Return Type is declared, all code paths within the function must lead to a return statement. It is common to have multiple return statements that return different values depending on the branching logic within the function.


![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/81514.png) Here, Nada gives us an error since we haven't specified a return value should the variable `DoMath` be false. A solution to this problem might be: ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/81627.png)



 # Related Materials

 ## Manual
- [Components](../../zilchmanual/architecture/components.md)
- [ Nada User Documentation](../../zilchmanual/nada_in_zilch.md)
- [ Functions](../../zilchmanual/nada_in_zilch/functions.md)
- [Create a New 2D Project](../../zilchmanual/editor/editorcommands/launchernewproject.md)

 ##  Tutorials
- [CustomComponents](customcomponents.md)

 ## Reference
 ### Classes
- [Transform](../../../code_reference/class_reference/transform.md)
- [Sprite](../../../code_reference/class_reference/sprite.md)
- [NadaScript](../../../code_reference/class_reference/nadascript.md)

 ### Commands
- [CreateSprite](../../../code_reference/command_reference.md#createsprite)
- [Add Resource](../../../code_reference/command_reference.md#add)
 

 
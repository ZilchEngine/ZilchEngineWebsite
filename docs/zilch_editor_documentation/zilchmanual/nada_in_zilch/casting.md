Fundamentally, casting is converting from one type to another.  As demonstrated in the code snippet below, a [Function](functions.md) that takes a grade and returns pass/fail can be thought of as a conversion from a [real](../../../code_reference/nada_base_types/real.md) to a [boolean](../../../code_reference/nada_base_types/boolean.md).
```TS:Conversion Function
function IsPassing(grade : Real) : Boolean
{
  if(grade >= 70)
    return true;
  else
    return false;
}
```

The logic of that particular conversion is defined as a function and intended for a specific situation, but *cast operations* are more general-case and defined by Nada.

 # Implicit and Explicit
There are two types of casting, implicit and explicit.  Implicit casting occurs during the assignment of a variable of one type, with a value of a *different* type.  Implicit casting is a mechanism that Nada uses when a [Variable](variables_and_data_types.md) of one type is set to data of another type.  Explicit casting is a mechanic used by the user with the `as` keyword.  Any cast that can happen implicitly can be done explicitly.

WARNING: Even with explicit casting, there are still *cast operations* that are invalid and will trigger compile-time exceptions.

```TS:Casting Implicitly and Explicitly
var myReal : Real = 1.0;
var myDoubleReal : DoubleReal = myReal; // implicit casting
var myInteger : Integer = myReal as Integer; // explicit casting
```
In the example above, `myDoubleReal` is being set to `myReal`, which invokes an implicit cast from [real](../../../code_reference/nada_base_types/real.md) to [doublereal](../../../code_reference/nada_base_types/doublereal.md).  When `myReal as Integer` is evaluated, explicit casting is invoked to convert a [real](../../../code_reference/nada_base_types/real.md) to an [integer](../../../code_reference/nada_base_types/integer.md).  The format for explicit casting is `<value> as <new type>`.

NOTE: Explicit casting should only be used when one is aware of all of the nuances of the cast.

 # Casting Between Numeric and Boolean Types
The following base data types are considerered Numeric and Boolean:
| [integer](../../../code_reference/nada_base_types/integer.md) |
| [doubleinteger](../../../code_reference/nada_base_types/doubleinteger.md) |
| [real](../../../code_reference/nada_base_types/real.md) |
| [doublereal](../../../code_reference/nada_base_types/doublereal.md) |
| [boolean](../../../code_reference/nada_base_types/boolean.md) |

All *cast operations* using only these types are valid, meaning either explicit or implicit.  The code snippit below demonstates implicit casting between numeric types.

```TS:Implicit Numeric Casts
var myInteger : Integer = 1;

var myDoubleInteger : DoubleInteger = myInteger;
var myReal : Real = myInteger;
var myDoubleReal1 : DoubleReal = myInteger;

var myDoubleReal2 : DoubleReal = myDoubleInteger;
var myDoubleReal3 : DoubleReal = myReal;
```
Notice that implicit casting is allowed when converting to a numeric set, from a smaller data size to a larger one.  The value of `myInteger` can be implicitly casted to a [doubleinteger](../../../code_reference/nada_base_types/doubleinteger.md), which holds twice the number of bits as an [integer](../../../code_reference/nada_base_types/integer.md).  The value of `myInteger` can also be implicitly casted to a [real](../../../code_reference/nada_base_types/real.md).  Real values can hold whole numbers and a decimal portion, whereas integers can only be whole numbers.

(NOTE)**From a Mathematics Perspective** The integer set is a subset of the real set.  For more information on mathematical sets, visit the [Wikipedia Set (Mathematics)](https://en.wikipedia.org/wiki/Set_(mathematics)) page.

 ## Truncation
When a real value is converted to an integer value explicitly, the value will be truncated.  This means the decimal part of the real value will be lost, and without rounding.

```TS:Implicit Numeric Casts
Console.WriteLine(1.1 as Integer);
Console.WriteLine(2.99 as Integer);
Console.WriteLine(-3.99 as Integer);
```
```name=Console Window
1
2
-3
```

 # Upcasting and Downcasting
When casting between classes related through [inheritance](inheritance.md), one class must be a base class of the other.

```TS:Classes with Inheritance
class A {}
class B : A {}
class C : B {}
```

The code snippet below uses the `Classes with Inheritance` snippet.
```TS:Upcasting and Downcasting
var a : A = A();
var b : B = B();
var c : C = C();

// implicit
var ba : A = b;
var ca : A = c;
var cb : B = c;

// explicit
var ab : B = a as B;
var ac : C = a as C;
var bc : C = b as C;
```
Notice how all the implicit casts involve converting from a derived class to a base class.  This is known as **upcasting**.  **Downcasting** involves taking a base class and casting it to a derived class, which must be done explicitly.  **Downcasting** is also a type of dynamic casting, which is validated at runtime.  Observe that the objects `a`, `b`, and `c` are all references being casted, and not values.  If a base class reference is downcasted to a derived class reference and the value referenced is of the base class type, then the cast failed at runtime.  A *failed dynamic cast* will result in the value `null`.  The code snippet below uses the `Classes with Inheritance` snippet.

```TS:Dynamic Casting
var a_ref_b : A = B(); // upcast invoked implicitly
var b_ref_a : B = A() as B; // downcast invoked explicitly
var b_ref_b : B = a_ref_b as B; // downcast invoked explicitly
Console.WriteLine(a_ref_b == null);
Console.WriteLine(b_ref_a == null);
Console.WriteLine(b_ref_b == null);
```
```name=Console Window
false
true
false
```
`a_ref_b` is a reference of type `A` to a value of type `B`, which uses an implicit **upcast**.  `b_ref_a` is a reference of type `B` to a value of type `A`, which uses an explicit **downcast**.  Notice how `b_ref_a` has the value `null` at runtime, the result of a //failed dynamic cast//.  On the other hand, `a_ref_b` is successfully cast since it has a value of type `B`.

 # Null Casts
The value `null` can be cast to any reference type implicitly.  The code snippet below uses the `Classes with Inheritance` snippet.

```TS:Null Casting
var a1 : A = null; // implicit cast
var a2 : A = null as A; // explicit cast (unnecessary)
```

NOTE: Interpreting `null` as an invalid state for object references is a common pattern in programming.

 # Any Casts
Any type can be cast implicitly to an [any](../../../code_reference/nada_base_types/any.md), and an [any](../../../code_reference/nada_base_types/any.md) value can be implicitly cast to any type.  The [any](../../../code_reference/nada_base_types/any.md) type is used as a generic reference to any instantiated class or struct.
```TS:Any Casting
var integerOne : any = 1;
var myInteger : Integer = integerOne; // any cast
var myReal : Real = integerOne; // runtime exception
```
Notice how the attempt to cast `integerOne`, which is an [any](../../../code_reference/nada_base_types/any.md), to a [real](../../../code_reference/nada_base_types/real.md) results in a runtime exception.  An [any](../../../code_reference/nada_base_types/any.md) must first be cast to the type of the value it holds, even before other implicit conversions.

 # Same Casts
Same casts are casts that convert a value of one type to the same type.  All same casts can be done implicitly and are unnecessary.
```TS:Same Casting
var myReal : Real = 1.0; // implicit same cast
var myInteger : Integer = 1 as Integer; // explicit same cast
```

 # Related Materials
 ## Manual
- [Function](functions.md)
- [Variable](variables_and_data_types.md)
- [inheritance](inheritance.md)

 ## Code Reference
- [integer](../../../code_reference/nada_base_types/integer.md)
- [doubleinteger](../../../code_reference/nada_base_types/doubleinteger.md)
- [real](../../../code_reference/nada_base_types/real.md)
- [doublereal](../../../code_reference/nada_base_types/doublereal.md)
- [boolean](../../../code_reference/nada_base_types/boolean.md)
- [any](../../../code_reference/nada_base_types/any.md) 

 
## Notes About C# Language

#### Where I am referencing:
https://msdn.microsoft.com/en-us/library/ms173104.aspx

### Notes

C# is a __strongly-typed language__. Every variable and constant has a type, as does every expression that evaluates to a value. Every method signature specifies a type for each input parameter and for the return value.

Class <--reference type

Struct <--value type

Enum <--value type


### Specifying Types in Variable Declarations
When you declare a variable or constant in a program, you must either specify its type or use the var keyword to let the compiler infer the type.

A typical C# program uses types from the class library as well as user-defined types that model the concepts that are specific to the program's problem domain.

#### The information stored in a type _can_ include the following:

• The storage space that a variable of the type requires.

• The maximum and minimum values that it can represent.

• The members (methods, fields, events, and so on) that it contains.

• The base type it inherits from.(typically all inherit from Object)

• The location where the memory for variables will be allocated at run time.

• The kinds of operations that are permitted.

### Type Safe
 Unlike Javascript where things can change type if manipulated by code. C# is considered TYPE SAFE which means If you declare a variable of type __int__, the compiler allows you to use the variable in addition and subtraction operations. If you try to perform those same operations on a variable of type __bool__, the compiler would generate an error. You cannot add True-False but you could do 4-3.


### Types
| Type  | Range  | Size| .Net Framework Type | Default Value|
| ---------- |:----------:| -----:| :----------: |:----------:| :-----:|
| int |-2,147,483,648 to 2,147,483,647| $Signed 32-bit integer | System.Int32| 0



float = value type.  float vs double. 32bit vs 64bit
maybe if you had an array of a billion items and you were looking to save space you might use float. otherwise, mostly used today is double.

string = reference type



### Reference Types
There are two kinds of types in C#: reference types and value types. Variables of reference types store references to their data (objects), while variables of value types directly contain their data. With reference types, two variables can reference the same object; therefore, operations on one variable can affect the object referenced by the other variable. With value types, each variable has its own copy of the data, and it is not possible for operations on one variable to affect the other (except in the case of ref and out parameter variables, see ref (C# Reference) and out parameter modifier (C# Reference)).

__The following keywords are used to declare reference types:__

• class

• interface

• delegate


__C# also provides the following built-in reference types:__

• dynamic

• object

• string

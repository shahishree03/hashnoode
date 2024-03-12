---
title: "Introduction to C sharp"
datePublished: Mon Jan 09 2023 16:49:44 GMT+0000 (Coordinated Universal Time)
cuid: clcp1hhw6000108mf3s0n2yuc
slug: introduction-to-c-sharp
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1673282086615/8a4f6136-a2c9-4aec-8d75-28e08826584b.png

---

### **WHAT IS C#?**

You pronounce C# as "C-Sharp."

It is a Microsoft-developed object-oriented programming language that utilizes [the.NET](http://the.NET) Framework.

C# is related to other widely used languages like C++ and Java and has origins in the C family.

In 2002, the initial version was made available. In November 2022, C# 11, the most recent version, was published.

Uses for C# include:

Mobile programs Using desktop programs Web-based programs Online services websites, video games, and database programmes.

**Why Use C#?**

1.\] It is one of the most popular programming languages in the world.

2.\] It is easy to learn and simple to use.

3.\] It has huge community support.

4.\] C# is an object-oriented language that gives a clear structure to programs and allows code to be reused, lowering development costs.

5.\] As C# is close to [C](https://www.w3schools.com/c/index.php), [C++](https://www.w3schools.com/cpp/default.asp) and [Java](https://www.w3schools.com/java/default.asp), it makes it easy for programmers to switch to C# or vice versa.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1673278994947/a073c24d-3850-4ee1-a04a-08180dac50eb.png align="center")

### **C# SYNTAX**

We created a C# file called Program.cs, and we used the following code to print "Hello World" to the screen:

```csharp
using System;

namespace HelloWorld
{
  class Program
  {
    static void Main(string[] args)
    {
      Console.WriteLine("Hello World!");    
    }
  }
}
```

line 1.\] The use of the System namespace allows us to use classes.

Line 2.\] It is left empty. White space is ignored in C#. The code is better understood when there are more lines, though.

Line 3.\] A namespace serves as a container for classes and other namespaces and is used to structure your code.

Line 4.\] A block of code has a beginning and an end indicated by curly brackets.

Line 5.\] A class is a container for data and operations that gives your application functionality. Every line of C# code that executes must be contained within a class. We gave the class in our example the name Program.

Line 6.\] Another thing that always appears in a C# program, is the `Main` method. Any code inside its curly brackets `{}` will be executed. You don't have to understand the keywords before and after Main. You will get to know them bit by bit while reading this tutorial.

Line 7.\] `Console` is a class of the `System` namespace, which has a `WriteLine()` methods that are used to output/print text. In our example, it will output "Hello World!".

**Note:** Every C# statement ends with a semicolon `;`.

**Note:** C# is case-sensitive: "MyClass" and "myclass" has a different meaning.

**Note:** Unlike Java, the name of the C# file does not have to match the class name, but they often do (for better organization). When saving the file, save it using a proper name and add ".cs" to the end of the filename. To run the example above on your computer, make sure that C# is properly installed.

### **C# Output**

To output values or print text in C#, you can use the `WriteLine()` method:

```csharp
Console.WriteLine("Hello World!");
```

You can add as many `WriteLine()` methods as you want. Note that it will add a new line for each method:

```csharp
Console.WriteLine("Hello World!");
Console.WriteLine("I am Learning C#");
Console.WriteLine("It is awesome!");
```

You can also output numbers, and perform mathematical calculations:

### The Write Method

There is also a `Write()` method, which is similar to `WriteLine()`.

The only difference is that it does not insert a new line at the end of the output:

```csharp
Console.Write("Hello World! ");
Console.Write("I will print on the same line.");
```

### C# Comments

Comments can be used to explain C# code, and to make it more readable. It can also be used to prevent execution when testing alternative code.

**Single-line Comments**

Single-line comments start with two forward slashes (`//`).

Any text between `//` and the end of the line is ignored by C# (will not be executed).

This example uses a single-line comment before a line of code:

```csharp
// This is a comment
Console.WriteLine("Hello World!");
```

This example uses a single-line comment at the end of a line of code:

```csharp
Console.WriteLine("Hello World!");  // This is a comment
```

**C# Multi-line Comments**

Multi-line comments start with `/*` and ends with `*/`.

Any text between `/*` and `*/` will be ignored by C#.

This example uses a multi-line comment (a comment block) to explain the code:

### C# Variables

Variables are containers for storing data values.

In C#, there are different types of variables (defined with different keywords), for example:

* `int` - stores integers (whole numbers), without decimals, such as 123 or -123
    
* `double` - stores floating point numbers, with decimals, such as 19.99 or -19.99
    
* `char` - stores single characters, such as 'a' or 'B'. Char values are surrounded by single quotes
    
* `string` - stores text, such as "Hello World". String values are surrounded by double quotes
    
* `bool` - stores values with two states: true or false
    

### Declaring (Creating) Variables

To create a variable, you must specify the type and assign it a value:

```java
type variableName = value;
```

Where *type* is a C# type (such as `int` or `string`), and *variableName* is the name of the variable (such as **x** or **name**). The **equal sign** is used to assign values to the variable.

To create a variable that should store text, look at the following example:

```csharp
string name = "Iliyan";
Console.WriteLine(name);
```

To create a variable that should store a number, look at the following example:

```csharp
int myNum = 33;
Console.WriteLine(myNum);
```

You can also declare a variable without assigning the value, and assign the value later:

```csharp
int myNum;
myNum = 33;
Console.WriteLine(myNum);
```

Note that if you assign a new value to an existing variable, it will overwrite the previous value:

```csharp
int myNum = 33;
myNum = 43; // myNum is now 43
Console.WriteLine(myNum);
```

**Other Types**

A demonstration of how to declare variables of other types:

```csharp
int myNum = 33;
double myDoubleNum = 5.99D;
char myLetter = 'I';
bool myBool = true;
string myText = "Hello";
```

### C# Data Types

As explained in the variables chapter, a variable in C# must be a specified data type:

```csharp
int myNum = 5;               // Integer (whole number)
double myDoubleNum = 5.99D;  // Floating point number
char myLetter = 'D';         // Character
bool myBool = true;          // Boolean
string myText = "Hello";     // String
```

A data type specifies the size and type of variable values.

It is important to use the correct data type for the corresponding variable; to avoid errors, to save time and memory, but it will also make your code more maintainable and readable.

**Integer Types**

**Int**

The `int` data type can store whole numbers from -2147483648 to 2147483647. In general, and in our tutorial, the `int` data type is the preferred data type when we create variables with a numeric value.

```csharp
int myNum = 100000;
Console.WriteLine(myNum);
```

**Long**

The `long` data type can store whole numbers from -9223372036854775808 to 9223372036854775807. This is used when `int` is not large enough to store the value. Note that you should end the value with an "L":

```csharp
long myNum = 33333330000;
Console.WriteLine(myNum);
```

[Try it Yourself »](https://www.w3schools.com/cs/trycs.php?filename=demo_type_long)

**Floating Point Types**

You should use a floating point type whenever you need a number with a decimal, such as 9.99 or 3.14515.

The `float` and `double` data types can store fractional numbers. Note that you should end the value with an "F" for floats and "D" for doubles:

```csharp
float myNum = 5.75F;
Console.WriteLine(myNum);
```

Double Example

```csharp
double myNum = 19.99D;
Console.WriteLine(myNum);
```

**Booleans**

A boolean data type is declared with the `bool` keyword and can only take the values `true` or `false`:

```csharp
bool isCSharpFun = true;
bool isFishTasty = false;
Console.WriteLine(isCSharpFun);   // Outputs True
Console.WriteLine(isFishTasty);   // Outputs False
```

**Characters**

The `char` data type is used to store a **single** character. The character must be surrounded by single quotes, like 'A' or 'c':

```csharp
char myGrade = 'B';
Console.WriteLine(myGrade);
```

**Strings**

The `string` data type is used to store a sequence of characters (text). String values must be surrounded by double quotes:

```csharp
string greeting = "Hello World";
Console.WriteLine(greeting);
```
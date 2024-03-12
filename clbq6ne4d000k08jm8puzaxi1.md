---
title: "Introduction to C++"
datePublished: Fri Dec 16 2022 07:22:21 GMT+0000 (Coordinated Universal Time)
cuid: clbq6ne4d000k08jm8puzaxi1
slug: introduction-to-c
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1671175273722/ogMaeS69I.png

---

**C++** is a [high-level](https://en.wikipedia.org/wiki/High-level_programming_language) [general-purpose programming language](https://en.wikipedia.org/wiki/General-purpose_programming_language) created by Danish computer scientist [Bjarne Stroustrup](https://en.wikipedia.org/wiki/Bjarne_Stroustrup) as an extension of the [C programming language](https://en.wikipedia.org/wiki/C_(programming_language)), or "C with [Classes](https://en.wikipedia.org/wiki/Class_(programming))". The language has expanded significantly over time, and modern C++ now has [object-oriented](https://en.wikipedia.org/wiki/Object-oriented_programming), [generic](https://en.wikipedia.org/wiki/Generic_programming), and [functional](https://en.wikipedia.org/wiki/Functional_programming) features in addition to facilities for [low-level](https://en.wikipedia.org/wiki/Low-level_programming_language) [memory](https://en.wikipedia.org/wiki/Memory_(computing)) manipulation.

**Why Use C++**

1.\] C++ is one of the world's most popular programming languages.

2.\] C++ can be found in today's operating systems, Graphical User Interfaces, and embedded systems.

3.\] C++ is an object-oriented programming language which gives a clear structure to programs and allows code to be reused, lowering development costs.

4.\] C++ is portable and can be used to develop applications that can be adapted to multiple platforms.

5.\] C++ is fun and easy to learn!

6.\] As C++ is close to [C](https://www.w3schools.com/c/index.php), [C#](https://www.w3schools.com/cs/index.php) and [Java](https://www.w3schools.com/java/default.asp), it makes it easy for programmers to switch to C++ or vice versa.

**C++ syntax**

`#include <iostream>   using namespace std;      int main()`

`{     cout << "Hello World!";     return 0;   }`

Example explained

Line 1: `#include <iostream>` is a **header file library** that lets us work with input and output objects, such as `cout` (used in line 5). Header files add functionality to C++ programs.

Line 2: `using namespace std` means that we can use names for objects and variables from the standard library.

Don't worry if you don't understand how `#include <iostream>` and `using namespace std` works. Just think of it as something that (almost) always appears in your program.

Line 3**:** A blank line. C++ ignores white space. But we use it to make the code more readable.

Line 4**:** Another thing that always appear in a C++ program, is `int main()`. This is called a **function**. Any code inside its curly brackets `{}` will be executed.

Line 5: `cout` (pronounced "see-out") is an **object** used together with the *insertion operator* (`<<`) to output/print text. In our example it will output "Hello World".

Note: Every C++ statement ends with a semicolon `;`.

Note: The body of `int main()` could also been written as:  
`int main () { cout << "Hello World! "; return 0; }`

Remember**:** The compiler ignores white spaces. However, multiple lines makes the code more readable.

Line 6**:** `return 0` ends the main function.

Line 7**:** Do not forget to add the closing curly bracket `}` to actually end the main function.

**C++ output**

The `cout` object, together with the `<<` operator, is used to output values/print text:

#include &lt;iostream&gt;  
using namespace std;  
  
`int main()`

`{     cout << "Hello World!";     return 0;   }`

You can add as many `cout` objects as you want. However, note that it does not insert a new line at the end of the output

**New Lines**

To insert a new line, you can use the `\n` character:

#include &lt;iostream&gt;  
using namespace std;  
`int main()`

`{     cout << "Hello World! \n";     cout << "I am learning C++";     return 0;   }`

Two `\n` characters after each other will create a blank line

Another way to insert a new line, is with the `endl` manipulator:

`#include <iostream>   using namespace std;      int main()`

`{     cout << "Hello World!" << endl;     cout << "I am learning C++";     return 0;   }`

**C++ Variables**

sVariables are containers for storing data values.

In C++, there are different **types** of variables (defined with different keywords), for example:

1.\] int - stores integers (whole numbers), without decimals, such as 123 or -123

2.\] double - stores floating point numbers, with decimals, such as 19.99 or -19.99

3.\] char - stores single characters, such as 'a' or 'B'. Char values are surrounded by single quotes

4.\] string - stores text, such as "Hello World". String values are surrounded by double quotes.

5.\] bool- stores values with two states: true or false

**Declaring (Creating) Variables**

To create a variable, specify the type and assign it a value:

**Syntax**

*type* *variableName* = *value*;

Where *type* is one of C++ types (such as `int`), and *variableName* is the name of the variable (such as **x** or **myName**). The **equal sign** is used to assign values to the variable.

To create a variable that should store a number, look at the following example:

Example

Create a variable called **myNum** of type `int` and assign it the value **15**:

`int myNum = 15;   cout << myNum;`

## Declare Many Variables

To declare more than one variable of the **same type**, use a comma-separated list:

### Example

int x = 5, y = 6, z = 50;  
cout &lt;&lt; x + y + z;  

**One Value to Multiple Variables**

You can also assign the **same value** to multiple variables in one line:

Example

int x, y, z;  
x = y = z = 50;  
cout &lt;&lt; x + y + z;

C++ Strings

Strings are used for storing text.

A `string` variable contains a collection of characters surrounded by double quotes:

Example

Create a variable of type `string` and assign it a value:

string greeting = "Hello";

To use strings, you must include an additional header file in the source code, the `<string>` library:

Example

`// Include the string library   #include <string>      // Create a string variable   string greeting = "Hello";`

## C++ Loops

Loops can execute a block of code as long as a specified condition is reached.

Loops are handy because they save time, reduce errors, and they make code more readable.

* * *

**C++ While Loop**

The `while` loop loops through a block of code as long as a specified condition is `true`:

**Syntax**

`while (condition)`

`{     // code block to be executed   }`  

In the example below, the code in the loop will run, over and over again, as long as a variable (`i`) is less than 5:

Example

`int i = 0;   while (i < 5) {     cout << i << "\n";     i++;   }`

**The Do/While Loop**

The `do/while` loop is a variant of the `while` loop. This loop will execute the code block once, before checking if the condition is true, then it will repeat the loop as long as the condition is true.

Syntax

`do {     // code block to be executed   }   while (condition);`  

The example below uses a `do/while` loop. The loop will always be executed at least once, even if the condition is false, because the code block is executed before the condition is tested:
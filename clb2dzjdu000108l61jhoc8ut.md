---
title: "C programming"
datePublished: Tue Nov 29 2022 15:41:17 GMT+0000 (Coordinated Universal Time)
cuid: clb2dzjdu000108l61jhoc8ut
slug: c-programming
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1669736062335/QKA6HFqop.png

---

**Introduction :-**  
Dennis Ritchie developed the general-purpose computer language C at Bell Laboratories in 1972. Despite being an ancient language, it is quite popular. Since the UNIX operating system was created using C, the two are closely related. C is commonly used on computer architectures that range from the largest supercomputers to the smallest microcontrollers and embedded systems.
With a static type system and support for structured programming, lexical variable scope, and recursion, C is an imperative procedural language. It was intended to be built, with minimum runtime assistance, to offer low-level memory access and language features that easily translate to machine instructions. Although the language has low-level capabilities, it was created to promote cross-platform development.

**Why learn C programming:-**  
1.) It is one of the most popular programming language in the world.  

2.) If you know C, you will have no problem learning other popular programming languages such as Java, Python, C++, etc, as the syntax is similar.  

3.) C is very fast, compared to other programming languages, like Java and Python.  

4.) C is very versatile; it can be used in both applications and technologies.  

**C SYNTAX: **

```
#include <stdio.h>

int main() {
  printf("Hello World!");
  return 0;
}
```
Lets understand each line of the given code,

 Line 1:]  #include <stdio.h> is a header file library that is already predefined and lets us work with input and output functions, such as printf() (used in line 4). Header files add functionality to C programs.

Line 2:] Another thing that always appear in a C program, is main(). This is called a function. Any code inside its curly brackets {} will be executed.
You can call n numbers of function but u need to first declare it.

Line 3:] printf() is a function used to output/print text to the screen. In our example it will output "Hello World".
Similarly ,scanf() is also used to take inputs from the user ,also the c programming is case sensitive so the printf and scanf must be of lowercase.

Line 4:] return 0 ends the main() function.

Line 5:] Do not forget to add the closing curly bracket } to actually end the main function.

**C output**  
You can use printf() function to print any statement whatever the requirements.You can use as many printf() functions as you want. However, note that it does not insert a new line at the end of the output:

for example : If u want to print your name and surname you can do it in following way-


```
#include<stdio.h>

int main()
{
 printf("Iliyan Momin");
 return 0;
}
``` 

**C new lines**
Everytime you use printf() function the new text wont be inserted in next line, to do so you must use  \n character in the printf() statement.
You can also output multiple lines with a single printf() function. However, be aware that this will make the code harder to read:

```
#include <stdio.h>

int main()
 {
  printf("Hello World!\n");
  printf("I am Iliyan Momin,");
  printf("Studying in KJSIEIT");
  return 0;
 }

//output:
Hello World!
I am Iliyan Momin,Studying in KJSIEIT
```
In the given code \n is used after first printf() and not used after Second printf() , hence the content of the third printf() is not inserted in next line.
Two \n characters after each other will create a blank line.

**Comments in C**  
Comments can be used to explain code, and to make it more readable. It can also be used to prevent execution when testing alternative code.

Comments can be singled-lined or multi-lined.

Single-line Comments
Single-line comments start with two forward slashes (//).
Any text between // and the end of the line is ignored by the compiler (will not be executed).

Multi-line comments start with /* and ends with */.
Any text between /* and */ will be ignored by the compiler

```
#include <stdio.h>

int main()
 {
  printf("Hello World!\n");
  printf("I am Iliyan Momin\n");
 //College I m studying in 
  printf("Studying in KJSIEIT");
  return 0;
 }
//output:
Hello World!
I am Iliyan Momin
Studying in KJSIEIT
```
While execution, the line which is comment out will be ignored by the compiler and will not be executed.


**C Variables :**
Variables are containers for storing data values.

In C, there are different types of variables (defined with different keywords), for example:

1.] int - stores integers (whole numbers), without decimals, such as 123 or -123  

2.] float - stores floating point numbers, with decimals, such as 19.99 or -19.99

3.] char - stores single characters, such as 'a' or 'B'. Char values are surrounded by single quotes.

Declaring (Creating) Variables
To create a variable, specify the type and assign it a value.

```
type variablename = value;
```
Where type is one of C types (such as int or float ), and variableName is the name of the variable (such as x or myName). The equal sign is used to assign a value to the variable.

So, to create a variable that should store a number, look at the following example:

**int per= 90;**
Note: If you assign a new value to an existing variable, it will overwrite the previous value:

Example
```
int per = 90;  // per is 90
per = 87;  // Now per is 87
```

**Data Types**
As explained in the Variables chapter, a variable in C must be a specified data type, and you must use a format specifier inside the printf() function to display it:

Example: 
```
// Create variables
int per = 90;                   // Integer (whole number)
float myper = 90.33;   // Floating point number
char grade = 'A';       // Character

// Print variables
printf("%d\n", per);
printf("%f\n", myper);
printf("%c\n", grade);
```
**C Operators**   
Operators are used to perform operations on variables and values.

In the example below, we use the + operator to add together two values:

Example
int myNum = 100 + 50;
Although the + operator is often used to add together two values, like in the example above, it can also be used to add together a variable and a value, or a variable and another variable:

Example
```
int sum1 = 100 + 50;        // 150 (100 + 50)
int sum2 = sum1 + 250;      // 400 (150 + 250)
int sum3 = sum2 + sum2;     // 800 (400 + 400)
```

C divides the operators into the following groups:

Arithmetic operators  
Assignment operators   
Comparison operators  
Logical operators   
Bitwise operators

**Different loop statements: ** 
1.] Do-while loop  
2.] for loop  
3.] while  

**C has the following conditional statements:**

1.] Use if to specify a block of code to be executed, if a specified condition is true

2.]Use else to specify a block of code to be executed, if the same condition is false

3.]Use else if to specify a new condition to test, if the first condition is false

4.]Use switch to specify many alternative blocks of code to be executed.

**The if Statement**

Use the if statement to specify a block of C code to be executed if a condition is true.Note that if is in lowercase letters. Uppercase letters (If or IF) will generate an error.

Syntax
```
if (condition) {
  // block of code to be executed if the condition is true
}
```
**The else Statement**   

Use the else statement to specify a block of code to be executed if the condition is false.

Syntax
```
if (condition)
 {
  // block of code to be executed if the condition is true
 }
 else 
 {
  // block of code to be executed if the condition is false
 }
```

**The else if Statement**

Use the else if statement to specify a new condition if the first condition is false.

Syntax
```
if (condition1) 
{
  // block of code to be executed if condition1 is true
} 
else if (condition2) 
{
  // block of code to be executed if the condition1 is false and condition2 is true
} 
else 
{
  // block of code to be executed if the condition1 is false and condition2 is false
}
```

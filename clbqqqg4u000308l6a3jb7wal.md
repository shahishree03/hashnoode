---
title: "Java and its interactive inputs"
datePublished: Fri Dec 16 2022 16:44:36 GMT+0000 (Coordinated Universal Time)
cuid: clbqqqg4u000308l6a3jb7wal
slug: java-and-its-interactive-inputs
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1671205759292/qtEmQxXZN.jpeg
tags: java

---

# History of Java:

Java Programming Language was first developed in 1990 by an Engineer at Sun Microsystems named James Gosling. He was not happily using the C++ programming language so he created a new language that he called “Oak”. The language was renamed “Java” in 1995 and was made freely available by Sun Microsystems.

### Let’s have a look at its features-

Object Oriented: In java, everything is an object. All the program codes and data reside in classes and objects.

Platform Independent: it is platform independent because it does not depend on any type of platform. The java compiled code (byte code) can run on all operating system that provides the environment i.e Java Virtual Machine (JVM) to run it

Simple and Secure: It is very easy to learn, and its syntax is simple, clean and easy to understand also java is secure because -No explicit pointer and Java Programs run inside a virtual machine sandbox. Java supports access modifiers to check memory access and ensures that no viruses enter an applet. Authentication techniques are based on public-key encryption.

Robust: It is robust as it is capable of handling runtime errors, supports automatic garbage collection and exception handling.

Multithreaded: With Java's multithreaded feature it is possible to write programs that can perform many tasks simultaneously. This design feature allows the developers to construct interactive applications that can run smoothly.

Performance: With the use of Just-In-Time compilers, Java enables high performance.

### Tools that are needed for Java Programming:

Operating System: Java works on windows and Linux operating systems as well.

JDK: JDK is a core package used in Java, along with the JVM i.e Java Virtual machine and the JRE  i.e Java Runtime Environment. 

Editors like notepad and any text editor like sublime text etc.

# Interactive inputs in Java

It is a computing system that allows the user to interact with a running program by giving it data or control directions through an input device such as a keyboard or a mouse**.**

There are three types of interactive inputs in a java-

*   Scanner class
    
*   Data InputStream class
    
*   BufferedReader class
    

### Scanner class:

Scanner is a class in java.util [package](http://package.It).It is used for obtaining the input of primitive types like int, double, etc. and strings. It is the simplest way to read input in a Java program. But it is not much efficient if you want an input method for scenarios where time is a constraint like in competitive programming.

Let's do a program using the scanner class:

```java
import java.util.Scanner;
public class ScanDemo
{
 public static void main(String[] args)
    { 
        Scanner sc = new Scanner(System.in);
        System.out.println('Enter the first number');
        Int a =sc.nextInt();
        System.out.println('Enter the second number');
        Int b =sc.nextInt();
        Int c = a+b;
        System.out.println('The result is:' +c);
        }
    }
```

Input:

```java
Enter the first number: 25
Enter the second number:  26
```

Output :

```java
The result is 51
```

Here, we first import the java package i.e java.util.

To create an object of the Scanner class, we use the predefined object System.in

To read numerical values of a certain data type ABC, the function to use is nextABC().

### Data inputStream class :

Data inputStream class is a class in java.io package.It is an application to read primitive data types from an underlying input stream in a machine-independent way.

We use a constructor DataInputStream(InputStream in) that creates a DataInputStream that uses the specified underlying InputStream.

There are some methods to read inputs such as readLine() to read lines of text , readChar() to read two input bytes and return a char value , readByte to read one input byte and return a byte value etc. and there are more methods.

Lets run a program-

```java
import java.io.*;
class DataInputStreamDemo {
    public static void main(String args[]){
  int a,b,c ;
  // Try block to check for exceptions
    try {
DataInputStream d = new DataInputStream((System.in));
System.out.println('Enter the value of A:'); 
String an = d.readLine();
System.out.println('Enter the value of B:'); 
String bn = d.readLine();
a = Integer.parseInt(an);
b= Integer.parseInt(bn);
c= a+b;
System.out.println('c=' +c);
}

Catch (IOException e)
{
    System.out.println('wrong input has given');
}
}
}
```

We used Integer.parseInt because

By default all arguments in java are strings. So to convert the string to an integer datatype we use ParseInt.

Input :

```java
Enter the value of A: 12

Enter the value of B : 13
```

Output :  
`c= 25`

### BufferedReader class:

The BufferedReader class of Java is used to read the stream of characters from the specified source (character-input stream). It is also under java.io package. t buffers the characters so that it can get the efficient reading of characters, arrays etc.

There are two types of constructors in bufferedReader class

BufferedReader(Reader reader) -This constructor creates a buffering character-input stream that works on a default-size input buffer.

BufferedReader(Reader reader, int size) - It uses the specified size for the input buffer for buffering the character-input stream.

Let's do an example-

```java
import java.io.*;
class additon{
public static void main(String args[] throws Exception)
{
int a , b, c;
BufferedReader b = new BufferedReader(new inputstreamreader System.in);
System.out.println('Enter the first number:');
a= Integer.parseInt(br.readLine());
System.out.println('Enter the second number:');
b= Integer.parseInt(br.readLine());
c= a+b;
System.out.println('sum' +c);
}
}
```

Input :

```java
Enter the first number= 23
Enter the second number= 31
```

 Output :

```java
Sum = 54
```

Here, we used java.io package to access the sub-packages inside the packages.

And here we stop our reading for today. Happy Learning.

Thank you for reading this blog.
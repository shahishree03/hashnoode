---
title: "Object-oriented Programming Concepts"
datePublished: Wed May 10 2023 14:13:15 GMT+0000 (Coordinated Universal Time)
cuid: clhhs6bxh000009l58rbibcag
slug: object-oriented-programming-concepts
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1683726635347/995dfe9a-a08c-4994-a0e6-5398ca4330b5.png
tags: java, oops, programmi

---

OOPs (Object-Oriented Programming) is a programming paradigm that emphasizes using objects and classes to organize and structure code. In OOPs, code is organized around objects, which are instances of classes, and classes are templates or blueprints for creating things. Oops, are based on encapsulating data and behaviour (methods) into a single unit (class) and provide a way to model real-world entities and their relationships.

OOPs offers several advantages over procedural programming, including better code organization and modularity, code reusability, and easier maintenance. The most important OOPs concepts are encapsulation, inheritance, polymorphism, and abstraction. These concepts form the foundation of OOPs and are used to model real-world systems, build software applications, and solve complex problems. OOPs are widely used in modern programming languages such as Java, C++, Python, and Ruby.

## **OOP's concepts:**

**Class:** A class is a blueprint or template for creating objects that define the properties and methods of the object. A class is a user-defined data type that encapsulates data and behavior (methods) into a single unit. It provides a way to organize and structure code and helps to create reusable code.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1683727156326/e980793e-68ae-4540-a36e-8bdc6fc8596d.jpeg align="center")

For example, consider a class called "Car" that defines the properties and methods of a car object. The class may have attributes like "make", "model", "color", "year", and methods like "start()", "accelerate()", "brake()", and "turn()". These attributes and methods define the state and behavior of a car object. When we create an instance of the "Car" class, we can set its attributes and call its methods to perform actions on the car object.

**Inheritance:** Inheritance is one of the fundamental concepts in OOPs (Object-Oriented Programming) that allows a class to inherit properties and methods from its parent class. It is a way to reuse code and build upon existing code, making it easier to manage and maintain large codebases.

Inheritance creates a relationship between a parent class (also called a base class or super class) and a child class (also called a derived class or subclass). The child class inherits all the properties and methods of its parent class, and can also add its properties and methods.The main advantage of inheritance is code reusability.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1683727787357/aa2bc51c-a157-49fa-a3db-5d954a34e1fe.png align="center")

**Polymorphism:** Allows objects to take on different forms depending on the context in which they are used. Polymorphism is achieved through two mechanisms: method overloading and method overriding.

Method overloading allows multiple methods in a class to have the same name but with different parameters. When a method is called, the compiler determines which version of the method to call based on the number, types, and order of the parameters passed to it.

Method overriding occurs when a child class provides its own implementation of a method that is already defined in its parent class. The child class must use the same method name, return type, and parameters as the parent class method, but can provide its own implementation.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1683727815523/7bbc2794-ff78-4c16-ab43-8be9af65b4be.png align="center")

**Abstraction:**

Abstraction involves hiding the complexity of a system by exposing only the essential details to the user, while hiding the implementation details.

In OOPs, abstraction is achieved through abstract classes and interfaces. An abstract class is a class that cannot be instantiated and is used as a base class for other classes. An abstract class can have both concrete and abstract methods, with the abstract methods being declared but not implemented. A class that inherits from an abstract class must implement all its abstract methods.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1683727873443/5ed0a0b4-e749-4465-b505-22d17cdb8697.png align="center")

**Encapsulation:** Encapsulation allows us to protect the internal state of an object from being directly accessed or modified by external code.

In OOPs, encapsulation is achieved through the use of access modifiers such as public, private, and protected. Public members of a class are accessible from any part of the program, while private members are only accessible within the class itself. Protected members are accessible within the class and its subclasses.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1683727959781/bddcdc69-a684-4ddb-87c2-9dccd198f24b.jpeg align="center")

Encapsulation allows us to maintain the integrity of an object's internal state by controlling how it is accessed and modified
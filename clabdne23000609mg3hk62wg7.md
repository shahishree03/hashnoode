---
title: "ES6 in Javascript"
datePublished: Thu Nov 10 2022 18:02:03 GMT+0000 (Coordinated Universal Time)
cuid: clabdne23000609mg3hk62wg7
slug: es6-in-javascript
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1668099797397/gZ7TnSbhC.jpeg

---

ES6 also known as** ECMAScript** is a JavaScript standard that allows the software to exchange and make use of information in web pages across different browsers.

Do you want to make your code more modern and systematic?
Use ECMAScript in Java, which allows the user to implement new syntax and awesome features.
It allows you to write less code and do more. ES6 introduces us to many great features like arrow functions, template strings, class destruction, Modules… and more.

Here are some syntax explanation with **code snippets** as well :

**1. CONST**

Const is a new keyword in ES6 for declaring variables. Const is more powerful than var.
This is best when targeting a selector, Once used the variable can’t be reassigned.When you want to target a single button for an event use const over var ,because 'var' is function or a variable that can be used before declaration.


```
var MyBtn=document.getElementById('mybtn');

//instead use const

const MyBtn=document.getElementById('mybtn');

``` 
In the above code, if you try to change the value it will return the error since you used const.


**2.Template Literals**
Template literals or template strings are very user friendly. We don’t have to use the plus (+) operator to concatenate strings, or when we want to use a variable inside a string.
This allows you to spend less amount of time on code, also a small error or mistake of syntax can lead to Error in your output.


```
//ES5 

function myFunc1(name,age)
{
  return 'Hi' + name + 'Your age is' + age + 'years old';
}
console.log(myFunc('Iliyan' , 19))

//output --> Hi Iliyan , Your age is 19 years old
``` 

instead use template literals 


```
//ES6

const myFunc=(name,age)
{
  return 'Hi ${name} , Your age is ${age} years old';
}
console.log(myFunc('Iliyan' , 19))

//output --> Hi Iliyan , Your age is 19 years old
``` 


**3. let **
let can be reassigned and take new value and creates a mutable variable.
let is the same as const in that both are blocked-scope. It means that the variable is only available within its scope.


```
let name="Iliyan";
     name="ILIYAN";
console.log(name)

//output --> ILIYAN 

``` 

**4. Array and object destructing**
Destruction makes the assignment of the values of an array or object to the new variable easier.


```
//ES5 SYNTAX
const contacts={
                  name : 'Iliyan',
                  familyname : 'Momin',
                  age : '19'
                }
let name=contacts.name;
let familyname=contacts.familyname;
let age=contacts.age;

console.log(name)
console.log(familyname)
console.log(age)

//output
//Iliyan
//Momin
//19
``` 
With ES5, we have to assign each value to each variable. With ES6, we just put our values within curly brackets to get any property of the object.


```
//ES6 SYNTAX
const contacts={
                  name : 'Iliyan',
                  familyname : 'Momin',
                  age : '19'
                }
let{name , familyname, age}=contacts

console.log(name)
console.log(familyname)
console.log(age)

//output
//Iliyan
//Momin
//19
``` 


Note: if you assign a variable that is not identical to the name of property, it will return undefined. For example, if the name of the property is name and we assign it to a username variable, it will return undefined.













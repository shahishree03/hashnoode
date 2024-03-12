---
title: "Hypertext Preprocessor [PHP]"
datePublished: Fri Dec 23 2022 06:25:46 GMT+0000 (Coordinated Universal Time)
cuid: clc04plns000308l783le1jyi
slug: hypertext-preprocessor-php
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1671776601109/77d9add8-a5c6-4cd9-b6b6-10cd31a3984c.png

---

**What is PHP?**

* PHP is an acronym for "PHP: Hypertext Preprocessor"
    
* PHP is a widely-used, open source scripting language
    
* PHP is free to download and use
    
* PHP scripts are executed on the server
    

**How Effective Is PHP?**

1.\]PHP can produce dynamic content for web pages.

2.\]On the server, PHP may open, create, read, write, delete, and close files.

3.\]PHP may get data from forms.

4.\]PHP is capable of exchanging cookies.

5.\] PHP allows you to add, remove, and alter database records.

6.\]The usage of PHP to manage user access PHP can encrypt data.

7.\]PHP does not just allow for HTML output.

8.\]You may create PDF files or photos. Any text, including XHTML and XML, can be produced as well.

**Why PHP?**

A variety of systems support PHP (Windows, Linux, Unix, Mac OS X, etc.) PHP works with nearly all servers in use today (Apache, IIS, etc.) PHP is compatible with a variety of databases. PHP is simple to learn and performs well on servers.

**PHP SYNTAX**

*Basic PHP Syntax*

A PHP script can be placed anywhere in the document.

A PHP script starts with

```php
<?php and ends with ?>

<?php // PHP code goes here ?>
```

The default file extension for PHP files is ".php".

A PHP file normally contains HTML tags, and some PHP scripting code.

**PHP Case Sensitivity**

In PHP, keywords (e.g. `if`, `else`, `while`, `echo`, etc.), classes, functions, and user-defined functions are not case-sensitive.

In the example below, all three echo statements below are equal and legal:

Example:

```php
<!DOCTYPE html> 
<html>
<body> 
<?php ECHO "Hello World!<br>"; 
echo "Hello World!<br>"; 
EcHo "Hello World!<br>"; ?> 
</body>
</html>
```

**Note:** However; all variable names are case-sensitive!

Look at the example below; only the first statement will display the value of the `$color` variable! This is because `$color`, `$COLOR`, and `$coLOR` are treated as three different variables:

Example

`<!DOCTYPE html> <html> <body> <?php $color = "red"; echo "My car is " . $color . "<br>"; echo "My house is " . $COLOR . "<br>"; echo "My boat is " . $coLOR . "<br>"; ?> </body> </html>`

**PHP Data Types**

Variables can store data of different types, and different data types can do different things.

PHP supports the following data types:

* String
    
* Integer
    
* Float (floating point numbers - also called double)
    
* Boolean
    
* Array
    
* Object
    
* NULL
    
* Resource
    

**PHP Integer**

An integer data type is a non-decimal number between -2,147,483,648 and 2,147,483,647.

Rules for integers:

* An integer must have at least one digit
    
* An integer must not have a decimal point
    
* An integer can be either positive or negative
    
* Integers can be specified in: decimal (base 10), hexadecimal (base 16), octal (base 8), or binary (base 2) notation
    

In the following example $x is an integer. The PHP var\_dump() function returns the data type and value:

Example

`<?php $x = 5985; var_dump($x); ?>`

**PHP Float**

A float (floating point number) is a number with a decimal point or a number in exponential form.

In the following example $x is a float. The PHP var\_dump() function returns the data type and value:

Example

`<?php`  
`$x = 10.365; var_dump($x); ?>`

**PHP Object**

Classes and objects are the two main aspects of object-oriented programming.

A class is a template for objects, and an object is an instance of a class.

When the individual objects are created, they inherit all the properties and behaviors from the class, but each object will have different values for the properties.

Let's assume we have a class named Car. A Car can have properties like model, color, etc. We can define variables like $model, $color, and so on, to hold the values of these properties.

When the individual objects (Volvo, BMW, Toyota, etc.) are created, they inherit all the properties and behaviors from the class, but each object will have different values for the properties.

If you create a \_\_construct() function, PHP will automatically call this function when you create an object from a class.

Example

`<?php class Car {   public $color;   public $model;   public function __construct($color, $model) {     $this->color = $color;     $this->model = $model;   }   public function message() {     return "My car is a " . $this->color . " " . $this->model . "!";   } } $myCar = new Car("black", "Volvo"); echo $myCar -> message(); echo "<br>"; $myCar = new Car("red", "Toyota"); echo $myCar -> message(); ?>`

**PHP Strings**

A string is a sequence of characters, like "Hello world!".

***PHP String Functions***

In this chapter we will look at some commonly used functions to manipulate strings.

**strlen() *\-*** Return the Length of a String

The PHP `strlen()` function returns the length of a string.

Example

Return the length of the string "Hello world!":

`<?php echo strlen("Hello world!"); // outputs 12 ?>`

**str\_word\_count() -** Count Words in a String

The PHP `str_word_count()` function counts the number of words in a string.

Example

Count the number of word in the string "Hello world!":

`<?php echo str_word_count("Hello world!"); // outputs 2 ?>`

**strrev()** - Reverse a String

The PHP `strrev()` function reverses a string.

*Example*

Reverse the string "Hello world!":

&lt;?php  
echo strrev("Hello world!"); // outputs !dlrow olleH  
?&gt;

**strpos()** - Search For a Text Within a String

The PHP `strpos()` function searches for a specific text within a string. If a match is found, the function returns the character position of the first match. If no match is found, it will return FALSE.

*Example*

Search for the text "world" in the string "Hello world!":

`<?php echo strpos("Hello world!", "world"); // outputs 6 ?>`

**Tip:** The first character position in a string is 0 (not 1).

**str\_replace()** - Replace Text Within a String

The PHP `str_replace()` function replaces some characters with some other characters in a string.

*Example*

Replace the text "world" with "Dolly":

`<?php echo str_replace("world", "Dolly", "Hello world!"); // outputs Hello Dolly! ?>`

**The PHP switch Statement**

Use the `switch` statement to select one of many blocks of code to be executed.The `switch` statement is used to perform different actions based on different conditions.

Syntax

`switch (n)`

`{`

`case label1:     code to be executed if n=label1;`

`break;`

`case label2:     code to be executed if n=label2;`

`break;   case label3:     code to be executed if n=label3;`

`break;     ...   default:     code to be executed if n is different from all labels;`

`}`

This is how it works: First we have a single expression *n* (most often a variable), that is evaluated once. The value of the expression is then compared with the values for each case in the structure. If there is a match, the block of code associated with that case is executed. Use `break` to prevent the code from running into the next case automatically. The `default` statement is used if no match is found.

Example

`<?php $favcolor = "red"; switch ($favcolor)`

`{   case "red":     echo "Your favorite color is red!";`

`break;`

`case "blue":     echo "Your favorite color is blue!";`

`break;`

`case "green":     echo "Your favorite color is green!";`

`break;`

`default:     echo "Your favorite color is neither red, blue, nor green!";`

`} ?>`

**PHP Loops**

When writing code, you frequently want a particular block of code to execute a given number of times again. Thus, we may utilise loops in a script rather than adding several almost identical code lines.

Loops are used to repeatedly run the same piece of code as long as a specific condition is met.

While the stated condition is true, while cycles over the block of code...

while - executes a loop over a piece of code once as long as the given condition is true for - loops over a block of code for each element in an array for a predetermined number of iterations for each The chapters that follow will explain and give examples of each loop type.

The `while` loop executes a block of code as long as the specified condition is true.

Syntax

while (*condition is true*)

`{   code to be executed; }`

Examples

The example below displays the numbers from 1 to 5:

`<?php $x = 1; while($x <= 5) {   echo "The number is: $x <br>";   $x++; } ?>`

Example Explained

* $x = 1; - Initialize the loop counter ($x), and set the start value to 1
    
* $x &lt;= 5 - Continue the loop as long as $x is less than or equal to 5
    
* $x++; - Increase the loop counter value by 1 for each iteration
    

This example counts to 100 by tens:

`<?php $x = 0; while($x <= 100) {   echo "The number is: $x <br>";   $x+=10; } ?>`
---
title: "jQuery"
datePublished: Tue Jan 03 2023 17:25:43 GMT+0000 (Coordinated Universal Time)
cuid: clcgi4o1l000j08l99kelg52j
slug: jquery
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1672764664496/afb462f1-e4ec-4993-b2f9-fad985b7dd10.png

---

**What You Should Already Know**

Before you start studying jQuery, you should have a basic knowledge of:

1. HTML
    
2. CSS
    
3. javascript
    

**<mark>What is jQuery?</mark>**

The "*write less, do more"* JavaScript library jQuery is small and efficient.The goal of jQuery is to make using JavaScript on your website more simpler.

With the help of jQuery, you can perform many basic activities that would otherwise require several lines of JavaScript code by using methods instead.

AJAX requests and DOM manipulation are only a couple of the complex JavaScript features that are greatly simplified by jQuery.

There are lots of other JavaScript libraries out there, but jQuery is probably the most popular, and also the most extendable.

Many of the biggest companies on the Web use jQuery, such as:

* Google
    
* Microsoft
    
* IBM
    
* Netflix
    

  
Adding jQuery to Your Web Pages

There are several ways to start using jQuery on your web site. You can:

* Download the jQuery library from [jQuery.com](http://jQuery.com)
    
* Include jQuery from a CDN, like Google
    

**jQuery CDN**

If you don't want to download and host jQuery yourself, you can include it from a CDN (Content Delivery Network).

Google is an example of someone who host jQuery:

**Google CDN:**

`<head>   <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.1/jquery.min.js"></script>   </head>`

**<mark>jQuery Syntax</mark>**

The jQuery syntax is tailor-made for **selecting** HTML elements and performing some **action** on the element(s).

Basic syntax is: **$(*selector*).*action*()**

* A $ sign to define/access jQuery
    
* A (*selector*) to "query (or find)" HTML elements
    
* A jQuery *action*() to be performed on the element(s)
    

Examples:

`$(this).hide()` - hides the current element.

`$("p").hide()` - hides all &lt;p&gt; elements.

`$(".test").hide()` - hides all elements with class="test".

`$("#test").hide()` - hides the element with id="test".

You might have noticed that all jQuery methods in our examples, are inside a document ready event:

`$(document).ready(function()`

`{        // jQuery methods go here...      }`

`);`

This is to prevent any jQuery code from running before the document is finished loading (is ready).

It is good practice to wait for the document to be fully loaded and ready before working with it. This also allows you to have your JavaScript code before the body of your document, in the head section.

Here are some examples of actions that can fail if methods are run before the document is fully loaded:

* Trying to hide an element that is not created yet
    
* Trying to get the size of an image that is not loaded yet
    

**<mark>jQuery Selectors</mark>**

jQuery selectors allow you to select and manipulate HTML element(s).

jQuery selectors are used to "find" (or select) HTML elements based on their name, id, classes, types, attributes, values of attributes and much more. It's based on the existing [CSS Selectors](https://www.w3schools.com/cssref/css_selectors.asp), and in addition, it has some own custom selectors.

All selectors in jQuery start with the dollar sign and parentheses: $().

**<mark>The element Selector</mark>**

The jQuery element selector selects elements based on the element name.

**<mark>The #id Selector</mark>**

The jQuery `#id` selector uses the id attribute of an HTML tag to find the specific element.

An id should be unique within a page, so you should use the #id selector when you want to find a single, unique element.

To find an element with a specific id, write a hash character, followed by the id of the HTML element:

`$("#test")`

When a user clicks on a button, the element with id="test" will be hidden:

**Example**

`$(document).ready(function(){     $("button").click(function(){       $("#test").hide();     });   });`

**<mark>What are Events?</mark>**

All the different visitors' actions that a web page can respond to are called events.

An event represents the precise moment when something happens.

Examples:

* moving a mouse over an element
    
* selecting a radio button
    
* clicking on an element
    

The term **"fires/fired"** is often used with events. Example: "The keypress event is fired, the moment you press a key".  

**<mark>jQuery Syntax For Event Methods</mark>**

In jQuery, most DOM events have an equivalent jQuery method.

To assign a click event to all paragraphs on a page, you can do this:

`$("p").click();`

The next step is to define what should happen when the event fires. You must pass a function to the event:

`$("p").click(function()`

`{     // action goes here!!   }`

`);`

**Get Content - text(), html(), and val()**

Three simple, but useful, jQuery methods for DOM manipulation are:

* `text()` - Sets or returns the text content of selected elements
    
* `html()` - Sets or returns the content of selected elements (including HTML markup)
    
* `val()` - Sets or returns the value of form fields
    

The following example demonstrates how to get content with the jQuery `text()` and `html()` methods:

*Example*

`$("#btn1").click(function()`

`{     alert("Text: " + $("#test").text());   }`

`);   $("#btn2").click(function()`

`{     alert("HTML: " + $("#test").html());   }`

`);`

**Set Content - text(), html(), and val()**

We will use the same three methods from the previous page to **set content**:

* `text()` - Sets or returns the text content of selected elements
    
* `html()` - Sets or returns the content of selected elements (including HTML markup)
    
* `val()` - Sets or returns the value of form fields
    

The following example demonstrates how to set content with the jQuery `text()`, `html()`, and `val()` methods:

Example

`$("#btn1").click(function()`

`{     $("#test1").text("Hello world!");   }`

`);   $("#btn2").click(function()`

`{     $("#test2").html("<b>Hello world!</b>");   }`

`);   $("#btn3").click(function()`

`{     $("#test3").val("Dolly Duck");   }`

`);`

**jQuery-add elements**

Add New HTML Content

We will look at four jQuery methods that are used to add new content:

* `append()` - Inserts content at the end of the selected elements
    
* `prepend()` - Inserts content at the beginning of the selected elements
    
* `after()` - Inserts content after the selected elements
    
* `before()` - Inserts content before the selected elements
    
    **jQuery - Remove Elements**
    
    With jQuery, it is easy to remove existing HTML elements.
    
    **Remove Elements/Content**
    
    To remove elements and content, there are mainly two jQuery methods:
    
    * `remove()` - Removes the selected element (and its child elements)
        
    * `empty()` - Removes the child elements from the selected element
        
    
    jQuery remove() Method
    
    The jQuery `remove()` method removes the selected element(s) and its child elements.
    
    `$("#div1").remove();`
    
    **jQuery empty() Method**
    
    The jQuery `empty()` method removes the child elements of the selected element(s).
    
    Example
    
    `$("#div1").empty();`
    

**jQuery Manipulating CSS**

jQuery has several methods for CSS manipulation. We will look at the following methods:

* `addClass()` - Adds one or more classes to the selected elements
    
* `removeClass()` - Removes one or more classes from the selected elements
    
* `toggleClass()` - Toggles between adding/removing classes from the selected elements
    
* `css()` - Sets or returns the style attribute
    

Example Stylesheet

The following stylesheet will be used for all the examples on this page:

`.important {     font-weight: bold;     font-size: xx-large;   }      .blue {     color: blue;   }`

**jQuery Dimension Methods**

jQuery has several important methods for working with dimensions:

* `width()`
    
* `height()`
    
* `innerWidth()`
    
* `innerHeight()`
    
* `outerWidth()`
    
* `outerHeight()`
    

**jQuery width() and height() Methods**

The `width()` method sets or returns the width of an element (excludes padding, border and margin).

The `height()` method sets or returns the height of an element (excludes padding, border and margin).

The following example returns the width and height of a specified `<div>` element:

Example

`$("button").click(function()`

`{     var txt = "";     txt += "Width: " + $("#div1").width() + "</br>";     txt += "Height: " + $("#div1").height();     $("#div1").html(txt);   }`

`)`
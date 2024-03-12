---
title: "How much JavaScript do you need to know to use Node.js?"
datePublished: Wed Feb 01 2023 16:59:07 GMT+0000 (Coordinated Universal Time)
cuid: cldlwy5hr000009kycwc8elpa
slug: how-much-javascript-do-you-need-to-know-to-use-nodejs
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1675270181234/08986e1a-f2df-4ac5-83da-5b19546636c3.jpeg
tags: nodejs, nodejs-developer

---

# **What is Node.js?**

Node.js is a server-side platform built on Google Chrome's JavaScript Engine (V8 Engine), developed by Ryan Dahl in 2009.

The definition of Node.js is −

Node.js is a platform built on Chrome’s JavaScript runtime for easily building fast and scalable network applications. Node.js uses an event-driven, non-blocking I/O model that makes it lightweight and efficient, perfect for data-intensive real-time applications that run across distributed devices.

Node.js is an open-source, cross-platform runtime environment for the development of server-side and networking applications. Node.js applications are written in JavaScript which can be run within the Node.js runtime on OS X, Microsoft Windows, and Linux.

Node.js provides various JavaScript libraries modules that simplify the development of web applications using Node.js to a great extent.

Node.js = Runtime Environment + JavaScript Library.

Now we will look at its features-

* **Asynchronous and Event Driven** − All APIs of the Node.js library are asynchronous, that is, non-blocking. It means a Node.js based server never waits for an API to return data. The server moves to the next API after calling it and a notification mechanism of Events of Node.js helps the server to get a response from the previous API call.
    
* **Faster execution**− Being built on Google Chrome's V8 JavaScript Engine, Node.js library is very fast in code execution.
    
* **Single-Threaded but Highly Scalable** − Node.js uses a single-threaded model with event looping. The event mechanism helps the server to respond in a non-blocking way which makes the server highly scalable.Node.js uses a single-threaded program and the same program can provide service to a much larger number of requests than traditional servers like Apache HTTP Server.
    
* **No Buffering** − Node.js applications don’t buffer any data. These applications produce output in chunks.
    

**To download node.js**

This [link](https://nodejs.org) will lead you to the official website of node.js where you download node.js .

**Who Uses Node.js?**

The user of Node.js includes eBay, General Electric, GoDaddy, Microsoft, PayPal, Uber, Wikipins, Yahoo!, and Yammer to name a few.

# How much JavaScript do you need to know to use Node.js?

As a beginner, it's hard to get to a point where you are confident enough in your programming abilities. While learning to code, you might also be confused about where JavaScript end, and where Node.js begins, and vice versa.

But you should have prior knowledge of using JavaScript.

Following are some topics you should learn in brief before you move on to node.js

* Lexical Structure
    
* Expressions
    
* Data Types
    
* Classes
    
* Variables
    
* Functions
    
* this operato[r](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/this)
    
* Arrow Functions
    
* Loops
    
* Scopes
    
* Arrays
    
* Template Literals
    
* Strict Mode
    
* ECMAScript 2015 (ES6) and beyond
    

Following is a basic code of node.js

```javascript
var http = require('http');
http.createServer(function (req, res) {
  res.writeHead(200, {'Content-Type': 'text/plain'});
  res.end('Hello World!');
}).listen(8080);
```

output:

`Hello World`

**Where to Use Node.js?**

Following are the areas where Node.js is proving itself as a perfect technology partner.

* I/O bound Applications
    
* Data Streaming Applications
    
* Data Intensive Real-time Applications (DIRT)
    
* JSON APIs based Applications
    
* Single Page Applications
    

So readers, today we read about Node.js and how much prior knowledge needed to become expert in this platform.See you in the next blog.
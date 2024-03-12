---
title: "DOM manipulation and Reconciliation in React.js"
datePublished: Wed Dec 21 2022 17:12:03 GMT+0000 (Coordinated Universal Time)
cuid: clbxwx09a000208mg8txg0eab
slug: dom-manipulation-and-reconciliation-in-reactjs
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1671641688766/a5BJoPAdE.jpg
tags: virtual-dom, dom, reactjs, dom-manipulation

---

# DOM-

DOM means Document Object Model. HTML, the language of web pages provides the web page structure with many specialized tags, including a way to link multiple pages together. The structure of a web page is represented as a tree structure that is called a document object. The JavaScript programming language can change the structure of this document object to make dynamic behavior to the web pages.

The DOM(Document Object Model) is the programming interface for the tree structure web page documents. The document tree is called DOM Tree.

Let's understand DOM with an example. This is an HTML code snippet, that aims to show the title of a web page and some information in the body of the page.

```xml
<! DOCTTYPE html>
<html>
<head>
<title>
what is DOM
</title>
</head>
<body>
<h1>DOM </h1>
<p>DOM is Document Object Model</p>
</body>
</html>
```

In the above code snippet i.e a document tree. Each of the HTML elements represents a node in the tree.

The output will be :

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1671642181418/dERH7b1Nw.avif align="center")

The mechanism of finding a particular node in the document tree is called Querying the DOM. Adding, deleting or updating a node in the document tree is called DOM Manipulation. The result of a DOM manipulation reflects on the web user interface. This process is called rendering.

# DOM manipulation -

DOM Manipulation is the process by which you can dynamically change the content of the web page. While working with the DOM javascript is used. Methods like getElementById or removeChild are part of the API provided by the HTML DOM.

### Main issue:

DOM Manipulation is the core of every interactive web pages. So, the DOM must be easy and faster. Since, it is tree-structured, traversing the DOM is easy. But when it comes to the quick part, it becomes slower.

For example, let us say we want to update the first item of a list containing 20 items. Most JavaScript frameworks would update the entire list, just to update only the first item. This behavior would cost too much. We can say that frequent update to the DOM is costly. It may degrade the web page performance and makes it slow

To overcome this problem, React introduced something called `Virtual DOM`.

# Virtual DOM-

ReactJS never updates the original DOM directly(unless a developer use case requires it). In ReactJS, for every DOM object, there will be a corresponding in-memory copy created and this copy is called the Virtual DOM(VDOM).

In the Virtual DOM tree, each element is represented by a node. A new Virtual DOM tree will be created whenever the element's state changes. The ReactJS's diffing algorithm will compare the present Virtual DOM tree with its previous version. The Virtual DOM uses the algorithm to update the actual DOM with the diff.

### Methodology:

*   First, ReactJS creates a copy of the original DOM, it is called the Virtual DOM. Each node of the Virtual DOM represents an element.
    
*   If there is any state update of an element, a new Virtual DOM is created.
    
*   The diffing algorithm identifies the difference of the change. Where a subtree from the changed node has been identified as the diff.
    
*   ReactJS runs a batch to update the Original DOM with these changes to keep it in sync.
    

The mechanism to diff one tree with another tree to determine which parts need to be changed and then update the original DOM. The process is called `Reconciliation`.

# An overview of the reconciliation process -

Reconciliation is the process by which React updates the Browser DOM. The reconciliation process makes React work faster.

Important concepts behind the working of Reconciliation process are:

*   Virtual DOM
    
*   Diffing Algorithm
    

The term rendering in React can closely be identified as making or becoming. In traditional rendering, Browser does the following tasks-

*   Creates a DOM then renders any new data to the DOM even if data is similar to previous ones.
    
*   This rendering by Browser has a sequence of steps and is rather costly. The concept of Virtual DOM used by React makes rendering much faster.
    

As we already discussed virtual DOM and how it works, as the name suggests virtual DOM is a `virtual` representation of the actual DOM. It is lightweight. In React JS, every DOM element has a corresponding Virtual DOM Object. No doubt that the virtual DOM has the same features as we have in the original DOM object but unlike the DOM object where we can directly change what is on the screen, we cannot do that for the virtual DOM.

## **How Virtual DOM makes things faster:**

When a new thing is added to the application, a virtual DOM is created and it is represented as a tree. Each element in the application is a node in this tree. So, whenever there is a change in the state of any element, a new Virtual DOM tree is created. This Virtual DOM tree is then compared with the previous Virtual DOM tree and makes a note of the changes. Then, it finds the best possible ways to make these changes to the real DOM. And only the updated elements will get rendered on the page again.

## Diffing Algorithm :

The diffing algorithm is generating the minimum number of operations to transform one tree into another. However, the algorithms have a complexity in the order of O(n3) where n is the number of elements in the tree.

It is based on two assumptions-

Elements of different types will produce different trees

We can set which elements are static and do not need to be checked.

React checks the root elements for changes and the updates depend on its types,

**Element in different types:** Whenever the type of the element changes in the root, react will scrap the previous tree and build a new one.

**Elements of the same type:** When the type of the changed element is the same, React then checks for attributes of both versions and then only updates the node which has changes without any changes in the tree. The component will be updated in the next lifecycle call.

So we learned about DOM, the issue we faced in DOM, virtual DOM and reconciliation process. We hope you enjoyed it. Happy learning.
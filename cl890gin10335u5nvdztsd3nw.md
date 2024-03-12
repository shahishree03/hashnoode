---
title: "What is Jamstack ?"
datePublished: Mon Sep 19 2022 16:57:50 GMT+0000 (Coordinated Universal Time)
cuid: cl890gin10335u5nvdztsd3nw
slug: what-is-jamstack
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1663595848057/QKFzun-NU.jpg
tags: technology, apis, learning, markup, jamstack

---

%[https://app.techlearnindia.com/ktech-academy]

![Jamstack_logo.svg.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1663596193608/tZhLY2U22.png align="left")
****JAMstack**** is software architecture and philosophy with an approach to fronted web development. It allows developers to quickly create and efficiently serve static website to users. JAMstack web application as much HTML as possible is pre built and stored in a content delivery network. Instead of running a monolithic backend application on the server side to generate dynamic content, dynamic components of the application are based on APIs that adheres to the following components :

****Javascript ****

****APIs****

****Markup****

****  :-What makes up the JAMstack? ****


Its history stems from growing the terms static site into something meaningful . So while a static site is the end result , its blown up to include first class tooling for every step of the way . There arn't specific tools that you need to use or any tools at all beyond simple HTML, there are great examples of what can make up each part of the stack.

****Javascript****

The component that's probably done the most work to popularise the JAMstack is Javascript. Our favorite browser language allows us to provide all of dynamic and interactive bits that we might not have if we're serving plain HTML without it.
This is where a lor od times you'll see UI framework like React, Vue and newcomers like Svelte come into play.
They make building apps similar and more Organized by providing components APIs and tooling that compile down to a simple HTML file.
Thosw HTML files include a group of assets like images, CSS and the actual JS that ultimately get served to a browser via your favorite Content Delivery Network ( CDN )
Javascript website are built to be flexible and not have one part of architectural setup limit. When you use a traditional content management system often referred ae using a monolith system yoy have everything coupled together. The database content and fronted templating are all handled in the system which means it's all depended upon each other. While there's nothing inherently wrong with that it can be limiting in terms of functionality and performance. 
Javascript is in charge of displaying the content to the user and ensuring a great user experience. And since it's all decoupled from the content it has complete freedom in how to do it. To avoid lack of flexibility a JAMstack site is spilt up and each part serves more specific and limited purpose. 

****APIs****

Utilising the strength of APIs is core to how you make a JAMstack apo dynamic. Whether it's authentication or search your application will usw Javascript to make an HTTP request to another provider which will ultimately enhance the experience in one form or another.
You don't necessarily have to reach out to only one host for an APIs but you can reach out to as many as you need. 
If you have headless WordPress APIs where you host your blog posts a Cloudinary account where you store your specialised media and ab Elasticsearch instance that provides your search functionality they all w9rk together to provide a single experience to the people using your site. 
APIs were only meant to consumed by server side application as that was the wat it was done at the time. But with the development of new Javascript standards all changed. Web APIs were developed and became available to any Javascript client running in a browser. 

****Markup**** 

This is the critical piece. Whether it's your handwritten HTML or the code that compiles down to the GTML, its the first part you're serving to the client. This is the kind of website but how you servebit is the most important. 
To be considered a JAMstack, the HTML beeds to be served statically which is basically means not being dynamically rendered from the server. 
If you're piecing a page together and serving it will PHP it's probably not a JAMstack app. If you upload and serve a single HTML file from storage that construct an app with Javascript it sounds like a JAMstack app. 
But that doesn't mean we have always build 100%of app within the browser. Toolsike Gatsby and other static site generator allow us to pull in all of post and ultimately create a new HTML file for each post. That means we're going to be able to serve a precompiled version of the page directly to the browser which usually equates to a quicker first paint and faster experience for your visitors. 
While HTML has come a long way it's primary job is still to serve up content and it's structured to the browser to display. This has not fundamentally changed with JAMstack sites. But the way it is being done and has served. 
With the markup pre built and ready to be consumed, it is up to Javascript to call in the content it needs. If Dynamic or customised content is required APIs will handle it instead of having the server request from database. 
![featured.jpeg](https://cdn.hashnode.com/res/hashnode/image/upload/v1663596054139/UiYhhtXaY.jpeg align="left")

****What makes JAMstack so great? ****

JAMstack apps inherently satisfy most if not all of the 5 pillars of AWS Well Architected framework. These are core concept that AWS consider to deliver fast, secure, high performing, resilient and efficient infrastructure. 

****Speed **** :

The fact thar you're serving JAMstack app as static files directly from CDN makes it likely your app is going to load superfast Gone are the days where the setver has to spend time building the page before responding now you serve the page as just plain HTML "as is"  or with some type of client side hydration like you'd see with react. 

****Cost****:

More often that not, JAMstack site are going to run cheaper than their server side counterpart. Hosting static asset is cheap and now your page is being served at the same rate. 

****Scalability ****:

Since you're serving your files off static hosting likely a CDN that pretty much automatically gives you infinite scalability. Most providers will make this claim, meaning you'll have no trouble letting any influx of people hitting your site in through the front door. 

****Maintenance ****:

The foundation of your static site isn't a server meaning you don't need to maintain it. Whether it's Netlify, S3 or any provider your static HTML , CSS and JS are maintained for your headache free. 

****Security****:

Doubling down on the lack of server that you have to personally maintain you don't need to worry as much about looking down ways for the people to tribute. 
Instead, you'll need to focus mostly on permission to lock down private content and assure your users that their information isn't publically available.
![JAMstack workflow.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1663598475873/CRe0Fn5E8.png align="left")

%[https://app.techlearnindia.com/ktech-academy]

Written by :Deepshikha Niyogi 

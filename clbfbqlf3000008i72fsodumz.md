---
title: "Create a Next.js App"
datePublished: Thu Dec 08 2022 16:59:20 GMT+0000 (Coordinated Universal Time)
cuid: clbfbqlf3000008i72fsodumz
slug: create-a-nextjs-app
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1670518666345/YWkHOoHeD.png

---

There are several crucial factors you must take into account if you're creating a full-featured web application from scratch with React:

1.] Code has to be converted using a compiler like Babel and packaged using a bundler like webpack.  
2.] Production improvements like code splitting must be carried out.  
3.] For speed and SEO, you might wish to statically pre-render some pages.    
4.] Use of client-side rendering or server-side rendering may also be desirable.  

In order to link your React app to your data store, you might need to create some server-side code.
These issues can be resolved by a framework. But for such a framework to be effective, the degree of abstraction must be just right. It must also have excellent "Developer Experience," guaranteeing that you and your team enjoy a fantastic experience.

**Next.js: The React Framework**

All of the aforementioned issues are addressed with Next.js. However, it is more significant in that it places you and your team in a position to succeed when developing React apps.

With its many built-in capabilities and best-in-class developer experience, Next.js strives to provide:

1.) A user-friendly page-based routing framework (with support for dynamic routes).
2.) Static generation (SSG) and server-side rendering (SSR) for pre-rendering are both available on a per-page basis.  
3.) Code splitting automatically to speed up page loads.   
4.) Prefetching that is optimised for the client.   
5.) Development environment with Fast support API routes to create API endpoints with Serverless Functions, as well as built-in CSS and Sass support.    
6.) Total extendibility.  

Tens of thousands of production-oriented websites and online apps, including many of the biggest brands in the world, employ js.

# **Setup**

Let's start by making sure your development environment is prepared.

-> Install [Node.js](https://nodejs.org/en/download/) from here if you don't already have it. Node.js 10.13 or later is required.   
-> For this training, you'll be using your own text editor and terminal application.    

Git for Windows, which comes with Git Bash and supports the UNIX-specific commands in this lesson, is advised if you are using Windows. Another choice is the Windows Subsystem for Linux (WSL).

# **Create a Next.js app**
To create a Next.js app, open your terminal, cd into the directory you’d like to create the app in, and run the following command:
```
npx create-next-app@latest nextjs-blog --use-npm --example "https://github.com/vercel/next-learn/tree/master/basics/learn-starter"
```

Under the hood, this uses the tool called create-next-app, which bootstraps a Next.js app for you. It uses this template through the --example flag.
If it doesn’t work, please take a look at this page.

**Run the development server**

You now have a new directory called nextjs-blog. Let’s cd into it:
```
cd nextjs-blog
```

Then, run the following command:
```
npm run dev
```
This starts your Next.js app’s "development server" (more on this later) on port 3000.

Let’s check to see if it’s working. Open http://localhost:3000 from your browser.

**Navigate between pages**

The Next.js application we developed so far just has one page. In general, websites and online applications have a large number of pages.

Let's look at how to expand our application with new pages.

What This Lesson Will Teach You
This lesson will teach you:

-> Utilize the integrated file system routing to create a new page.   
-> Learn how to provide client-side navigation across pages by using the Link component.   
-> Learn about code splitting and prefetching built-in support.  

Next.js-enabled pages
A page in Next.js is a React Component exported from a file in the directory for pages.

Based on the file name of the page, a route is connected with it. For instance, in progress

1.] The / route is connected with pages/index.js.   
2.] The /posts/first-post route is related with pages/posts/first-post.js.      

Let's create pages/posts/first-post.js to test it out because we already have the files for pages/index.js and pages/posts.

Launch a New Page
Make a posts directory in the pages directory.

Make a file named first-post.js in the directory for posts with the following information:

```
export default function FirstPost()
 {
  return <h1>First Post</h1>;
 }
```

**TypeScript**      
Navigate Between Pages
Pages in Next.js
In Next.js, a page is a React Component exported from a file in the pages directory.

Pages are associated with a route based on their file name. For example, in development:

pages/index.js is associated with the / route.
pages/posts/first-post.js is associated with the /posts/first-post route.
We already have the pages/index.js file, so let’s create pages/posts/first-post.js to see how it works.

**Create a New Page**   


![welcome-to-nextjs.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1670518731209/tAUeDolYX.png align="left")

Create the posts directory under pages.

Create a file called first-post.js inside the posts directory with the following content:

```
export default function FirstPost() 
{
  return First Post;
}
```
The component can have any name, but you must export it as a default export.

Now, make sure that the development server is running and visit http://localhost:3000/posts/first-post. You should see the page:


This is how you can create different pages in Next.js.

Simply create a JS file under the pages directory, and the path to the file becomes the URL path.

In a way, this is similar to building websites using HTML or PHP files. Instead of writing HTML you write JSX and use React Components.

Let's add a link to the newly added page so that we can navigate to it from the homepage.

**Link Component**

When linking between pages on websites, you use the <a> HTML tag.

In Next.js, you can use the Link Component next/link to link between pages in your application. <Link> allows you to do client-side navigation and accepts props that give you better control over the navigation behavior.

Using <Link>
First, open pages/index.js, and import the Link component from next/link by adding this line at the top:
```
import Link from 'next/link';
```
Then find the h1 tag that looks like this:

```
<h1 className="title">
  Welcome to <a href="https://nextjs.org">Next.js!</a>
</h1>
```
And change it to:

```
<h1 className="title">
  Read <Link href="/posts/first-post">this page!</Link>
</h1>
```
Next, open pages/posts/first-post.js and replace its content with the following:

```
import Link from 'next/link';

export default function FirstPost()
{
  return (
    <>
      <h1>First Post</h1>
      <h2>
        <Link href="/">Back to home</Link>
      </h2>
    </>
  );
}
```

As you can see, the Link component is similar to using <a> tags, but instead of <a href="…"> , you use <Link href="…"> .

**Code splitting and prefetching**   
Next.js does code splitting automatically. As a result, each page only loads the content that is required. That implies that the code for other pages is not first served when the homepage is shown.

This guarantees that even if your homepage has hundreds of pages, it loads swiftly.

Pages become isolated because just the code for the page you request is loaded. Even if a particular page contains an error, the remainder of the programme will continue to function.

Every time a Link component appears in the browser's viewport, a production build of Next.js automatically prefetches the code for the connected website in the background. The background loading of the destination website's code will have finished by the time you click the link, making the page change practically instantaneous!
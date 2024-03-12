---
title: "Vite.Js"
datePublished: Thu Jan 19 2023 15:42:02 GMT+0000 (Coordinated Universal Time)
cuid: cld39gy2n000k08kzb8tnaqek
slug: vitejs
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1674142906067/b5de7b40-bb05-4266-a7d3-1e2806d50b6e.jpeg

---

### Introduction

A build tool called Vite greatly enhances the front-end development process. With only three lines, Vite enables you to set up a development environment for frameworks like Vue and React as well as for a simple JavaScript application with a dev server and quick reloading.

With no extra configuration, you can also use Vite for TypeScript, and with one additional command, you can use it for Sass. (That would take a lot of config for a webpack project. You’d need to mess around with loaders and separately install the webpack dev server.)

Once you have Vite installed, you’ll have a build tool and dev server and be ready to start working with the latest tools and languages.

In this introduction, you’ll learn how simple it is to get up and running with Vite. You’ll also learn about how fast Vite is, how to take the first steps towards using it with a library such as Vue, and how much it gets out of your way when you’re using it.

***Fun fact****: the name “Vite” comes from the French word for “fast”, which is pronounced, “vit”.*

### How Vite Works?

Vite follows a recent trend of tools like Svelte (where the framework is basically compiled away) and other tools like Snowpack that leverage modern JavaScript features (such as ES modules) to provide a smooth, fast dev experience with little to no configuration and not much overhead in the way of installed packages. You basically install Vite with a plugin or two, do very little configuration, and just start working on your app.

Vite provides a modern dev environment that can forego the bundling step because it serves the browser's native ES modules. It provides templates (a set of starter files) for a number of frameworks and vanilla JavaScript and also offers TypeScript, JSX and Sass support (although you need to install one dependency for Sass).

Vite is really fast, because it leverages native ES modules and doesn’t need to rebuild the whole bundle when something changes. This makes HMR updates consistently fast, regardless of the size of your application. When bundling for production, Vite ships with a pre-configured build command that bakes in many performance optimizations out of the box.

As well as being fast, Vite also offers hot module replacement (meaning you see the code refresh in the browser as you develop), and you can use it to compile a minified version of your project to serve in production. By using it, you can get up and running very quickly with a Vue or React project without the buy-in to the Vue CLI or Create React App, both of which ship with the kitchen sink included. This makes it ideal for quick prototyping and smaller projects, although there’s nothing stopping you from using it in a larger project either.

So, let’s take Vite for a spin and see how we go. It will be interesting to see how much of our normal workflow would be better handled with Vite.

### After Installation

We get to choose a project name and a template. At the time of writing, the options are:

* `vanilla`
    
* `vue`
    
* `vue-ts`
    
* `react`
    
* `react-ts`
    
* `preact`
    
* `preact-ts`
    
* `lit-element`
    
* `lit-element-ts`
    
* `svelte`
    
* `svelte-ts`
    

Let's stick with vanilla for now. This creates a directory with certain files in it based on the project name. There are files for npm and Git, as well as an index.html, main.js, style.css, and favicon.svg. Only a few scripts to launch the development environment and a build are included in the package.json file in addition to vite as a dependency.

The instructions on screen state that we must switch to the project folder and install the dependencies:

```bash
cd vite-project
npm install
```

Then, using npm run dev, we can launch the development server and view our app at [http://localhost:3000/](http://localhost:3000/). Any of our project files that are edited instantly update on the screen.

The project is compiled into a dist folder, where the JavaScript and CSS files are located, by running npm run build. Both files appear to be compressed.

According to the documentation, TypeScript files are supported right out of the box. Despite the lack of a specific TypeScript template in the vanilla option, we should be able to rename main.js to main.ts and Vite should build it for us automatically, right? It does, indeed! It appears to be compiling successfully after renaming the file and adding some TypeScript-specific grammar.

Let’s try the same with CSS by renaming it to `style.scss` and add some Sass-specific syntax. The following error is shown in both the console and on the web page:

![Error message: Internal server error: Preprocessor dependency “sass” not found. Did you install it?](https://uploads.sitepoint.com/wp-content/uploads/2021/03/1617015645error-sass.png align="left")

I do enjoy a (somewhat) detailed mistake! We may now use Sass as much as we like after executing npm instal sass —save-dev and restarting the watcher. Nice.

Normally, I would plan out the stack in advance, instal the necessary dependencies, and spend an absurd amount of time configuring and trying to figure out why some tools won't get along. Of course, we still need to consider our stack in advance, but the fact that we can easily transition from JavaScript to TypeScript and from CSS to Sass is pretty useful.

I'm excited right now since we can build up a really sophisticated stack in a matter of minutes. Given that Vite develops using plain HTML, CSS, and JavaScript and utilises an index.html as the entry point,

Vite already proves to be a great tool for static sites and potentially [**Jamstack**](https://www.sitepoint.com/learn-jamstack/) applications.

### Why prefer Vite over create-react

**1\. Faster spin-up of the development server:**

\-&gt; As dependencies do not change, they can also be cached and we can skip pre-bundling.

\-&gt;Vite pre-bundles these dependencies using esbuild, which is 10-100x faster than JavaScript-based bundlers.

**2\. Less waiting time for reflecting file updates :**

\-&gt; In Vite, Hot Module Replacement(HMR) is performed over native ESM. When a file is edited, Vite invalidates the chain between the edited module and its closest HMR boundary. This makes HMR updates simple and fast regardless of the size of your application.

**3\. Improved build performance**

CSS code splitting: Vite automatically extracts the CSS used by modules in an async chunk and generates a separate file for it. The CSS file is automatically loaded via a &lt;link&gt; tag when the associated async chunk is loaded.

Async chunk loading optimization: While code splitting, Webpack, and Rollup produce a common chunk (code that is shared between two or more other chunks). This, when combined with dynamic import, can lead to many network round trips
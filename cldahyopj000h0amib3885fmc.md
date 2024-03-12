---
title: "Build an app with astro framework"
datePublished: Tue Jan 24 2023 17:14:09 GMT+0000 (Coordinated Universal Time)
cuid: cldahyopj000h0amib3885fmc
slug: build-an-app-with-astro-framework

---

### **What is Astro?**

Astro is a comprehensive web framework for quickly creating websites with an emphasis on their content. Astro works with your favorite content sources. Pulls content from the filesystem or fetches it remotely from your favorite CMS, database, or API. Astro supports both static output (SSG) and live server output (SSR) that can render your content on demand.

**KEY FEATURES:**

1.\] *Component Islands:* A new web architecture for building faster websites.

2.\] *Server-first API design:* Move expensive hydration off of your users’ devices.

*3.\] Zero JS, by default:* No JavaScript runtime overhead to slow you down.

*4.\] Edge-ready:* Deploy anywhere, even a global edge runtimes like Deno or Cloudflare.

*5.\] Customizable:* Tailwind, MDX, and 100+ other integrations to choose from.

*6.\] UI-agnostic:* Supports React, Preact, Svelte, Vue, Solid, Lit and more.

**Starting the first project**

Get a new Astro project up and running locally with our helpful create Astro CLI wizard!

**npm**

```plaintext
# create a new project with npm
npm create astro@latest
```

It has full, step-by-step instructions for installing Astro using our CLI wizard, creating a new project from an existing Astro GitHub repository, and installing Astro manually.

**pnpm**

```plaintext
# create a new project with pnpm
pnpm create astro@latest
```

**yarn**

```plaintext
# create a new project with yarn
yarn create astro
```

**Requirements:**

\-Node.js - v16.12.0 or higher.

\-Text editor - We recommend Vs code with the Official Astro extension.

\-Terminal - Astro is accessed through its command-line interface (CLI).

### **Installation**

Creating Astro is the fastest way to start a new Astro project from scratch. It will walk you through every step of setting up your new Astro project. It allows you to choose from a few different official starter templates or you use any existing project on Git hub with the--template argument.

**1\. Run the Setup Wizard**

Run the following command in your terminal to start our handy install wizard:

**npm** pnpm Yarn

```plaintext
# create a new project with npm
npm create astro@latest
```

You can run create Astro anywhere on your machine, so there’s no need to create a new empty directory for your project before you begin. If you don’t have an empty directory yet for your new project, the wizard will help create one for you automatically.

If all goes well, you should see a “Ready for liftoff!” message followed by some recommended “Next steps”. cd into your new project directory to begin using Astro.

If you skipped the npm install step during the CLI wizard, then be sure to install your dependencies before continuing.

**2\. Start Astro**

Astro comes with a built-in development server that has everything you need for project development. The Astro dev command will start the local development server so that you can see your new website in action for the very first time.

Every starter template comes with a pre-configured script that will run Astro dev for you. Use your favorite package manager to run this command and start the Astro development server.

**npm**

```plaintext
npm run dev
```

If all goes well, Astro should now be serving your project.

Astro will listen for live file changes in your src/ directory, so you will not need to restart the server as you make changes during development.

If you aren’t able to open your project in the browser, go back to the terminal where you ran the dev command and look to see if an error occurred, or if your project is being served at a different URL than the one linked to above.

## **Starter Templates**

You can also start a new Astro project based on an official example or the main branch of any GitHub repository by passing a --template argument to the create Astro command.

**npm**

```plaintext
# create a new project with an official example
npm create astro@latest -- --template <example-name>

# create a new project based on a GitHub repository’s main branch
npm create astro@latest -- --template <github-username>/<github-repo>
```

By default, this command will use the template repository’s main branch. To use a different branch name, pass it as part of the --template argument: &lt;github-username&gt;/&lt;github-repo&gt;#&lt;branch&gt;.

Explore themes and starters showcase where you can browse themes for blogs, portfolios, documentation, landing pages, and more! Or, search on GitHub for even more starter projects.

## **Directories and Files**

[Section titled Directories and Files](https://docs.astro.build/en/core-concepts/project-structure/#directories-and-files)

Astro leverages an opinionated folder layout for your project. Every Astro project root should include the following directories and files:

1.\] src/\* - Your project source code (components, pages, styles, etc.)

2.\] public/\* - Your non-code, unprocessed assets (fonts, icons, etc.)

3.\] package.json - A project manifest.

4.\] Astro config. mjs - An Astro configuration file.

5.\] tsconfig.json - A TypeScript configuration file.

**Example Project Tree**

A common Astro project directory might look like this:

* `public/`
    
    * `robots.txt`
        
    * `favicon.svg`
        
    * `social-image.png`
        
    * `src/`
        
        * `components/`
            
            * `Header.astro`
                
            * `Button.jsx`
                
        * `layouts/`
            
            * `PostLayout.astro`
                
        * `pages/`
            
            * `posts/`
                
                * [`post1.md`](http://post1.md)
                    
                * [`post2.md`](http://post2.md)
                    
                * [`post3.md`](http://post3.md)
                    
            * `index.astro`
                
        * `styles/`
            
            * `global.css`
                
            * `astro.config.mjs`
                
            * `package.json`
                
            * `tsconfig.json`
                

[](https://docs.astro.build/en/core-concepts/project-structure/#src)**The section titled src/**

The src/ folder is where most of your project source code lives. This includes:

* Pages
    
* Layouts
    
* Astro components
    
* UI framework components (React, etc.)
    
* Styles (CSS, Sass)
    
* Markdown
    

Your src/ files are processed, enhanced, and bundled by Astro to produce the finished website that is sent to the browser. Your src/ files, in contrast to the static public/ directory, are created and maintained by Astro.

Some files (such as Astro components) are even transformed to static HTML rather than being given to the browser as intended. In order to improve efficiency, additional files (like CSS) may be bundled with other CSS files or optimized before being transmitted to the browser.

**The section src/components**:

Your HTML pages can use reusable blocks of code called components. These may be UI framework components from React or Vue, or components from Astro. All of your project's components should typically be gathered and organized in this folder.

Although it isn't essential, this is a standard practice in Astro projects. You are able to arrange your parts any way you choose.

**The section src/layouts**:

A unique type of component called a layout encloses certain information in a bigger page layout. Markdown or MDX pages and Astro pages are the ones that use these the most to specify the page's layout.

Similar to src/components, this directory is a standard practice but not necessary.

**The src/styles section:**

Although it is customary, it is not necessary to place your CSS or Sass files in the src/styles directory. Astro will manage and optimize your styles as long as they are appropriately imported and located in the src/ directory.

**public/:**

Files and assets that do not need to be handled during the construction process for Astro are kept in the public/ directory. These files will be transferred unchanged to the build folder.

This behavior makes common assets like photos and fonts, as well as specialized files like robots.txt and manifest. web manifest, public/ideal.

You are able to put CSS and JavaScript in your public/ directory, but you should be aware that your final build will not bundle or optimize those items.
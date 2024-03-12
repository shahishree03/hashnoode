---
title: "Angular V16"
datePublished: Sun May 21 2023 08:15:07 GMT+0000 (Coordinated Universal Time)
cuid: clhx5852j000308jjfruj2b3j
slug: angular-v16
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1684655881538/0fbf294e-b88c-4617-b5e7-3454102a988f.png
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1684656866460/47f5cb88-6793-4128-8f62-cd8516241514.png

---

The Signal pattern is in place since the beginning in the Solid Js library and is based on the push/pull pattern.

As the name suggests, pull allows you to retrieve the value and push allows you to set a new one or to mutate it.

Anyway a signal always has a value and the retrieval of this value is always done synchronously.

In version 16 of Angular, the pattern base API will be integrated and will allow to get more performance in the way Angular handles change detection.

### Feature highlights in Angular v16

Feature highlights in Angular v16.

Faster builds with the esbuild developer preview.

Standalone component migration and scaffolding.

Required inputs.

Highlighted breaking changes in Angular v16.

Angular v16 requires node.js version v16 or v18.

Angular v16 requires TypeScript version 4.9 or later.

### Angular Signals developer preview

This release includes the first developer preview of Angular's new reactivity primitives: signal, computed, and effect. See the signals guide for details and the Angular Signals RFC for more background.

### Enhanced hydration developer preview

Previously, when Angular bootstrapped on a page that was server-side rendered or compile-time pre-rendered, the framework would discard any existing DOM nodes and re-render from scratch. With v16's enhanced hydration support, you can opt into Angular reusing these existing DOM nodes. This developer preview feature can improve page load performance in many scenarios. See the full hydration guide for details.

### Faster builds with the esbuild developer preview

v16 brings you the developer preview of Angular CLI's new builders based on esbuild. This new architecture can significantly improve build times in many scenarios. This preview additionally includes integration with Vite powering the CLI's development server.

### Standalone component migration and scaffolding

To support developers transitioning their apps to standalone APIs, Angular v16 includes migration schematics and a standalone migration guide. These tools dramatically reduce the effort required to move your code to standalone components, directives, and pipes. Visit the standalone migration guide for details.

The Angular v16, has joined the Angular revolution with its latest improvements and updates making it even better and more efficient for the developer community and tech enthusiasts. This Angular version has addressed dozens of quality-of-life improvements across feature requests, with a combined total of over 2500 thumbs up on GitHub. Let’s take a closer look at what the latest version of Angular v16.
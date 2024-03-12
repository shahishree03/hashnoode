---
title: "Angular V15"
datePublished: Mon Nov 21 2022 16:59:03 GMT+0000 (Coordinated Universal Time)
cuid: clar18qbl001h08l1cw7q5dmk
slug: angular-v15
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1669048744546/3YAYdLUyS.png

---

The most recent iteration of the TypeScript-based web application framework created by Google is called** Angular 15**. The release includes "standalone" APIs that are now stable and enable developers to create apps without utilising NgModules.

On November 16, Angular 15 was revealed in public. The standalone APIs allow programmers to start an application using just one component and were released as a developer preview in Angular 14 in June. They function in router, Angular Elements, HttpClient, and other places. NgModules, a method of handling dependencies that developers considered as needlessly complicated, are being replaced with standalone components in an effort to streamline development.
A new directive composition API in Angular 15 also aims to increase code reuse. Developers may utilise directives to enhance host components, and Angular is integrated with a code reuse method.

The addition of a new image directive, which is now stable, offers capabilities like automated srcset creation, which guarantees a correctly sized picture, and experimental fill mode, which causes an image to fill its parent container and eliminates the need to express the image's height and width. Direct usage of the independent NgOptimizedImage in a component or NgModule is possible.

Before moving to the features of the angular V15 let us see what actually Angular is 

Angular is a development platform, built on TypeScript. As a platform, Angular includes:
1.   A component-based framework for building scalable web applications
2.  A collection of well-integrated libraries that cover a wide variety of features, including routing, forms management, client-server communication, and more
3.  A suite of developer tools to help you develop, build, test, and update your code

With Angular, you're taking advantage of a platform that can scale from single-developer projects to enterprise-level applications. Angular is designed to make updating as straightforward as possible, so take advantage of the latest developments with minimal effort. Best of all, the Angular ecosystem consists of a diverse group of over 1.7 million developers, library authors, and content creators.

**Angular applications: The essentials**

This section explains the core ideas behind Angular. Understanding these ideas can help you design and build your applications more effectively.

**Components**

Components are the building blocks that compose an application. A component includes a TypeScript class with a @Component() decorator, an HTML template, and styles. The @Component() decorator specifies the following Angular-specific information:

A CSS selector that defines how the component is used in a template. HTML elements in your template that match this selector become instances of the component.

An HTML template that instructs Angular how to render the component

An optional set of CSS styles that define the appearance of the template's HTML elements

The following is a minimal Angular component.


```
content_copy
import { Component } from '@angular/core';

@Component({
  selector: 'hello-world',
  template: `
    <h2>Hello World</h2>
    <p>This is my first component!</p>
  `
})
export class HelloWorldComponent {
  // The code in this class drives the component's behavior.
}
``` 
**
Templates**

Every component has an HTML template that declares how that component renders. You define this template either inline or by file path.

Angular adds syntax elements that extend HTML so you can insert dynamic values from your component. Angular automatically updates the rendered DOM when your component's state changes. One application of this feature is inserting dynamic text, as shown in the following example.

The value for message comes from the component class:

```
content_copy
import { Component } from '@angular/core';

@Component ({
  selector: 'hello-world-interpolation',
  templateUrl: './hello-world-interpolation.component.html'
})
export class HelloWorldInterpolationComponent {
    message = 'Hello, World!';
}
``` 

Angular 15 also includes the following features and enhancements:

1. Stack traces are more helpful, Angular v15 makes debugging Angular applications easier with cleaner stack traces. Angular worked with Google Chrome developers to present stack traces that show more of your application's code and less from the libraries it calls.
2. Material Design Components for Web (MDC), now stable. Many of the components in Angular Material v15 have been refactored to be based on Angular Material Design Components (MDC) for the Web. The refactored components offer improved accessibility and adherence to the Material Design spec.
3. Range selection support in the slider and a density customization API for components.
4. Component Dev Kit (CDK) adds a CDK listbox primitive.
5. Improvements to the experimental support for the ESbuild JavaScript bundler, with experimental backing for Sass, SVG template, file replacement, and ng – watch.
6. The Angular CLI lets you generate a new standalone component, via ng g component –- standalone. And the output of ng new has been simplified, removing test.ts, polyfills.ts, and environments to reduce the configuration.
7. Developers can globally change the default formatting configuration for DatePipe.
8. The language service now can automatically import components being used on a template but that have not been added to a standalone component or NgModule.
9. Adding NgOptimizedImage directive to your component or NgModule can help reduce the download time of images in your Angular application. For more information about using the NgOptimizedImage directive, see Getting started with NgOptimizedImage.
10. A preview of dependency injection debugging in Angular DevTools.
11. Simplified Angular CLI output for ng new, for creating a new Angular workspace.
12. Improved debugging in Zone.js, for async stack traces with the new async stack tagging API developed in conjunction with the Chrome DevTools team.

In other Angular news, the project’s developers have decided to deprecate the Protractor testing framework, based on community feedback. Plans were detailed in a blog post on August 10. A long-term support option will be sought for those wishing to continue using Protractor for active projects. The last version of Protractor is expected in Angular 16, due in the summer of 2023. Angular 12 previously added support for testing frameworks including Cypress, Nightwatch, and WebdriverIO. 
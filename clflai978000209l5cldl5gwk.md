---
title: "What is Flask in Python-"
datePublished: Thu Mar 23 2023 15:50:18 GMT+0000 (Coordinated Universal Time)
cuid: clflai978000209l5cldl5gwk
slug: what-is-flask-in-python
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1679583353413/875068ba-3b14-4515-9e2d-f92a7ed4e554.webp
tags: python, apis, flask, wed-development

---

Flask is a web application framework written in Python. It was developed by Armin Ronacher, who led a team of international Python enthusiasts called Poocco. Flask is based on the Werkzeg WSGI (Web Server Gateway Interface) toolkit and the Jinja2 template engine. Both are Pocco projects. It’s a Python module that lets you develop web applications quickly. It has a small and easy-to-extend core: a microframework that doesn’t include an ORM (Object Relational Manager) or features.

It does have many cool features like URL routing, and a template engine. It is a WSGI web app framework.

It is designed to make getting started quick and easy, with the ability to scale up to complex applications. It began as a simple wrapper around Werkzeug and Jinja and has become one of the most popular Python web application frameworks. Flask offers suggestions but doesn't enforce any dependencies or project layouts. It is up to the developer to choose the tools and libraries they want to use. The community provides many extensions that make adding new functionality.

## **Installation of Flask**

#### **Python Version**

Install the latest version of Python or at least use a version &gt;= Python 3.7

#### **Creating Virtual Environment**

Virtual environments are separate collections of Python libraries, one for each project. Installed packages for one project do not affect other projects or the operating system’s packages. Python has the venv package, which allows you to build virtual environments.

#### **For Windows**

```typescript
> mkdir myproject
> cd myproject
> py -3 -m venv venv
```

#### **For Mac**

```typescript
$ mkdir myproject
$ cd myproject
$ python3 -m venv venv
```

#### **Make the Environment Active**

Before you begin working on your project, turn on the environment-

#### **For Windows**

```typescript
> venvScriptsactivate
```

#### **For Mac**

```typescript
$ . venv/bin/activate
```

The name of the current active environment will be shown in your shell prompt.

#### **Install Flask**

Run the following command in the active environment to install Flask:

```typescript
$ pip install Flask
```

The flask run command is capable of doing more than simply starting the development server. When we enable debug mode, the server will immediately reload if the code changes and an interactive debugger will appear in the browser if an error occurs during a request.

### Debug Mode-

A **Flask** application is started by calling the **run()** method. However, while the application is under development, it should be restarted manually for each change in the code. To avoid this inconvenience, enable **debug support**. The server will then reload itself if the code changes. It will also provide a useful debugger to track the errors if any, in the application.

The **Debug** mode is enabled by setting the **debug** property of the **application** object to **True** before running or passing the debug parameter to the **run()** method.

```typescript
app.debug = True
app.run()
app.run(debug = True)
```

# **Flask – Routing**

Modern web frameworks use the routing technique to help a user remember application URLs. It is useful to access the desired page directly without having to navigate from the home page.

The **route()** decorator in Flask is used to bind the URL to a function. For example −

```typescript
@app.route(‘/hello’)
def hello_world():
   return ‘hello world’
```

Here, the URL **‘/hello’** rule is bound to the **hello\_world()** function. As a result, if a user visits [**http://localhost:5000/hello**](http://localhost:5000/hello) URL, the output of the **hello\_world()** function will be rendered in the browser.

The **add\_url\_rule()** function of an application object is also available to bind a URL with a function as, in the above example, **route()** is used.

A decorator’s purpose is also served by the following representation −

```typescript
def hello_world():
   return ‘hello world’
app.add_url_rule(‘/’, ‘hello’, hello_world)
```

## Advantages and disadvantages of Flask

### Advantages of Flask

#### Scalable-

Size is everything, and Flask’s status as a microframework means that you can use it to grow a tech project such as a web app incredibly quickly. If you want to make an app that starts small, but has the potential to grow quickly and in directions you haven’t completely worked out yet, then it’s an ideal choice. Its simplicity of use and few dependencies enable it to run smoothly even as it scales up and up.

#### Flexible-

This is the core feature of Flask, and one of its biggest advantages. To paraphrase one of the principles of the [**Zen of Python**](https://www.python.org/dev/peps/pep-0020/#the-zen-of-python), simplicity is better than complexity because it can be easily rearranged and moved around. The minimal nature of Flask and its aptitude for developing smaller web apps means that it’s even more flexible than Django itself.

#### Easy to negotiate-

Like Django, being able to find your way around easily is key for allowing web developers to concentrate on just coding quickly, without getting bogged down. At its core, the microframework is easy to understand for web developers, not just saving them time and effort but also giving them more control over their code and what is possible.

#### Lightweight-

When we use this term about a tool or framework, we’re talking about its design of it—a few constituent parts need to be assembled and reassembled, and it doesn’t rely on a large number of extensions to function. This design gives web developers a certain level of control.

### Disadvantages of Flask

#### Not a lot of tools-

Inevitably there are some downsides to this microframework’s lightweight nature. Chief among them is that, unlike Django, Flask lacks a large toolbox. This means that developers will have to manually add extensions such as libraries. And, if you add a huge number of extensions, it may start to slow down the app itself due to a multitude of requests.

#### Difficult to get familiar with a larger Flask app-

Because the development of a web app using Flask can take a variety of twists and turns, a web developer arriving at the project mid-way through can struggle to come to terms with how it’s been designed. The modular nature of the micro-framework that we mentioned earlier can come back to haunt coders, who will have to familiarize themselves with each constituent part.

#### Maintenance costs-

Because it is so versatile in terms of which technologies it can interface with, quite often a company using Flask will incur extra costs of supporting those technologies. For example, if a technology interfacing with your Flask app becomes obsolete or is discontinued, then the company will have to scramble to find a new compatible one. The more complicated the app becomes, the higher the potential maintenance and implementation costs.

### Conclusion-

Flask also supports modular programming, which is where its functionality can be split into several interchangeable modules. Each module acts as an independent building block, which can execute one part of the functionality. Together this means that the whole constituent parts of the structure are flexible, moveable, and testable on their own.

Flask users will find a healthy number of examples and tips arranged in a structured manner. This encourages developers to use the framework, as they can easily get introduced to the different aspects and capabilities of the tool.
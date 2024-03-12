---
title: "An overview of Spring Boot"
datePublished: Tue Feb 07 2023 14:46:05 GMT+0000 (Coordinated Universal Time)
cuid: clducu6ov000909l08putgveu
slug: an-overview-of-spring-boot
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1675780786916/1e80251f-be63-4a6b-b647-1881e68cf653.jpeg
tags: java-framework, springboot, spring-framework

---

Spring Boot is an open-source Java-based framework used to create a micro-Service. It is developed by Pivotal Team and is used to build stand-alone and production-ready spring applications. MicroService is an architecture that allows developers to develop and deploy services independently.

### **What is Spring Boot?**

Spring Boot is a project that is built on top of the Spring Framework. It provides an easier and faster way to

It is a Spring module that provides the **RAD (*Rapid Application Development*)** feature to the Spring Framework. It is used to create a stand-alone Spring-based application that you can just run because it needs minimal Spring configuration.

Spring boot is a combination of spring framework, embedded HTTP servers and XML&lt;bean&gt; configuration or @configuration.

In short, Spring Boot is the combination of **Spring Framework** and **Embedded Servers**.

In Spring Boot, there is no requirement for XML configuration (deployment descriptor). It uses convention over configuration software design paradigm which means it decreases the effort of the developer.

We can use Spring **STS IDE** or **Spring Initializer** to develop Spring Boot Java applications.

### **Why should we use Spring Boot Framework?**

We should use Spring Boot Framework because:

* The dependency injection approach is used in Spring Boot.
    
* It contains powerful database transaction management capabilities.
    
* It simplifies integration with other Java frameworks like JPA/Hibernate ORM, Struts, etc.
    
* It reduces the cost and development time of the application.
    

Spring Boot Framework has Spring sister projects which help to build applications addressing modern business needs. There are the following Spring sister projects are as follows:

* **Spring Data:** It simplifies data access from the relational and **NoSQL** databases.
    
* **Spring Batch:** It provides powerful **batch** processing.
    
* **Spring Security:** It is a security framework that provides robust **security** to applications.
    
* **Spring Social:** It supports integration with **social networking** like LinkedIn.
    
* **Spring Integration:** It is an implementation of Enterprise Integration Patterns. It facilitates integration with other **enterprise applications** using lightweight messaging and declarative adapters.
    

### **Advantages of Spring Boot**

* It creates **stand-alone** Spring applications that can be started using Java **\-jar**.
    
* It tests web applications easily with the help of different **Embedded** HTTP servers such as **Tomcat, Jetty,** etc.
    
* It provides '**starter**' POMs to simplify our Maven configuration.
    
* It provides **production-ready** features such as **metrics, health checks,** and **externalized configuration**.
    
* There is no requirement for **XML** configuration.
    
* It offers a **CLI** tool for developing and testing the Spring Boot application.
    
* It also reduces writing multiple **boilerplate codes** (the code that has to be included in many places with little or no alteration), XML configuration, and annotations.
    
* It **increases productivity** and reduces development time.
    

### **The disadvantage of Spring Boot**

Spring Boot uses dependencies that are not going to be used in the application. These dependencies increase the size of the application.

### **Goals of Spring Boot**

The main goal of Spring Boot is to reduce **development, unit test,** and **integration test** time.

* Provides Opinionated Development approach
    
* Avoids defining more Annotation Configuration
    
* Avoids writing lots of import statements.
    

By providing or avoiding the above points, Spring Boot Framework reduces **Development time, and effort,** and **increases productivity**.

### **Spring Boot Features contains the following**

* Web Development
    
* Spring Application
    
* Application events and listeners
    
* Admin features
    
* Externalized Configuration
    
* Properties Files
    
* YAML Support
    
* Type-safe Configuration
    
* Logging
    
* Security
    

**Web Development**

It is a well-suited Spring module for web application development where we can easily create a self-contained HTTP application that uses embedded servers like **Tomcat, Jetty,** or Undertow. We can use the **spring-boot-starter-web** module to start and run the application faster.

**Spring Application**

The SpringApplication is a class that provides a convenient way to bootstrap a Spring application. It can be started from the main method. We can call the application just by calling a static run() method.

```java
public static void main(String[] args)  
{    
SpringApplication.run(ClassName.class, args);    
}  
```

**Application Events and Listeners**

Spring Boot uses events to handle a variety of tasks. It allows us to create factories file that is used to add listeners. We can refer it to using the **ApplicationListener key**.

Always create factories files in META-INF folder like **META-INF/spring.factories**.

**Admin Support**

Spring Boot provides the facility to enable admin-related features for the application. It is used to access and manage applications remotely. It can enable in the Spring Boot application by using **spring.application.admin.enabled** property.

**Externalized Configuration**

Spring Boot allows developers to externalize their configuration so that developers can work with the same application in different environments. The application uses YAML files to externalize configuration.

**Properties Files**

Spring Boot provides a rich set of **Application Properties**. The properties file is used to set properties like **server-port =8082** and many others. It helps to organize application properties.

**YAML Support**

It provides a convenient way of specifying the hierarchical configuration. It is a superset of JSON. The SpringApplication class automatically supports YAML. It is an alternative of the properties file.

**Type-safe Configuration**

A strong type-safe configuration is provided to govern and validate the configuration of the application. Application configuration is always a risky task that should be typed safely. We can use the annotation provided by this library.

**Logging**

Spring Boot uses Common logging for all internal logging. Logging dependencies are managed by default. We should not change logging dependencies if no customization is needed.

**Security**

Spring Boot applications are spring-based web applications. So, it is secure by default with basic authentication on all HTTP endpoints. A rich set of Endpoints is available to develop a secure Spring Boot application.

So readers today we learned about Spring Boot -what it is ? why should we learn it?

See you in the next blog. Happy learning.
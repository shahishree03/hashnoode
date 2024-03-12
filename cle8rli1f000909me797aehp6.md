---
title: "Threads ! Threading in Java"
datePublished: Fri Feb 17 2023 16:48:00 GMT+0000 (Coordinated Universal Time)
cuid: cle8rli1f000909me797aehp6
slug: threads-threading-in-java
cover: https://cdn.hashnode.com/res/hashnode/image/stock/unsplash/hTeYcjviZ-s/upload/1bb9de1efe45ec83ac191fd1829e4294.jpeg
tags: programming-blogs, java, threading

---

we can define threads as the smallest unit of a process with lightweight and has separate paths of execution. These threads use shared memory but they act independently hence if there is an exception in threads that do not affect the working of other threads despite them sharing the same memory.

A thread runs inside the process; a process can have multiple threads that run simultaneously. The Multithreading concept is popularly applied in games, animation…etc.

### **What is multitasking?**

Operating System provides the facility, where users can perform multiple actions simultaneously on the machine. This Multitasking can be achieved in two ways: 

1. **Process-Based Multitasking** 
    
2. **Thread-Based Multitasking** 
    

**Process-Based Multitasking (Multiprocessing)**

In this type of Multitasking, processes are heavyweight and each process was allocated by a separate memory area. And as the process is heavyweight the cost of communication between processes is high and it takes a long time for switching between processes as it involves actions such as loading, saving in registers, updating maps, lists, etc. 

**Thread-Based Multitasking(Multithreading)** 

As we discussed above Threads are provided with lightweight nature and share the same address space, and the cost of communication between threads is also low. 

### **Why Threads are used?** 

Now, we can understand why threads are being used as they had the advantage of being lightweight and can provide communication between multiple threads at a Low Cost.

### **Life Cycle Of Thread**

There are different states a Thread transfers into during its lifetime, namely: 

1. New State
    
2. Active State
    
3. Waiting/Blocked State
    
4. Terminated State
    

**New State** 

By default, a Thread will be in a new state.

**Active State**

A Thread in a new state by default gets transferred to an Active state when it invokes the start() method, his Active state contains two sub-states namely:

* **Runnable State:** In This State, The Thread is ready to run and it’s the job of the Thread Scheduler to provide the thread time for the runnable state preserved threads. A program with Multithreading shares slices of time intervals which are shared between threads hence, these threads run for some short period and wait in the runnable state to get their schedules slice of a time interval.
    
* **Running State:** When The Thread Receives CPU allocated by Thread Scheduler, it transfers from the “Runnable” state to the “Running” state. and after the expiry of its given time slice session, it again moves back to the “Runnable” state and waits for its next time slice.
    

**Waiting/Blocked State** 

If a Thread is inactive but on a temporary time, then either it is in a waiting or blocked state.In this state, the thread waits for some I/O completion. When we call sleep() method or wait() it goes to waiting/blocked state from running state.

**Terminated State**

A thread will be in Terminated State, due to the below reasons: 

* Termination is achieved by a Thread when it finishes its task Normally.
    
* Sometimes Threads may be terminated due to unusual events like segmentation faults, exceptions…etc. and such kind of Termination can be called Abnormal Termination.
    
* A terminated Thread means it is dead and no longer available
    

### **What is Main Thread?** 

As we create Main Method in every Java Program, which acts as an entry point for the code to get executed by JVM, Similarly in this Multithreading Concept, Each Program has one Main Thread which was provided by default by JVM, hence whenever a program is being created in java, JVM provides the Main Thread for its Execution

### **How to Create Threads using Java ?** 

We can create Threads in java using two ways : 

1. By extending Thread Class
    
2. Implementing a Runnable interface
    

**1\. By Extending Thread Class** 

We can run Threads in Java by using Thread Class, which provides constructors and methods for creating and performing operations on a Thread, which extends a Thread class that can implement Runnable Interface. We use the following constructors for creating the Thread: 

* Thread
    
* Thread(Runnable r)
    
* Thread(String name)
    
* Thread(Runnable r, String name)
    

```java
import java.io.*;
import java.util.*;
public class ThreadDemo extends Thread {
  // initiated run method for Thread
     public void run()
    {
      System.out.println("Thread Started Running...");
    }
    public static void main(String[] args)
    {
        ThreadDemo t1 = new ThreadDemo();
        // invoking Thread
        t1.run();
    }
 }
```

Output:

`Thread Started Running...`

 Sample code to create Thread by using Runnable Interface:

```java
import java.io.*;
import java.util.*;
public class ThreadDemo implements Runnable {
    // method to start Thread
    public void run()
    {
        System.out.println("Thread is Running Successfully");

    }
      public static void main(String[] args)
    {
      ThreadDemo  t1 = new ThreadDemo ();
        // initializing Thread Object
        Thread th1 = new Thread(t1);
        th1.run();
    }
}
```

Output:

`Thread is Running Successfully`

Folks today this much only. We will meet in our next blog. Happy learning.
---
title: Threads
parent: Iteration 1
has_children: false
---

## Threads
When a process starts, the common language runtime automatically creates a single foreground thread to execute application code. Along with this main foreground thread, a process can create one or more threads to execute a portion of the program code associated with the process. These threads can execute either in the foreground or in the background.
> To begin execution it is called the **Start** method to begin.

We can also display information about thread properties, using the following comands:
> Thread.CurrentThread.**ManagedThreadId**
>
> Thread.CurrentThread.**ThreadState**
>
> Thread.CurrentThread.**Priority**

Background threads are identical to foreground threads with one exception: a background thread does not keep a process running if all foreground threads have terminated. Once all foreground threads have been stopped, the runtime stops all background threads and shuts down.
> To change a thread to execute in the background, it has to be set to **IsBackground**

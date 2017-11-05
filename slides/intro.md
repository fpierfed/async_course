# [Asynchronous Programming With Python](https://pythoncomputing.com/#section-training)
#### _Francesco Pierfederici_


## Home Page
 * Course: https://pythoncomputing.com/#section-training
 * Code: https://github.com/fpierfed/async_course


## Asynchronous Programming
* Python has great support for async programming
    * Since the end of the 90s
    * But especially since the early 2000s
* There are only few main ideas to keep in mind
    * Asynchronous/non-blocking functions return "immediately"
    * Synchronous/blocking ("normal") functions do not return until they are done
    * Use async programming especially when the CPU is idle most of the time
    * Write code in a way that does not block (see collaborative multitasking)
    * Everything happens in a single thread (most of the time)
        * We get concurrency (i.e., several pieces of code "alive" at the same time)
        * We do not get parallelism  (i.e., only one piece of code runs at any given point in time)
        * We do not need locks etc. if we are careful
        * We do need an event loop/scheduler
    * We need a way to know when your async functions are done
        * Futures and callbacks

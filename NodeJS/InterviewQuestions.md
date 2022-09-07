# Q. What is Node js?

Node.js is an open-source server side runtime environment built on Chrome's V8 JavaScript engine. It provides an event driven, non-blocking (asynchronous) I/O and cross-platform runtime environment for building highly scalable server-side applications using JavaScript.

# Q. How NodeJS works?

# Q. Why is LIBUV needed in Node JS?
libuv is a C library originally written for Node.js to abstract non-blocking I/O operations. It provide the below features

* It allows the CPU and other resources to be used simultaneously while still performing I/O operations, thereby resulting in efficient use of resources and network.

* It facilitates an event-driven approach wherein I/O and other activities are performed using callback-based notifications.

* It provides mechanisms to handle file system, DNS, network, child processes, pipes, signal handling, polling and streaming

* It also includes a thread pool for offloading work for some things that can't be done asynchronously at the operating system level.

# Q. How to achieve multi-threading in node js?

Node.js runs JavaScript code in a single thread, which means that your code can only do one task at a time.However, Node.js itself is multithreaded and provides hidden threads through the libuv library, which handles I/O operations like reading files from a disk or network requests. Through the use of hidden threads, Node.js provides asynchronous methods that allow your code to make I/O requests without blocking the main thread.

Node.js introduced the worker-threads module, which allows you to create threads and execute multiple JavaScript tasks in parallel. Once a thread finde and distribute a task to multiple workers to optimize it.


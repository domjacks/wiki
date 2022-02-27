# Engines & Runtimes

## Engines

There are a few popular JavaScript Engines.  

The engine is responsible for parsing, compiling, optimising and then executing your JavaScript code.  

We often say JavaScript is an interpreted language. But it is way more complex than that these days.  

It is comprised of 2 main components: 
* Memory Heap
* Call Stack

Popular engines:
* V8 – Chromium
* SpiderMonkey – Mozilla
* JavaScriptCore - WebKit

## Runtimes

In order for JavaScript to be useful, it needs more than just an engine.  

The runtime is the collection of things needed to make useful JavaScript applications.  

These runtimes differ depending on the target. So for example, the browser provides a different runtime to the server. 

Browsers, Node, Deno etc. all provide their own runtimes made up of different things.  

### Browser runtime
* Engine
* Web APIs
* Callback Queue
* Event Loop

### Node.js
* Engine
* C++ Bindings
* Thread Pool
* Callback Queue
* Event Loop
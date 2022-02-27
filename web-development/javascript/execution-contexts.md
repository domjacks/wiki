# Execution Contexts

Execution contexts are where your code is actually run in the engine.

## Contents

When a new EC is created as part of the "creation phase", the following is made available:

### Variable Environment

The things that are declared in the execution context:
  * `let`, `const`, `var` declarations
  * Functions
  * Arguments object

### Scope Chain

Each EC gets the whole scope chain needed for it to be able to run all the code inside.

It can be thought of as all the variable environments of all the parents scopes added together.

See [Scope Chain](web-development/javascript/scope-chain) for more info.

### `this`

See [the 'this' keyword](web-development/javascript/this) for more info.

## Types of EC
### Global EC

The global EC is where the top level code is executed.  

Expressions and declarations at the top level are executed here.  

Note, although functions can be declared in the global EC, the function body is not executed here.  

### Function EC

Each function gets its own EC. 

## Call Stack 

A stack of Execution Contexts.  

This is how an engine keeps track of what code it is executing. This is especially important because JavaScript is single-threaded. 
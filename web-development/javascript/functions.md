# Functions

Functions are one of the basic building blocks of JavaScript and allow us to reuse functionality across our code. 

## Creating functions
### Declarations

A function declaration uses the `function` keyword to declare a function signature. 

Function declarations in JavaScript are hoisted. See [Hoisting & TDZ](./hoisting-and-tdz.md) for more info. 

e.g.

```javascript
function printHelloWorld() { 
    console.log("Hello, world!") 
} 
```

### Expressions

A function expression is when you declare a variable and assign it to an anonymous function.

Function expressions are not hoisted. See [Hoisting & TDZ](./hoisting-and-tdz.md) for more info.

e.g.

```javascript
const printHelloWorld = function () { 
    console.log("Hello, world!") 
} 
```

#### Arrow Functions

Arrow functions are a type of function expression which do not have their own `this` keyword or `arguments` in their execution context. See [Execution Contexts](./execution-contexts.md) for more info.

e.g.

```javascript
function test() { 
  this.hello = 'hello' 

  function sayHello() {  
    console.log(this.hello) // Oops, hello isn't defined on this functions 'this' 
  } 

  // However the arrow function references the outer 'this' 
  const sayHello2() = () => console.log(this.hello) 
}  
```

## First Class Functions
Functions in Javascript are known as first-class. This means they can be passed into, and returned from other functions. 

e.g.

TODO

## Closures

JavaScript supports closures, meaning inner functions can reference variables and functions from their outer functions. However outer functions cannot reach into things declared inside inner functions. 

e.g.

TODO

## Parameters vs. Arguments

**Parameters** are declared in the function signature.

e.g.

```javascript
function add(x, y) { ... }
```
In this example, `x` and `y` are the parameters. 

**Arguments** are the values passed into the function at the point it is executed. 

e.g.


```javascript
add(2, 3) // 5
```

In this example, `2` and `3` are the arguments.


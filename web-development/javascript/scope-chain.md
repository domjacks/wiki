# Scope Chain

Scoping controls how our variables are organised and accessed. 

JavaScript uses something called *Lexical Scoping* to determine where variables can be accessed from. Lexical scoping is controlled by the placement of functions and blocks in the code.

A Scope refers to the place that a certain variable is declared.

A variables' scope is where a variable can be accessed. There's a subtle difference here in that the scope in which a variable is declared is not the same as the scope it can be accessed. 

When a variable is not in the current scope, it will look up the scope chain until it finds what it is looking for. This is called *variable lookup*.

## Types of Scopes

### Global

Top level code outside function or block. 

The variables declared here are accessible anywhere.

### Function

Variables are only accessible inside the function. This can also be known as 'local scope'.

e.g.

```javascript
function helloWorld() {
    const str = 'Hello, world!'
    console.log(str) // Hello, world!
}

console.log(str) // ReferenceError
```

### Block

Blocks are any time the curly braces are used `{}`. 

Variables declared inside a block are only accessible inside the block.

This only applies to variables declared using `let` and `const`. We call them *block scoped*.

e.g.

```javascript
const myNum = 5

if (myNum === 5 ) {
    var isIncorrect = false
    const isCorrect = true
}

console.log(isIncorrect) // false
console.log(isCorrect) // ReferenceError
```

Functions are also *block scoped* when in `strict` mode.

## The Scope Chain

The scope chain simply refers to the relationships between functions and blocks within your code that indfluence the scope a variable can be accessed in. 

e.g.

```javascript
const name = 'Dom'

function logName() {
    const greeting = 'Hello'
    function print() {
        const str = `${greeting}, ${name}`
        console.log(str) // Hello, Dom
    }
    print()
    console.log(str) // ReferenceError
}

console.log(greeting) // ReferenceError
```
In the example above, you can see the chain of scope as inner functions can reference variables in their outer functions. 

So the `print()` function can reference it's parents variable of `greeting` as well as the global scope variable of `name`.

However, the global scope cannot access the `greeting` variable that was declared within the scope of the `log` function. And the `log` function scope cannot access the `str` variable that was declared in the `print` function scope.


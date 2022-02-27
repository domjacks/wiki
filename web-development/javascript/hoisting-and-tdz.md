# Hoisting & TDZ

## Hoisting
Pulls your `function` and `var` declarations into either the global scope to be used anywhere in the window, or to the top of your function/block scope to be used anywhere in the function. 

`var`s when hoisted are defined with a value of `undefined` until assigned. 

For `function`s, only the declaration is hoisted, not the expression.

e.g.

```javascript
funcDeclaration(); // prints "hello" 

function funcDeclaration () {
    console.log('hello')
} 

funcExpression(); // TypeError: expression is not a function 

const funcExpression = function () {
    console.log('hello')
} 
```

## Temporal Dead Zone (TDZ)

`let`/`const` declarations are still hoisted to the top of the scope it is in. 

However, `let`/`const` aren't actually defined with any value (`null`) until the definition is reached in your code. So everything above the definition is known as the temporal deadzone for that variable. 

If you try and reference the `let`/`const` you will get a `ReferenceError` 
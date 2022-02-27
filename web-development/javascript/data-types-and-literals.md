# Data Types & Literals

## Data Types

JavaScript is a dynamically and loosely typed language. This means the type of a variable is known only at run-time, and it does not require you to specify the type of a variable when it is declared.

### Primitives

Primitives are one half of the data types. They are the only data types that can be immutable.

* String, Number, BigInt, Boolean, `null`, `undefined`, Symbol

### Object

The second half of the data types are objects. Objects are a fundamental building block of JavaScript.

See [Object](./object.md) for more info.

## Literals

Literals represent the actual values. Variables have types, _values_ are literals. 

* Array, Floating-point, Numeric, String, Object, RegExp, Boolean
* Template Literals


## Type conversion & coercion

You can manually convert a data type from one to another. e.g.

```javascript
const myString = "4" // "4" 

const myNumber = Number(myString) // 4 
```

Alternatively, JavaScript will try and coerce the value into the right type. 

We see this when concatenating two strings using the `+` operator on strings. 

e.g.

```javascript
const myString = 'Hello' + ', world!' // Hello, world!
```

JavaScript understands that the two values are String literals and thus uses the `+` operator to concatenate into one String.

Subtly changing the example above shows how JavaScript coerces the value differently.

e.g.

```javascript
const myNumber = '12' / 6 // 2
```
# Objects

Pretty much everything in Javascript is an object. Including functions and all the data structures. The only things that aren't objects are the primitive data types as mentioned previously.

The order of the elements in an object are unstructured/unordered. 

## Creating objects

There are 4 ways to create an object: Object literal, `Object.create()`, function constructor, `class`.

### Object Literal

e.g.

```javascript
const myObject = { 
  firstName: "Dom", 
  lastName: "Jackson" 
} 
```

### Object.create(proto)

You can use the `Object` data type to create new objects. It has a method on it called `create` which can be passed a `prototype` object. 

See [Object-oriented JavaScript](oop-javascript.md) for more info on `prototype`s.

## Property Access

### Dot notation

e.g.

```javascript
const prop = myObject.firstName // // 'Dom'
```

### Bracket notation

You can also access a property using bracket notation which has the added benefit of allowing you to pass in an expression.  

e.g.

```javascript
const prop = myObject['first' + 'Name'] // 'Dom'
const prop2 = myObject['lastName'] // 'Jackson'
```


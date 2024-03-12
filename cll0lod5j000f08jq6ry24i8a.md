---
title: "ECMAScript  - (ES10) VS  (ES11)"
seoTitle: "ES 10 vs ES 11"
seoDescription: "Here are the features introduced in ES10 and ES11"
datePublished: Mon Aug 07 2023 08:18:03 GMT+0000 (Coordinated Universal Time)
cuid: cll0lod5j000f08jq6ry24i8a
slug: ecmascript-es10-vs-es11
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1691396132887/bc8be616-4fbe-41f6-b5e2-c9ef6dabe7d7.png
tags: tutorial, javascript, technology, google, es6

---

Here are the features introduced in ES10 and ES11 :

### ECMAScript 2019 (ES10):

**1\.** `Array.prototype.flat()`: Flattens nested arrays to a specified depth.

```javascript
const nestedArray = [1, [2, [3, [4]]]];
const flattenedArray = nestedArray.flat(2);
console.log(flattenedArray); // Output: [1, 2, 3, [4]]
```

**2\.** `Array.prototype.flatMap()`: Maps and flattens array elements.

```javascript
const arr = [1, 2, 3];
const mappedAndFlattened = arr.flatMap(x => [x * 2]);
console.log(mappedAndFlattened); // Output: [2, 4, 6]
```

**3\.** `String.prototype.trimStart()`: Removes leading whitespace from a string.

```javascript
const str = "   Hello, world!   ";
const trimmedStr = str.trimStart();
console.log(trimmedStr); // Output: "Hello, world!   "
```

**4\.** `String.prototype.trimEnd()`: Removes trailing whitespace from a string.

```javascript
const str = "   Hello, world!   ";
const trimmedStr = str.trimEnd();
console.log(trimmedStr); // Output: "   Hello, world!"
```

**5\.** `Function.prototype.toString()`: Allows access to function source code.

```javascript
function greet() {
  return "Hello!";
}
const greetSource = greet.toString();
console.log(greetSource); // Output: "function greet() { return \"Hello!\"; }"
```

**6\.** `Object.fromEntries()`: Creates an object from key-value pairs.

```javascript
const entries = [['a', 1], ['b', 2]];
const obj = Object.fromEntries(entries);
console.log(obj); // Output: { a: 1, b: 2 }
```

**7\.** `Symbol.prototype.description`: Provides a description for symbols.

```javascript
const mySymbol = Symbol('My Symbol');
console.log(mySymbol.description); // Output: "My Symbol"
```

**8\.** `try...catch` with optional binding: Simplified error handling with optional catch parameter.

```javascript
try {
  throw new Error('Oops!');
} catch {
  console.log('Error caught!');
}
// Output: "Error caught!"
```

### ECMAScript 2020 (ES11):

**1\.** `BigInt`: Data type for arbitrary precision integers.

```javascript
const bigIntValue = 9007199254740991n;
console.log(bigIntValue); // Output: 9007199254740991n
```

**2\.** `Optional Chaining`: Simplifies accessing nested properties.

```javascript
const user = {
  name: 'John',
  address: {
    city: 'New York'
  }
};
const city = user.address?.city;
console.log(city); // Output: "New York"
```

**3\.** `Nullish Coalescing Operator`: Provides a default value for nullish values.

```javascript
const value1 = null;
const value2 = "Hello, world!";
const result = value1 ?? value2;
console.log(result); // Output: "Hello, world!"
```

**4\.** `Promise.allSettled()`: Handles multiple promises, regardless of rejection or fulfillment.

```javascript
const promises = [
  fetch('/data'),
  fetch('/users'),
  fetch('/settings')
];
Promise.allSettled(promises).then(results => console.log(results));
```

**5\.** `String.prototype.matchAll()`: Returns an iterator of all regex matches.

```javascript
const regex = /\d+/g;
const str = '10 apples and 25 oranges';
const matches = [...str.matchAll(regex)];
console.log(matches);
```

**6\.** `globalThis`: A reference to the global this value.

```javascript
console.log(globalThis === window); // Output: true (in a browser environment)
```

**7\.** `import()`: Dynamically imports modules.

```javascript
const modulePath = './my-module.js';
import(modulePath).then(module => console.log(module));
```

<mark>Please refer to the official ECMAScript website (</mark>[<mark>https://tc39.es/</mark>](https://tc39.es/)<mark>) or the ECMAScript proposal repository (</mark>[<mark>https://github.com/tc39/proposals</mark>](https://github.com/tc39/proposals)<mark>).</mark>
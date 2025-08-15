# 📚 JavaScript Datatypes & ECMAScript Standards

JavaScript is a **loosely typed** or **dynamic** language, meaning variables are not directly associated with any particular data type.  
The type of a variable is determined by the value assigned to it.

---

## 🗂 Types of Data in JavaScript

JavaScript has **two main categories** of data types:

1. **Primitive Data Types** (Immutable)
2. **Non-Primitive (Reference) Data Types**

---

### 🔹 1. Primitive Data Types
These are **immutable** and stored directly in the variable.

| Data Type    | Description                                         | Example |
|--------------|-----------------------------------------------------|---------|
| `String`     | Sequence of characters                              | `"Hello World"` |
| `Number`     | Numeric values (integer or floating-point)          | `42`, `3.14` |
| `BigInt`     | Very large integers beyond `Number` limit            | `123456789012345678901234567890n` |
| `Boolean`    | Logical value: `true` or `false`                    | `true` |
| `Undefined`  | Variable declared but not assigned a value          | `let a;` |
| `Null`       | Represents intentional absence of any value         | `let b = null;` |
| `Symbol`     | Unique and immutable value used as object property key | `Symbol('id')` |

---

### 🔹 2. Non-Primitive (Reference) Data Types
These are **mutable** and stored as a reference in memory.

| Data Type   | Description                       | Example |
|-------------|-----------------------------------|---------|
| `Object`    | Collection of key-value pairs     | `{ name: "John", age: 30 }` |
| `Array`     | Ordered list of values            | `[1, 2, 3]` |
| `Function`  | Reusable block of code            | `function greet() {}` |
| `Date`      | Represents dates and times        | `new Date()` |

---

## 🧠 Checking Data Types
You can check the type of a value using the `typeof` operator.

```javascript
console.log(typeof "Hello");     // string
console.log(typeof 42);          // number
console.log(typeof null);        // object (JavaScript quirk)
console.log(typeof undefined);   // undefined
console.log(typeof Symbol("id")); // symbol
console.log(typeof {});          // object
console.log(typeof []);          // object
console.log(typeof function(){}); // function
```

## 📜 ECMAScript (ES) Standards

ECMAScript (ES) is the standard specification that JavaScript follows.
The official standard is maintained by ECMA International.

### History of ECMAScript Versions
| Version       | Year | Key Features                                                |
| ------------- | ---- | ----------------------------------------------------------- |
| ES1           | 1997 | First edition                                               |
| ES3           | 1999 | Regular expressions, try/catch                              |
| ES5           | 2009 | Strict mode, JSON support                                   |
| ES6 (ES2015)  | 2015 | `let`, `const`, arrow functions, template literals, classes |
| ES7 (ES2016)  | 2016 | `includes()`, exponentiation operator                       |
| ES8 (ES2017)  | 2017 | Async/await, Object.entries, Object.values                  |
| ES9 (ES2018)  | 2018 | Rest/spread properties, async iteration                     |
| ES10 (ES2019) | 2019 | Flat, flatMap, Object.fromEntries                           |
| ES11 (ES2020) | 2020 | Nullish coalescing, optional chaining                       |
| ES12 (ES2021) | 2021 | Logical assignment operators, String.replaceAll             |
| ES13 (ES2022) | 2022 | Top-level await, class fields                               |

### 💡 Summary
- JavaScript supports primitive and non-primitive types.
- typeof is used to check a value's type.
- ECMAScript defines the core JavaScript language features and updates.
- Modern JavaScript heavily relies on ES6+ features for cleaner and more efficient code.



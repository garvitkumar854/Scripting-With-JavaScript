## 🌟 Variables in JavaScript  

Variables in JavaScript are used to store **data values**. JavaScript provides three ways to declare variables:  

### 🔹 **1. Using `var` (Old way, Avoid using)**  
- Function-scoped.  
- Can be **redeclared** and **updated** within the same scope.  
- Does **not** support block scope.  

```js
var name = "Garvit";  
console.log(name);  // Output: Garvit  
```

### 🔹 **2. Using `let` (Modern way, Preferred for changeable values)**  
- Block-scoped (Limited to `{}` blocks).  
- Cannot be redeclared in the same scope.  

```js
let age = 20;  
age = 21;  // ✅ Allowed  
console.log(age);  // Output: 21  
```

### 🔹 **3. Using `const` (Preferred for constant values)**  
- Block-scoped.  
- Cannot be **reassigned**.  
- Must be **initialized** at declaration.  

```js
const PI = 3.14159;  
console.log(PI);  // Output: 3.14159  
// PI = 3.14; ❌ Error! Cannot reassign a constant.
```

### 🔹 **Best Practices**  
✅ Use `const` for values that won't change.  
✅ Use `let` for values that will change.  
❌ Avoid `var` (due to scope and hoisting issues).  

### 🔹 **Data Types in Variables**  
JavaScript variables can store different types of data:

```js
let str = "Hello";  // String  
let num = 42;  // Number  
let isJSFun = true;  // Boolean  
let arr = [1, 2, 3];  // Array  
let obj = { name: "Garvit", age: 20 };  // Object  
let unknown;  // Undefined  
```

### 🚀 **Summary Table**  

| Keyword | Scope | Can Reassign? | Can Redeclare? | Hoisting |
|---------|-------|--------------|--------------|----------|
| `var` | Function | ✅ Yes | ✅ Yes | ✅ Hoisted (but undefined) |
| `let` | Block | ✅ Yes | ❌ No | ❌ Not hoisted |
| `const` | Block | ❌ No | ❌ No | ❌ Not hoisted |


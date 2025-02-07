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

## 📝 Rules for Choosing Variable Names in JavaScript  

When naming variables in JavaScript, follow these rules:  

### ✅ **Allowed:**  
✔ Variable names can contain **letters, digits, underscores (`_`) and dollar signs (`$`)**.  
✔ Variable names **must begin with a letter, `_`, or `$`** (not a number).  
✔ JavaScript is **case-sensitive** (`name` and `Name` are different).  

```js
let userName = "Garvit";  // ✅ Valid  
let _count = 10;          // ✅ Valid  
let $price = 99.99;       // ✅ Valid  
```

### ❌ **Not Allowed:**  
✖ Variable names **cannot start with a number**.  
✖ Reserved **keywords** cannot be used as variable names.  
✖ No spaces or special characters (except `_` and `$`).  

```js
let 1name = "Error";  // ❌ Invalid  
let var = "Wrong";    // ❌ Invalid (reserved keyword)  
let user name = "No"; // ❌ Invalid (spaces not allowed)  
```

### 🌟 **Best Practices:**  
✅ Use **camelCase** (`firstName`, `totalAmount`).  
✅ Make variable names **meaningful & readable**.  
✅ Use **`const` for constants**, `let` for changeable values, and avoid `var`.  

```js
const MAX_USERS = 1000;  // ✅ Constant (all uppercase)  
let userAge = 25;        // ✅ Meaningful name  
```

### 🚀 **Summary Table**  

| Keyword | Scope | Can Reassign? | Can Redeclare? | Hoisting |
|---------|-------|--------------|--------------|----------|
| `var` | Function | ✅ Yes | ✅ Yes | ✅ Hoisted (but undefined) |
| `let` | Block | ✅ Yes | ❌ No | ❌ Not hoisted |
| `const` | Block | ❌ No | ❌ No | ❌ Not hoisted |


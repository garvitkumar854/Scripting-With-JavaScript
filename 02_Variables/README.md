# 📝 Variables in JavaScript  

Variables are **containers** for storing data values in JavaScript.  
They allow us to **store, change, and reuse** information in our programs.

---

## 📌 Declaring Variables  

JavaScript provides **three ways** to declare variables:  
- `var` – Old way (function-scoped)  
- `let` – Modern way (block-scoped)  
- `const` – Modern way for constants (block-scoped & cannot be reassigned)  

---

## 🔹 1. var  
- Introduced in **ES1 (1997)**.  
- **Function-scoped**: Accessible throughout the function in which it’s declared.  
- Can be **redeclared** and **updated**.  
- **Avoid using** in modern JavaScript due to scope-related issues.  

```javascript
var name = "John";
var name = "Doe"; // ✅ Redeclaration allowed
console.log(name); // Output: Doe
```

## 🔹 2. let
- Introduced in **ES6 (2015)**.
- **Block-scoped**: Only accessible inside the block `{}` where it’s declared.
- Can be updated, but not redeclared in the same scope.
- Preferred for variables whose values will change.

```javascript
let age = 25;
age = 26; // ✅ Update allowed
// let age = 30; ❌ Redeclaration not allowed
console.log(age); // Output: 26
```

## 🔹 3. const
- Introduced in **ES6 (2015)**.
- Block-scoped like `let`.
- Cannot be reassigned once a value is given.
- Must be initialized at the time of declaration.

```javascript
const PI = 3.14159;
// PI = 3.14; ❌ Error: Assignment to constant variable
console.log(PI); // Output: 3.14159
```

## Quick Comparison
| Feature         | var               | let                        | const                      |
| --------------- | ----------------- | -------------------------- | -------------------------- |
| Scope           | Function          | Block                      | Block                      |
| Redeclaration   | ✅ Yes             | ❌ No                       | ❌ No                       |
| Reassignment    | ✅ Yes             | ✅ Yes                      | ❌ No                       |
| Hoisting        | ✅ Yes (undefined) | ✅ Yes (temporal dead zone) | ✅ Yes (temporal dead zone) |
| Must Initialize | ❌ No              | ❌ No                       | ✅ Yes                      |


## 💡 Best Practices
- Use let for variables whose values will change.
- Use const for values that should never change.
- Avoid var in modern JavaScript unless working with legacy code.
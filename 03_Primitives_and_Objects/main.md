## 🔹 Primitives and Objects in JavaScript  

JavaScript has two main types of values: **Primitives** and **Objects**.  

---

### 🟢 **Primitives (Immutable, Stored by Value)**  
Primitives are simple **immutable** data types that store only a **single value**.  

#### ✅ **There are Seven Primitive Data Types:**  
| Type         | Example |
|-------------|---------|
| **String**  | `"Hello"` |
| **Number**  | `42`, `3.14` |
| **Boolean** | `true`, `false` |
| **Undefined** | `let x;` (not assigned) |
| **Null** | `let y = null;` (empty value) |
| **BigInt** | `1234567890123456789n` |
| **Symbol** | `Symbol('id')` (unique identifier) |

#### 🔹 **Example:**
```js
let name = "Garvit";  // String
let age = 20;  // Number
let isStudent = true;  // Boolean
let score;  // Undefined
let nothing = null;  // Null
let bigNumber = 9007199254740991n;  // BigInt
let id = Symbol("id");  // Symbol
```

---

### 🔵 **Objects (Mutable, Stored by Reference)**  
Objects are **collections of key-value pairs** and are stored by **reference**.  

#### ✅ **Types of Objects:**  
- **Object Literals**
- **Arrays**
- **Functions**
- **Dates**
- **RegExp**  

#### 🔹 **Example:**
```js
let person = {
    name: "Garvit",
    age: 20,
    isStudent: true
};

let numbers = [1, 2, 3, 4, 5];  // Array (special type of object)

function greet() {
    return "Hello, world!";
}

console.log(person.name);  // Output: Garvit
console.log(numbers[0]);   // Output: 1
console.log(greet());      // Output: Hello, world!
```

---

### 🔥 **Key Differences:**
| Feature | Primitives | Objects |
|---------|------------|---------|
| **Stored** | By Value | By Reference |
| **Mutable?** | ❌ No (Immutable) | ✅ Yes (Mutable) |
| **Example** | `let x = "Hello";` | `let obj = {name: "Garvit"};` |
| **Memory Usage** | Fixed Size | Dynamic |

### 🚀 **Summary:**  
✅ Use **primitives** for simple values (strings, numbers, etc.).  
✅ Use **objects** when you need complex data structures (arrays, functions, etc.).  

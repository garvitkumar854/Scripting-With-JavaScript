# Operators and Expressions in JavaScript
In JavaScript, an operator is a symbol that performs an operation on values or variables, while an expression is a combination of values, variables, and operators that produces a result.


## 📌 What are Operators ?
Operators are used to perform operations on variables and values. JavaScript provides different types of operators:

### 🔸 Arithmetic Operators
Perform Basic Mathematical Calculations
| Operator | Description            | Example  | Result |
|----------|------------------------|----------|--------|
| `+`      | Addition               | `5 + 3`  | `8`    |
| `-`      | Subtraction            | `10 - 4` | `6`    |
| `*`      | Multiplication         | `6 * 2`  | `12`   |
| `/`      | Division               | `10 / 2` | `5`    |
| `%`      | Modulus (Remainder)    | `10 % 3` | `1`    |
| `**`     | Exponentiation (Power) | `2 ** 3` | `8`    |
| `++`     | Increment              | `let x = 5; x++` | `6` |
| `--`     | Decrement              | `let y = 10; y--` | `9` |

### 🔹 Example Code:
```js
let a = 16, b = 4;
console.log("A + B = ",a+b);
console.log("A - B = ",a-b);
console.log("A ** B = ",a**b);
```

### 🔸 Assignment Operators
Assignment operators are used to assign values to variables.

| Operator | Description                    | Example          | Equivalent To  | Result (if `x = 10`) |
|----------|--------------------------------|------------------|---------------|------------------|
| `=`      | Assign value                   | `x = 5`          | `x = 5`       | `5`              |
| `+=`     | Add and assign                 | `x += 3`         | `x = x + 3`   | `13`             |
| `-=`     | Subtract and assign            | `x -= 4`         | `x = x - 4`   | `6`              |
| `*=`     | Multiply and assign            | `x *= 2`         | `x = x * 2`   | `20`             |
| `/=`     | Divide and assign              | `x /= 5`         | `x = x / 5`   | `2`              |
| `%=`     | Modulus and assign (remainder) | `x %= 3`         | `x = x % 3`   | `1`              |
| `**=`    | Exponentiation and assign      | `x **= 2`        | `x = x ** 2`  | `100`            |

### 🔹 Example Code:
```js
let x = 10;
x += 5;  // x = x + 5 → x = 15
x *= 2;  // x = x * 2 → x = 30
console.log(x); // Output: 30
```

### 🔸 Comparison Operators

Comparison operators are used to compare two values and return a boolean (`true` or `false`).

| Operator | Description                         | Example        | Result |
|----------|-------------------------------------|---------------|--------|
| `==`     | Equal to (checks value only)       | `5 == "5"`    | `true` |
| `===`    | Strict equal to (checks value & type) | `5 === "5"`   | `false` |
| `!=`     | Not equal to (checks value only)   | `10 != 5`     | `true` |
| `!==`    | Strict not equal to (checks value & type) | `10 !== "10"` | `true` |
| `>`      | Greater than                       | `8 > 5`       | `true` |
| `<`      | Less than                          | `3 < 7`       | `true` |
| `>=`     | Greater than or equal to           | `6 >= 6`      | `true` |
| `<=`     | Less than or equal to              | `4 <= 3`      | `false` |

### 🔹 Example Code:
```js
console.log(10 > 5);   // true
console.log(5 == "5"); // true (loose comparison)
console.log(5 === "5");// false (strict comparison)
console.log(7 !== "7");// true (strict not equal)
```

### 🔸 Logical Operators  
Logical operators are used to combine multiple conditions and return `true` or `false`.

| Operator | Description                          | Example              | Result  |
|----------|--------------------------------------|----------------------|---------|
| `&&`     | Logical AND (both must be true)     | `(5 > 3) && (8 > 5)` | `true`  |
| `||`     | Logical OR (at least one is true)   | `(5 < 3) || (8 > 5)` | `true`  |
| `!`      | Logical NOT (reverses boolean value)| `!(5 > 3)`           | `false` |

### 🔹 Example Code:
```js
console.log(true && false);  // Output: false
console.log(true || false);  // Output: true
console.log(!true);          // Output: false
```

### 🔸 Bitwise Operators  
Bitwise operators perform operations at the **binary level**.

| Operator | Description               | Example (x = 5, y = 3) | Result  |
|----------|---------------------------|------------------------|---------|
| `&`      | Bitwise AND                | `5 & 3`  (0101 & 0011) | `1`     |
| `|`      | Bitwise OR                 | `5 | 3`  (0101 | 0011) | `7`     |
| `^`      | Bitwise XOR (exclusive OR) | `5 ^ 3`  (0101 ^ 0011) | `6`     |
| `~`      | Bitwise NOT (inverts bits) | `~5` (inverts `0101`)  | `-6`    |
| `<<`     | Left shift                 | `5 << 1` (0101 → 1010) | `10`    |
| `>>`     | Right shift                | `5 >> 1` (0101 → 0010) | `2`     |

### 🔹 Example Code:
```js
console.log(5 & 3);  // Output: 1
console.log(5 | 3);  // Output: 7
```

### 🔸 Ternary Operator
The **ternary operator** is a shorthand for `if...else` conditions.  

### 🔹 Example Code:
```js
let age = 20;
let access = (age >= 18) ? "Allowed" : "Denied";
console.log(access);  // Output: Allowed
```
## 📌 What are Expressions ?
An expression is a combination of variables, values, and operators that produces a result.
### 🔸 Types of Expressions:
- 1️⃣ Arithmetic Expression → `let total = (5 + 3) * 2;`
- 2️⃣ String Expression → `let greet = "Hello" + " World!";`
- 3️⃣ Logical Expression → `let isAdult = (age >= 18) && (age < 60);`
- 4️⃣ Function Expression → `let sum = function(a, b) { return a + b; };`

## Comments in JavaScript
Comments in JavaScript are used to add notes, explanations, or disable parts of the code without affecting its execution. They are ignored by the JavaScript engine.

## Types of Comments
- ### Single Line Comment: Used for short, one-line comments.
    ```js
    // This is a Single Line Comment
    ```
- ### Multi-line Comment: Used for longer comments spanning multiple lines.
    ```js
    /* This is a 
    Multi Line 
    Comment */
    ```


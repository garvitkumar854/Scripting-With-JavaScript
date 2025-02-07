# Operators and Expressions in JavaScript
In JavaScript, an operator is a symbol that performs an operation on values or variables, while an expression is a combination of values, variables, and operators that produces a result.


## 📌 What are Operators ?
Operators are used to perform operations on variables and values. JavaScript provides different types of operators:

### 🔹 Arithmetic Operators
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

Example:
```js
let a = 16, b = 4;
console.log("A + B = ",a+b);
console.log("A - B = ",a-b);
console.log("A ** B = ",a**b);
```

### 🔹 Assignment Operators
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

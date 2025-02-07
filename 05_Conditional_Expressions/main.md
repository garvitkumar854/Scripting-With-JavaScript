# Conditional Expressions
Conditional expressions in JavaScript are used to make decisions in the code based on conditions. They evaluate an expression and execute different blocks of code depending on whether the condition is true or false.

## Types of Conditional Expressions In JavaScript

## 1. If Statement
✅ Executes block of code only if the condition is true.

🔹 Example
```js
let age = 18;
if (age >= 18) {
    console.log("You are an adult!");
}
```

## 2. If-else Statement
✅ Executes one block of code if true, otherwise executes another block.

🔹 Example
```js
let num = 5;
if (num > 0) {
    console.log("Positive Number");
} else {
    console.log("Negative Number");
}
```

## 3. If-else if-else Statement
✅ Checks multiple conditions in sequence.

```js
let score = 75;
if (score >= 90) {
    console.log("Grade A");
} else if (score >= 60) {
    console.log("Grade B");
} else {
    console.log("Grade C");
}
```

## 4. Ternary Operator (? :)
✅ A shorthand for if-else.

```js
let x = 10;
let result = (x > 5) ? "Greater than 5" : "Less than 5";
console.log(result);
```

## 5. switch Statement
✅ Checks a variable against multiple values.

```js
let day = 3;
switch (day) {
    case 1: console.log("Monday"); break;
    case 2: console.log("Tuesday"); break;
    case 3: console.log("Wednesday"); break;
    default: console.log("Invalid day");
}
```
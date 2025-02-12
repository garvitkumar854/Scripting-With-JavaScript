# Arrays in JavaScript
An array in JavaScript is a special variable that can hold multiple values in a single variable. It allows storing ordered collections of elements like numbers, strings, objects, etc.

## ✅ Creating an Array
```js
let fruits = ["Apple", "Banana", "Mango"];  // Array of strings
let numbers = [10, 20, 30, 40];             // Array of numbers
let marks_class_12 = [31, 78, "Absent", 74, 50, "Fail"];        // Array of Student Marks
console.log(marks_class_12);
```

## 🔹 Accessing Elements
Array elements are accessed using indexing (starting from 0).
```js
console.log(fruits[0]); // Output: Apple
console.log(numbers[2]); // Output: 30
console.log(marks_class_12[6])      // Output: 'undefined' {index not exists}
```

## 🔹 Array Properties & Methods
| Method              | Description                                 | Example Output |
|---------------------|---------------------------------------------|---------------|
| `length`           | Returns the number of elements in an array  | `fruits.length → 3` |
| `push(value)`      | Adds a new element at the **end**           | `fruits.push("Orange")` |
| `pop()`            | Removes the **last** element                | `fruits.pop()` |
| `shift()`          | Removes the **first** element               | `fruits.shift()` |
| `unshift(value)`   | Adds a new element at the **beginning**     | `fruits.unshift("Grapes")` |
| `indexOf(value)`   | Returns the index of a value               | `fruits.indexOf("Banana") → 1` |
| `includes(value)`  | Checks if value exists in array            | `fruits.includes("Mango") → true` |
| `join(", ")`       | Converts array to a string                 | `"Apple, Banana, Mango"` |

## 🔹 Looping Through an Array
Using a for loop:
```js
for (let i = 0; i < fruits.length; i++) {
    console.log(fruits[i]);
}
```
Using forEach():
```js
fruits.forEach(fruit => console.log(fruit));
```

# Question 4 Answer
```js
let num = prompt("Enter a Number: ");
num = Number.parseInt(num)          // Converts String to Number
if(num % 2 == 0 || num % 3 == 0){
    console.log("Number is Either Divisible by 2 or 3.");
} else{
    console.log("Not Divisible by Either 2 or 3.");
}
```
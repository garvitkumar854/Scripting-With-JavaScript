# Question 3 Answer
```js
let num = prompt("Enter a Number: ");
num = Number.parseInt(num)          // Converts String to Number
if(num % 2 == 0 && num % 3 == 0){
    console.log("Number is Divisible by 2 & 3.");
} else{
    console.log("Not Divisible by 2 & 3.");
}
```
# Question 2 Answer

```js
let arr = [1,2,3,4];
let a;
do{
    a = prompt("Enter a Number: ");
    a = Number.parseInt(a);
    arr.push(a);
    console.log(a);
} while(a != 0);
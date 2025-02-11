# Question 4 Answer

```js
let str = "Please give Rs 1000"
let amount = str.slice("Please give Rs ".length)            // str.slice(15)
console.log(amount)     
amount = Number.parseInt(amount)
console.log(typeof amount)
```
# Question 1 Answer
```js
let marks = {
    harry: 90,
    naveen: 50,
    manish: 70,
    lovish: 71
}

for(let i=0; i<Object.keys(marks); i++){
    console.log("The Marks of " + Object.keys(marks)[i] + " are " + marks[Object.keys(marks)[i]]);
}
```
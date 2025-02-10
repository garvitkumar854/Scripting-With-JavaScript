# Strings In JavaScript
Strings in JavaScript are used to store **text data**. They are immutable (cannot be changed) and can be written using **single (`'`), double (`"`)**, or **backticks (\``)** for template literals.

---

## 1️⃣ **Creating Strings**
```js
let str1 = "Hello, World!";
let str2 = 'JavaScript is awesome!';
let str3 = `My name is Garvit`; // Template literal
```

## 2️⃣ String Properties
- `.length` → Returns the number of characters in a string.
```js
let text = "JavaScript";
console.log(text.length); // 10
```

## 3️⃣ String Methods
-🔹 Changing Case
```js
let word = "Hello";
console.log(word.toUpperCase()); // "HELLO"
console.log(word.toLowerCase()); // "hello"
```

- 🔹 Extracting Parts of a String
```js
let str = "JavaScript";
console.log(str.slice(0, 4));   // "Java"
console.log(str.substring(4, 10)); // "Script"
console.log(str.substr(4, 6));  // "Script"
```

- 🔹 Replacing Text
```js
let sentence = "I love JavaScript!";
console.log(sentence.replace("love", "like")); // "I like JavaScript!"
```

- 🔹 Concatenation
```js
let firstName = "Garvit";
let lastName = "Kumar";
console.log(firstName + " " + lastName); // "Garvit Kumar"
console.log(`${firstName} ${lastName}`); // "Garvit Kumar" (Template literals)
```

- 🔹 Trimming Spaces
```js
let msg = "   Hello World!   ";
console.log(msg.trim());  // "Hello World!"
console.log(msg.trimStart()); // "Hello World!   "
console.log(msg.trimEnd());   // "   Hello World!"
```

- 🔹 Splitting a String
```js
let names = "Alice,Bob,Charlie";
console.log(names.split(",")); // ["Alice", "Bob", "Charlie"]
```

## 4️⃣ String Searching Methods
```js
let sentence = "JavaScript is a great language";
console.log(sentence.indexOf("great")); // 17
console.log(sentence.includes("JavaScript")); // true
console.log(sentence.startsWith("Java")); // true
console.log(sentence.endsWith("language")); // true
```








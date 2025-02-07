# Variables in JavaScript
Variables in JavaScript are used to store data values. JavaScript provides three ways to declare variables:

## 🔹 1.Using **var** (Old way, Avoid using)
- Function-scoped
- Can ve redeclared and updated within the same scope.
- Does not support block scope.
```javascript
var name = "Garvit";
console.log(name); // Output: Garvit
```
## 🔹 2.Using **let** (Modern way, Preferred for changeable values)
- Block-scoped (Limited to {} blocks).
- Cannot be redeclared in the same scope.
# Working with Stirng Formatting Methods (JavaScript)
This section covers basic formatting methods that are commnly used in JavaScript.
---

## 1. Changing the Casing of a String

JavaScript provides built-in methods to change the letter casing of a string.

### Convert to Uppercase 
```js
let text = "hello world";
let result = text.toUpperCase();
console.log(result); // "HELLO WORLD";
```

### Convert to Lowercase 
```js
let text = "Resah Febriyanto";
let result = text.toLowerCase();
console.log(result); // "resah febriyanto";
```

#### Real Use Case 
- Normalizing user input
- Case-insensitive comparisson (login, search, validation)

---

## 2. Trimming Whitespace from a String

Whitespace includes spaces, tabs, and new lines at the beginning or end of string.

#### Remove Whitespace from Both Sides

```js
let text = "   JavaScript   ";
let result = text.trim();
console.log(result); // "JavaScript"
```

#### Remove Whitespace from the Start Only

```js
let text = "   JavaScript";
let result = text.trimStart();
console.log(result); // "JavaScript"
```

#### Remove Whitespace from the End Only 

```js
let text = "JavaScript   ";
let result = text.trimEnd();
console.log(result); // "JavaScript"
```

### Real Use Case 
- From input validation
- Cleaning user data before saving
- Preventig empty input errors

----

### Summary

#### Methods                   
- `toUpperCase()`: Converts string to Uppercase
- `toLowerCase()`: Converts string to Lowercase
- `trim()`: Removes whitespace from both sides
- `trimStart()`: Removes whitespace from the start only
- `trimEnd()`: Removes whitespace from the end only





























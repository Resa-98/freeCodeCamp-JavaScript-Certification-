
# Working with String Modification Methods
This section covers basic methods used to modify strings in JavaScript.
---

## 1. Replacing Parts of a String
You can replace part of a string using the `replace()` method.

### Example 
```js
let text = "I love JavaScript";
let newText = text.replace("JavaScript", "Coding");
console.log(newtext); // "I love Coding"
```
### Important Notes 
- `replace()` does not change the original string
-  It returns a new string
-  By default, it replaces only the first match

### Real Use Case 
- Replacing words in text
- Formatting user input
- Simple text corecctions

## 2. Repeating a String
You can repeat a string multiple times using the `repeat()` method.

### Example 
```js
let word = "Hello";
let result = word.repeat(3);
console.log(result); // "Hello Hello Hello"
```

### Important Notes 
- `repeat()` accepts a number
- The original string remains unchanged

### Real Use Case 
- Generating repeated text
- Creating simple patterns
- UI placeholders or separators

 #### Summary 
- `replace()` : Replaces part of a string with another
- `repeat()` : Repeats a string a given number of times
 





















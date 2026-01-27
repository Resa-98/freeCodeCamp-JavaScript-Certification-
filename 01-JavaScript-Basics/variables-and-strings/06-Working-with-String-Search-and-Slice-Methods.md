# Working with String Search and Slice Methods 
  This lesson focuses on how to **search inside strings** and **extract parts of strings** in JavaScript
---
## 1. Testing if a String Contains a Substring

### `includes()`
The `includes()` method checks whether a string contains a specific substring.
```js
let sentence = "I Love JavaScript";

sentence.includes("JavaScrpit"); // true
sentence.includes("python"); // false
```

Key Points: 
- Returns `true` od `false`
- Case-sensitive
- Does not modify the original string
---

### `indexOf()`
The `indexOf()` method returns the position of substring.
```js
sentence.indexOf("JavaScript"); // 7
sentence.indexOf("python"); // -1
```
Key points:
- Returns the index number
- Returns `-1` if not found
- Case-sensitive
---

## Extracting a Substring from a String
`slice()`
The `slice()` method extracts a portion of a string and returns a new string.
```js
let word = "JavaScript";

word.slice(0, 4); // "Java"
word.slice(4); // "Script" 
```
Key points: 
- Takes `start` and `end` indexes
- End index is not included
- Original string is not changed
--- 

### Negative Index 
You can use negative values to count from the end.

```js
word.slice(-6); //"Script"
```

#### Common Mistakes 
- Forgetting that methods are Case-sensitive
- Confusing `slice()` end index (not inclusive)
- Expecting strings to change (strings are immutable)

#### Summary 
- `includes()` checks if a substring exist
- `indexOf()` finds the position of a substring
- `slice()` extracs part of a string
-  All string methods return new strings
























  

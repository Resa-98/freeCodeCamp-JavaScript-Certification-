# Working with Strings in JavaScript

This lesson covers how strings work in JavaScript, how to access and manipulate them, and how they are used in real user interactions.

---

## 1. Bracket Notation
**Bracket notation** is used to access individual characters in a string.

```js
let word = "JavaScript";
console.log(word[0]); // J
console.log(word[4]); // S
```
### Core Concepts 
- Index starts from `0`
- Strings are **read-only** (immutable)
- You cannot change characters directly
```js
word[0] = "j"; // does not work
```

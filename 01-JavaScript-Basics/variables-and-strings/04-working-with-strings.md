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
#### Core Concepts 
- Index starts from `0`
- Strings are **read-only** (immutable)
- You cannot change characters directly
```js
word[0] = "j"; // does not work
```
---

## 2. Newline and Escape Characters
#### Newline
Use `\n` to create a new line in a string.
```js
let text = "Hello\nWrold";
console.log(text);
```
#### Escape Charactes
Used when you need special characters inside strings.
```js
let quote = "he said, \"JavaScript is fun\"";
```
Common escape characters: 
-  `\n` : new line
-  `\"` : double quote
-  `\'` : single quote
-  `\\` : backslash
---

## 3. Template Literals & String Interpolation
Template litarals use **backticks**  `` ` `` instead of quotes.
```js
let name = "Resah Febriyanto";
let age = 28;
let message = `My name is ${name} and I am ${age} years old.`;
```
#### Why Tempalte Literals Are Important
- Cleaner syntax
- Easier to read
- Support multi-line strings
- Allows string interpolation using `${}`
---

## 4. Finding a Substring Position
Use `indexOf()` to find the position of a substring.
```js
let sentence = "I love JavaScript";
console.log(sentence.indexOf("JavaScript")); // 7
```
#### Important Notes 
- Returns the **index number**
- Returns `-1` if the substring is not found
- Case-sensitive
---

## 5. The `Prompt()` Method
The `prompt()` mehtod displays a dialog  box that asks the user for input.
```js
let userName = prompt("What is your name?");
console.log(userName);
```
#### How is Works 
- Input is always returned as a **stirng**
- Used mainly for simple user interaction
- Common id learning and small demos
---
### Summary
- Bracket notation accesses string characters
- Escape characters handle special formatting
- Template literals improve readibilty
- `indexOf()` helps locate substrings
- `prompt()` collects user input as strings


















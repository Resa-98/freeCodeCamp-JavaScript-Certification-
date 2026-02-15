# STRINGS & CONCATINATION (JavaScript)
---
## What is it?
A string is a data type for storing text in JavaScript.

## Why is it important?
Strings are used to:
- Display text on websites
- Store user input (name, email, message)
- Combine data into sentences

## Core Concept (Must Understand)

### 1. Strings are Immutable
- Strings **cannot be changed directly**
- Each change produces a new string



#### Code Example
```js
let text = "hello";
text[0] = "H";
console.log(text); // "hello"
```

### 2. Strings Have Indexes
- Indexes start at 0
- Can be accessed per character

#### Code Example
```js
let word = "JavaScript";
console.log(word[0]); // J
```
### 3. String Length
- Use  `.length` to find the number of characters

#### Code Example 
```js
let word = "Hello";
console.log(word.length); // 5
```
#### Important notes: 
- `.length` no matter the index of sequence.
- 

### 4. How to write strings
- `" "` -> double quote
- `' '` -> single quote
- `` ` ` `` -> template literal (recomended)

#### Code Example 
```js
let name = "Resa";
let message = `Hello, ${name}`;
```

### 5. Strings Can Be Concatenated
- Using the `+` operator
- Or the template literal `${}`

#### Code Example 
```js
let result = "Hello " + "World";
let name = "Resa";
let greeting = "Hello " + name;
let age = 25;
let message = `My name is ${name}, I am ${age} years old`;
```

  
   



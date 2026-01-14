# Working with Data Types (JavaScript)

## What are Data Types?
Data types define the kind of value a variable can hold.  
JavaScript uses data types to know how to process and manipulate values.

---

## Core Data Types

### 1. Number
Used for numeric values (integers and decimals).

#### Code Example
```js
let age = 25;
let price = 19.99;
```
- No separate type for integers or floats
- Can be used in math operations

### 2. String
Used for text values.

#### Code Example
```js
let name = "Resa";
let message = `Hello, ${name}`;
```
##### Core Concepts:
- Strings are immutable
- Index starts from `0`
- Use template literals for readability

### 3. Boolean
Used for logical values.

#### Code Example
```js
let isLoggedIn = true;
let isAdmin = false;
```
- Often Used in conditions (`if`,`else`)
- Only two values: `true` or `false`

### 4. Undefined
A variable that is declared but not assigned a value.

#### Code Example
```js
let score;
console.log(score); // undefined
```
### 5. Null 
Represents an intentional empty value.

#### Code Example
```js
let selectedUser = null;
```
- `null` means **nothing on purpose**
- Different from `undefined`

### Checking Data Types
Use `typeof` to check a value's data type. 

#### Code Example 
```js
typeof 10;          // "number"
typeof "hello";     // "string"
typeof true;        // "boolean"
typeof undefined;   // "undefined"
typeof null;        // "object" (JavaScript quirk)
```
### Type Conversion 
#### Implicit Conversion
JavaScript automatically converts types.
```js
"5" + 1; // "51"
"5" - 1; // 4
```
### Explicit Conversion
You manually convert types.
```js
Number("10"); // 10
String(25); // "25"
Boolean(1); // true
```

#### Real World Usage 
- Numbers : prices, quantities, calculations
- Strings : user input, messeages, UI text
- Booleans : login status, conditions
- Null/Undefined : empty or missing data

#### Common Mistakes
- Mixing strings and numbers unintentionally
- Forgetting that strings are immutable
- Confusing `null` with `undefined`


## Summary 
- JavaScript has multiple data types
- Each type behaves differently
- Understanding data types prevents logic bugs
- Always be aware of type conversion













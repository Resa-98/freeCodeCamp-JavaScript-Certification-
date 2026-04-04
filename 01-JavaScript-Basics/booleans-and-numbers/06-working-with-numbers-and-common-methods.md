# Working with Numbers and Common Number Methods (JavaScript)

This section explains common number-related methods used in JavaScript for validation, conversion, and formatting.

---

## 1. How does isNaN() work?

The `isNaN` function checks whether a value is **Not a Number (NaN)**.

### Example
```js
console.log(isNaN(10)); // false
console.log(isNaN("10")) // false
console.log(isNaN("hello")) // true
```

#### Important Notes 
- `isNaN()` converts the value before checking
- `"10"` is NOT NaN because it can be converted to a number
- `"hello"` is NaN because it can't be converted

## 2. parseFloat() and parseInt()

These methods convert strings into numbers.

---
### `parseInt()`

Converts a string into an integer (whole number).
```js
parseInt("100"); // 100
parseInt("100px"); // 100
parseInt("abc"); // NaN
```
---

### `parseFloat()` 

Converts a string into a decimal (floating-point number).
```js
parseFloat("10.5"); // 10.5
parseFloat("10.5px"); // 10.5
parseFloat("abc"); // NaN
```
---

#### Important Notes 

- Both methods read numbers from the start of the string
- Stop reading when encountering invalid characters
- Return `NaN` if no valid number is found

---

## 3. `toFixed()` 

The `toFixed()` method formats a number to a fixed number of decimal places.

### Example 
```js
let price = 10.456;
console.log(price.toFixed(2)); // "10.46"
```

#### Important Notes 
- Returns a string, not a number
- Rounds the value
- Useful for displaying prices

---

## Real Use Cases 
- `isNaN` → validation user input
- `parseInt()` → converting from data to numbers
- `parseFloat()` → handling decimal values (prices)
- `toFixed()` → formatting currency

---

### Summary 
|**Method** | **Description**|
|-----------|----------------|
|`isNaN` | Checks if a value is not number|
|`parseInt()`| Converts string to integer |
|`parseFloat()` | Convetrs string to decimal |
|'toFixed()` | Formats number to fixed decimal places |









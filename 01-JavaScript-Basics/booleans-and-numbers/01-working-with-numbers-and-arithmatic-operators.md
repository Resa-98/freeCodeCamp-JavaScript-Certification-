# Working with Numbers and Arithmetic Operators in JavaScript
This section explains how numbers work in JavaScript and how arithmetic operations are performed.

---

## 1. The Number Type in JavaScript
In JavaScript, there is only **one number type**, called `Number`.

### Types of Numbers
- **Integers**: `1`, `10`, `-5
- **Floating-point numbers (decimals)**: `3.14`, `0.5`
- **Special numbers**:
  - `Infinity`
  - `-Infinity`
  - `NaN` (Not a Number)

### Example
```js
let age = 25;
let price = 19.99;
let result = 10 / 0;
console.log(result); // Infinity
```
#### Important Notes
- JavaScript does not separate integers and decimals
- All numbers use **64-bit floating-point**

## 2. Arithmetic Operators in JavaScript
JavaScript provides several arithmetic operators to work with numbers.

### Common Arithmetic Operators

| **Operator** | **Description** |  **Example** |
| ----------- | ----------- | ----------- |
| `+`      | Addition | `5 + 2` ➡ `7` | 
| `-`  | Substraction | `5 - 2` ➡ `3`|
| `*`      | Multiplication | `5 * 2` ➡ `10` | 
| `/`  | Division | `5 / 2` ➡ `2.5`|
| `%`      | Modulus (remainder) | `5 % 2` ➡ `1` | 
| `**`  | Exponentiation | `2 ** 3` ➡ `8`|


### Example 

```js
let a = 10;
let b = 3;

console.log(a + b); // 13
console.log(a % b); // 1
```

#### Real Use Case 
- Calculating prices
- Working with scores or counters
- Pagination logic

## 3. Calculations with Numbers and Strings
When numbers and strings are used together, JavaScript follows specific rules.

### Using the `+` Operator
- If one operand is a string, JavaScript performs **string concatenation**

  ```js
  let result = 5 + "5";
  console.log(result); // "55"
  ```
### Using Other Operators
- JavaScript tries to convert string into numbers

```js
console.log(10 - "5"); // 5
console.log(10 * "2"); // 20
console.log(10 / "a"); // NaN
```
#### Important Notes 
- `+` is special (can mean addition or concatenation)
- Other operators force numeric conversion
- Invalid conversions result in `NaN`

### Summary

| **Concept** | **Explanation** |
| :---        | :---            |
| Number type | JavaScript uses one number type |
| Arithmetic Operators | Used for mathematical operations |
| String + Number | Results in string concatenation |
| other operators | Converts strings to numbers |

  

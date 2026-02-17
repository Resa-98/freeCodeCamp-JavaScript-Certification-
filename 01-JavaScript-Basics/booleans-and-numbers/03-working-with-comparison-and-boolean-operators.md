# Working with Comparison and Boolean Operators (JavaScript) 

This section explains how booleans work in JavaScript and how comparison operators are used to make decisions in code.

--- 

## 1. What Are Booleans?

A **Boolean** is a data type that has only two values: 
- `true`
- `false`

Booleans are commonly used in conditions, comparisons, and decision-making logic.

### Example 
```js
let isLoggedIn = true;
let hasPermission = false;

console.log(isLoggedIn); // true
console.log(hasPermission); // false
```
### Real Use Case 
- Login status
- Form validation
- Feature toogles

# 2. Equality and Inequality Operators 

Equality operators are used to compare values.

### Loose Equality (`==`) and Inequality (`!=`) 
- Compares **values only**
- Performs **type conversion (coercion)**

  ```js
  console.log(5 == "5"); // true
  console.log(5 != "5"); // false
  ```
### Strict Equality (`===`) and Inequality (`!==`)
- Compares **values AND type**
- Does not perform type conversion

  ```js
  console.log(5 === "5"); // false
  console.log(5 !== "5"); // true
  ```

  #### Improtant Notes
  - Always prefer `===` and `!==`
  - They prevent unexpected bugs

# 3. Comparison Operators

Comparison operators compare two values and return a boolean.

#### Common Comparison Operators

| **Operators** | **Description** | **Example** |
| ---           |    ---------    |         ---- |
|`>` | Greather than | `5 > 3` ➡ `true` |
|`<` | Less than | `3 < 5` ➡ `true` |
|`>=` | Greather than or equal to | `5 >= 5` ➡ `true` |
|`>=` | Less than or equal to | `3 <= 5` ➡ `true` |

### Example 
```js
let score = 80;

console.log(score > 70); // true
console.log(score <= 60); // false
```

#### Real Use Case
- Passing grades
- Age verification
- Price comparison

# 4. Booleans Results in Expressions

Comparison expressions always return a boolean value.

### Example 
```js
let age = 18;
let isAdult = age >= 18;
console.log(isAdult); // true
```

## Summary

|**Concept** |**Description**|
| ----------- | -------------|
|Boolean | `true` or `false`|
|`==` vs `===` | Loose vs strict comparison|
|Comparison operators | Compare numeric or string values|
|Result | Always returns a boolean|

















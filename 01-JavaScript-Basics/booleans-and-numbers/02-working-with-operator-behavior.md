# Working with Operator Behavior in JavaScript 

This section explains how operators behave in JavaScript, including precedence, increment/decrement, and compound assignment operators.

---

## 1. Operator Precedence

Operator precedence determines **the order in which operators are evaluated** in an expression.

### Basic Rule 
- Operators with **higher precedence** are evaluated first.
- Parentheses `()` override precendece.

### Example 
```js
let result = 5 + 3 * 2;
console.log(result); // 11

let result = (2 + 1) * 5;
console.log(result); // 15
```

### Common Precendece Order (High ➡ Low)
1. `()`
2. `**`
3. `*`, `/`, `%`
4. `+`, `-`
5. `=`

#### Real Use Case
- Calcualation in forms
- Complex expressions in logic
- Avoiding unexpected result

---

## 2. Increment and Decrement Operators

Increment and decrement operators increase or decrease a number by `1`.

### Increment (`++`)

```js
let count = 1;
count++;

console.log(count); // 2
```

### Decrement (`--`)

```js
let count = 3;
count--;

console.log(count); // 2
```
### Prefix vs Postfix

```js
let x = 5;

console.log(++X); // 6
console.log(X++); // 6 (then x becomes 7)
```

#### Important Notes
- Prefix changes the value **before** use.
- Postfix changes the value **after** use.

### Real Use Case 
- Counters
- Loops
- Tracking user actions

---

## 3. Compound Assignment Operators 

Compound assignment operators combine an operation with assignment.

### Common Compound Operators

| **Operators** | **Example** | **Same As** |
|:---           | :----------: |        ---:|
|`+=` | `x += 5` | `x = x + 5`|
|`-=` | `x -= 2` | `x = x - 2`|
|`*=` | `x *= 3` | `x = x * 3`|
|`/=` | `x /= 2` | `x = x / 2`|
|`%=` | `x %= 2` | `x = x % 2`|

### Example

```js
let total = 10;
total += 5;

console.log(total); // 15
```

### Real Use Case
- Updating values in loops
- Managing totals or scores
- Cleaner and shorter code

---
### Summary 

| **Concept** | **Description**|
| ------------ | ----------|
|Operator precedence | Defines calculation order|
|Increment/Decrement | Adds or substracts 1|
|Compound assignment | Shorter way to update values|





















  

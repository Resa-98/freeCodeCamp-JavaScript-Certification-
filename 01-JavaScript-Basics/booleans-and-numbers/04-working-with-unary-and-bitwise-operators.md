# Working with Unary and Bitwise Operators 

This note explains **Unary Operators** and **Bitwise Operators** in JavaScript, how they work, and simple mental models to understand them easily.

---

## 1. What Are Unary operators, and How Do They Work?

**Unary operators** are operators that work with **only one operand**

--- 

### 1.1 Unary Plus (`+`)

Convert a value into a **number**.

```js
+"5" // 5
+true // 1
+false // 0
```
#### Commonly used for:
- Quick string-to-number conversion

### 1.2 Unary Minus (`-`)

Converts a value into a negative number.

```js
-"5" // -5
-true // -1
```

### 1.3 Logical NOT (`!`)

Reverses a boolean value.

```js
!true // false
!fasle // true
```
if the value is not a boolean, Javascript converts it to boolean first.

```js
!0 // true
!"hello" // false
```

### 1.4 Double NOT (`!!`)

Converts a value into a real boolean (`true` or `false`)

```js
!!1 // true
!!0 // false
!!"text" // true
!!"" // false
```

#### Often used for:
- Validation
- Checking truthy / falsy values

### 1.5 Increment (`++`) and Decrement (`-`)

```js
let x = 5;
x++; // 6
x--; // 5
```
Pre vs Post 

```js
++x // increment first, then use the value
x++ // use the value first, then increment
```

## 2. What Are Bitwise Operators, and How Do they Work?

**Bitwise operatos work at the binary level (0 and 1).**
javaScript converts numbers into binary before applying these operators.

### 2.1 Bitwise AND (`&`)

A bit is `1` only if both bits are 1

```js
 5 & 3
```
```
5 → 101
3 → 011
---------
    001 → 1
```

##### Analogy: both switches must be ON

## 2.2 Bitwise OR (`|`)

A bit is `1` if at least one bit is 1.

```js
5 | 3
```

```
101
011
---
111 → 7
```

##### Analogy: one switch ON is enough

## 2.3 Bitwise XOR (`^`)

A bit is `1` if the bits are different.

```js
5 ^ 3
```

```
101
011
---
110 → 6
```
###### Same = 0, Different = 1

## 2.4 Bitwise NOT (`~`)

Inverts all bits.

```js
~5
```

```
00000101
11111010
```
###### Produces a **negative number** (this is normal behavior).

## 2.5 Bitwise LEft Shift (`<<`)

Shifts bits to the left.

```js
8 << 2
```
```
8 → 1000
<< 2 → 100000 → 32
```
##### Formula:

```js
x << n === x * 2^n
```

## 2.6 Bitwise Right Shift (`>>`)

Shifts bits to the right

```js
8 >> 1 
```
```
1000 → 100 → 4
```
##### Formula: 

```js
x >> n === Math.floor(x /2^n)
```

## 3. Logical Operators vs Bitwise Operators

|**Operator** | **Type** | **How It Works**|
|----          | --------- |          ------|
|`&&` | Logical | Returns an operand (truthy/falsy)|
|`             |              | `     |
|`&`          | Bitwise | Operates on bits |
| `          |`           | Bitwise |


⚠️ Do not confuse them: 

```js
true && false // false
1 & 0 // 0
```
## 4.When Are Bitwise Operators Used?
- Permission flags
- Game development
- Performance optimization
- Low-level logic

 ⚠️ Rarely used on everyday web development, but **important to understand**

## 5. Quick Summary
- Unary operators  → work with one operand
- Bitwise operators  → work with binary (0 and 1)
- `<<`  → multiply by 2
- `>>` → divide by 2
- Logical operators ≠ Bitwise operators

## 6. Key Takeaway

JavaScript does not always work `true` and `false`.
sometimes it works with **raw values**, and even with **bits inside numbers.**







  

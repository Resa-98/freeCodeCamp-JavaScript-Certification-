# Working with Conditional Logic and Math Methods

This note explains how conditional logic and math utilities work in JavaScript, including real-world use cases in front-end projects.

---

## 1. What Are Conditional Statements, and How Do If / Else If / Else Statements Work?

### What Is a Conditional Statement?
A **conditional statement** allows JavaScript to make decisions based on a condition that evaluates to `true` or `false`.

JavaScript mainly uses:
- `if`
- `else if`
- `else`

---

### Basic Syntax
```js
if (condition) {
  // code runs if condition is true
} else if (anotherCondition) {
  // runs if first condition is false and this is true
} else {
  // runs if all conditions are false
}
```


#### Example
```js
let score = 75;

if (score >= 80) {
  console.log("Excellent");
} else if (score >= 60) {
  console.log("Good");
} else {
  console.log("Try Again");
}
```
### How It Works (Flow)
1. JavaScript Checks the `if` condition.
2. If `true`, it runs that block and stops.
3. If `false`, it moves to `else if`.
4. If all conditions are `false`, `else` runs.


#### Real Used Case: 
- Showing login errors
- Form validation
- Displaying messages based on user input
- Checking user roles (admin / user)

## 2. What Are Binary Logical Operators, and How Do They Work?

Binary logical operatos work with two operands and return **one result.**

#### Common Binary Logical Operators

| **Operator** | **Name** | **Description** |
|---           | --------- |          -----|
|`&&`          | AND | Returns first falsy value or last truthy |
| `!`          | NOT | Reverses boolean value |

### AND (`&&`) 
```js
true && "hello"   // "hello"
false && "hello"  // false
0 && 5            // 0
```
##### How it works: 
- If the first operand is falsy → return it
- If the first operand is truthy → return the second operand

### OR (`||`)
```js
false || "hello" // "hello"
true || "hello" // true
```
##### How it works: 
- Returns the first truthy value
- If all are falsy, returns the last value

### NOT (`!`) 
```js
!true // false
!0 // true
!"hi" // false
```

#### Real used case: 
- Default values
- Conditional rendering
- Authentication checks
- Feature toggles

##### Example: 
``js
const userName = userInput || "guest";
```

## 3. What is the Math Object in JavaScript, and What Are Some Common Methods?

The **Math object** providfes built-in mathematical functions.

##### Common Math Methods

| **Mehthod** | **Description**|
|----         |----            |
|`Math.random()` | Generates random number (0-1) |
|`Math.floor()` | Rounds down |
|`Math.cell()` | Rounds up |
|`Math.round()` | Rounds to nearest integer |
|`Math.max()` | Returns highest value |
|`Math.min()` | Returns lowest value |
|`Math.abs()` | Absolute value |

#### Example: Rendom Number Between Two Values
```js
const min =  5;
const max = 10;

const randomNUm = Math.floor(Math.random() * ( max - min + 1)) + min;
console.log(randomNum); 
```
#### How the Code Works (Step by Step)
- `Math.random()` →  generates number between `0` and `0.999`
- Multiply by (`max`, `min` + 1) → scale range
- `Math.floor()` → remove decimals
- Add `min` → shift range

Result: random number **between 5 and 10 (inclusive)**

#### Real Used Case:
- Random banner images
- OTP / verification codes
- Game mechanics
- Random UI animations
- Paginations logic

### Summary
- Conditional statements control program flow
- logical operators return operands, not always booleans
- Math object helps with calculations and randomness
- These concetps are core for front-end interactivity






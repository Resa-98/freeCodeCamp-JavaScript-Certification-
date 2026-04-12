# Understanding Comparisons and Conditionals (JavaScript)

This sectuion explains how comparisons work with `null` and `undefined`, and how `switch` statements differ from `if/else` chains.

--- 

## 1. Comparisons with `null` and `undefined`

In JavaScript, `null` and `undefined` represent "no value", but they behave differently in comparisons.

--- 

### Loose Equality (`==`)
```js
console.log(null == undefined); // true
```

- JavaScript treats `null` and `undefined` as equal
- This is a special rule in loose comparison

---

### Strict Equality (`===`)
```js
console.log(null === undefined); // false
```
- Different types not equal
- No type coercion

#### Comparison with Numbers
```js
console.log(null > 0); // false
console.log(null == 0); // false
console.log(null >= 0); // true
```
```js
console.log(undefined > 0); // false
console.log(undefined < 0); // false
console.log(undefined == 0); // false
```
---

##### Important Notes 
- `null` becomes `0` in numeric comparisons
- `undefined` becomes `NaN`
- Avoid using `==` for comparisons
- Prefer `===` for predictable result

### Real use case 
```js
let data = null;

if (data == null) {
console.log("No data available");
}
```
- Checks both `null` and `undefined`

## 2. Switch Statements

A `swtich` statement is used to perform different actions based on different conditions.

---

### Basic Syntax 
```js
let value = 2;

switch (value) {
    case 1;
          console.log("One");
    break;
     case 2;
          console.log("Two");
    break;
     case 3;
          console.log("Three");
    break;
  default:
          console.log("Other);
}
```

#### Important Notes 
- Uses strict comparison `===`
- No type coercion
- Requires `break` to stop execution

---

### Fall-through Behavior (without break)

```js
  let value = 2;

switch (value) {
        case 1:
              console.log("one");
        case 2:
              console.log("two");
        case 3:
              console.log("three";
        case 4:
          console.log("Fall-through output here");
}
```

#### Real Use Case
- Menu Systems
- Role based access
- Handling fixed values

---

## 3. Switch vs if/Else

**if/Else Example**
```js
let score = 85;
if (score > 90) {
  console.log("A");
} else if (score > 75) {
  console.log("B");
} else {
  console.log("C");
}
```

**Switch Example** 
```js
let role = "admin";

switch(role) {
    case "admin":
        console.log("Full access");
        break;
`    case "user":
        console.log("Limited access");
        break;
}
```
---

### Key Differences 
|**Feature** | **Switch** | **if/Else**|
|------------|------------|------------|
| Comparison | Strict (`===`) | Flexible |
| Use case | Fixed values | Ranges / conditions |
| Readabilty | Cleaner for many cases | Better for logic |

---

#### Summary 

| **Concept** | **Description**|
|----          |         -----|
| `null` vs `undefined` | Different types of "no value" |
| `==` vs `===` | Loose vs strict comparison | 
| `switch` | Best for fixed comparison | 
| `if/Else` | Best for complex logic |















## ASCII and Character Codes 

### What Is ASCII?
ASCII (American Standard Code for Information Interchange) is a character encoding system that assigns a **number** to each character.
#### Examples: 
- ``A`` : 65
- ``a`` : 97
- ``0`` : 48
- Space : 32
  Computers use these numbers to represent text internally.
---
### charCodeAt()
The `charCodeAt()` method returns the **ASCII (Unicode) number** of a character at a given index in a string.
```js
let letter = "A";
console.log(letter.charCodeAt(0)); // 65
```
Key points: 
- Requires an Index
- Returns a number
- Based on Unicode (ASCII is a subset)
---
### fromCharCode()
The `String.fromCharCode()` method converts a **number** back into a character.
```js
console.log(String.fromCharCode(65)); // "A"
```

Key Point:
- Takes one or more numbers
- Returns a string
- Useful for generating characters dynamically
---
#### Why This Matters
- Helps compare characters logically
- Used in encryption, validation, and sorting
- Explain why character comparisson works internally
---
#### Summary 
- ASCII maps characters to numbers
- `charCodeAt()` -> character -> number
- `fromCharCode()` -> number -> character
- Javascript uses Unicode, but ASCII values still apply
















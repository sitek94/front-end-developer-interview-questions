# JavaScript

<details>
  <summary>What is Scope?</summary>

- each function has its own scope
- only the code inside the function can access the variables scoped in that function
- scopes can be nested inside another
- variable name has to be unique within the same scope
</details>

<details>
  <summary>How to empty an array?</summary>
  
  * substitute with a new array
    ```js
    let arr = [1, 2, 3];
    arr = [];
    ```
  * set length of the array to 0
     ```js
    let arr = [1, 2, 3];
    arr.length = 0;
    ```
</details>

<details>
  <summary>What is unary operator?</summary>
  
  * it takes a single operand/argument and performs an operation
  * examples:
    * `!` logical NOT - converts to a boolean value then negates it
    * `+` unary plus - tries to convert an operand to a number 
    * `typeof` - returns a string which is a type of operand
</details>

<details>
  <summary>What is binary operator?</summary>
  
  * it works with two operands
  * most operators are binary:
    * Multiplicative Operators
    * Additive Operators
    * Bitwise Shift Operators
    * Relational Operators
    * Equality Operators
    * Binary Bitwise Operators
    * Binary Logical Operators
</details>

<details>
  <summary>What is ternary operator?</summary>
  
  * the only JavaScript operator that takes three operands
  * shortened version of `if ... else` statement
  * `condition ? ifTrueExpression : ifFalseExpression`
</details>

<details>
  <summary>What is Symbol?</summary>
  
  * a new primitive data type introduced in ES6
  * completely unique identifiers
    ```js
    let sym1 = Symbol('symbol');
    let sym2 = Symbol('symbol');
    console.log(sym1 === sym2) // → false
    ```
  * tokens that can be used as unique IDs
  * the only purpose of the text in the parentheses is to identify the symbol
</details>

<details>
  <summary>What data types do you know?</summary>
  
  Primitives - their purpose is to hold a value
  * `Undefined` 
  * `Number`
  * `String`
  * `Boolean`
  * `BigInt` - introduced in ES2020
  * `Symbol`
  Structural/reference types - they hold references to values
  * `Object`
  * `Function` - every function is derived from Object constructor
</details>

<details>
  <summary>How to clone an object?</summary>
  
  * `Object.assign()` (copying by reference)
    ```js
    let a = { a: 10 };
    let b = Object.assign({}, a);
    ```
  * `JSON.parse` and `JSON.stringify`
    ```js
    let a = { a: 10 };
    let b = JSON.parse(JSON.stringify(a));
    ```
  * spread operator (copying by reference)
    ```js
    let a = { a: 10 };
    let b = { ...a };
    ```
  * `for ... in` loop (copying by reference)
    ```js
    let a = { a: 10 };
    let b = {};
    for (let key in a) {
      b[key] = a[key];
    }
    ```
  * `cloneDeep` from Lodash
    ```js
    let a = { a: 10, b: { c: 10 } };
    let b = _.cloneDeep(a);
    ```
</details>

<details>
  <summary>Is the data stored in localStorage visible in other apps (different domains)?</summary>
 
  * the answer is **no**
  * data stored in `localStorage` is specific to the protocol of the page
  * In particular, data stored by a script on a site accessed with HTTP (e.g., http://example.com) 
    is put in a different localStorage object from the same site accessed with HTTPS (e.g., https://example.com).
</details>

<details>
  <summary>What are falsy values?</summary>
 
  * they are evaluated to false in conditionals
  * `0` 
  * `null`
  * `undefined`
  * `false`
  * `NaN`
  * `''` empty string
</details>

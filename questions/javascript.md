# JavaScript

<details>
  <summary>What is Scope?</summary>

  * each function has its own scope
  * only the code inside the function can access the variables scoped in that function
  * scopes can be nested inside another
  * variable name has to be unique within the same scope
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



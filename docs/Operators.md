# Operators

> Operators - weaving logic with javascript's thread.

Operators are special characters used to perform various operations (usually arithmetic) on values. They allow you to manipulate and perform calculations with data in your programs. JavaScript supports multiple types of operators, including the following:

1. **Arithmetic operators:** Arithmetic operators perform mathematical operations like addition, subtraction, multiplication, division, and more.

   ```javascript
   let x = 10;
   let y = 5;
   let sum = x + y; // Addition
   let difference = x - y; // Subtraction
   let product = x * y; // Multiplication
   let quotient = x / y; // Division
   let remainder = x % y; // Modulus (remainder)
   ```

2. **Comparison operators:** Comparison operators compare two values and return a Boolean (true or false) result.

   ```javascript
   let a = 10;
   let b = 5;
   let isEqual = a === b; // Equality
   let isNotEqual = a !== b; // Inequality
   let isGreaterThan = a > b; // Greater than
   let isLessThan = a < b; // Less than
   ```

3. **Logical operators:** Logical operators combine or manipulate Boolean values.

   ```javascript
   let isTrue = true;
   let isFalse = false;
   let andResult = isTrue && isFalse; // Logical AND
   let orResult = isTrue || isFalse; // Logical OR
   let notResult = !isTrue; // Logical NOT
   ```

4. **Assignment operators:** Assignment operators assign values to variables.

   ```javascript
   let x = 10;
   x += 5; // Equivalent to x = x + 5
   ```

5. **Increment and decrement operators:** Using these operators, you can either increase or decrease the value of a variable by one.

   ```javascript
   let count = 5;
   count++; // Increment by 1
   count--; // Decrement by 1
   ```

6. **Ternary (conditional) operator:** The ternary operator is a concise way to write simple conditional statements.

   ```javascript
   let age = 18;
   let canVote = age >= 18 ? "Yes" : "No";
   ```

7. **String concatenation operator:** The `+` operator can also be used to concatenate (join) strings together.

   ```javascript
   let firstName = "John";
   let lastName = "Doe";
   let fullName = firstName + " " + lastName;

   console.log(fullName); // John Doe
   ```

These are just a few examples of the many operators available in JavaScript. There are also bitwise operators, typeof operators, and more. Each operator has its specific purpose and usage.

!> It's crucial to understand the behaviour and [precedence of operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Operator_precedence) to write effective JavaScript code.

Understanding and using operators is fundamental to performing various tasks in JavaScript, from basic arithmetic calculations to complex logical evaluations and string manipulations. Operators allow you to work with data dynamically and efficiently in your JavaScript programs.

### Further study

Here are some links for further study on the concept of operators in JavaScript:

1. [Operators - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators).
2. [JavaScript operators - W3Schools](https://www.w3schools.com/js/js_operators.asp).

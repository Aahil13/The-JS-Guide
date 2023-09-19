# Error handling

> Error handling - navigating stormy code waters.

Error handling in JavaScript is the process of dealing with unexpected situations and errors that can occur during the execution of your code. Proper error handling ensures your programs can gracefully handle issues, provide helpful feedback, and prevent crashes.

There are various types of errors in JavaScript, which include the following:

- **`SyntaxError`:** This is a built-in error type that occurs when there are issues in the syntax in your code, such as missing parentheses or a typo. These errors prevent the code from running and are caught by the JavaScript engine before execution.

  ```javascript
  // Example of a syntax error
  console.log("Hello, World" // Missing closing parenthesis
  ```

- **`TypeError`:** Another built-in JavaScript error occurs when a value is of the wrong type, or an operation is performed on an inappropriate value.

  ```javascript
  var x = "5"; // x is a string
  var y = 10; // y is a number

  var result = x + y; // Try to add a string and a number

  console.log(result); // 510
  ```

- **Runtime error:** This type of error occurs when dividing by zero or attempting to access an undefined variable during code execution. These errors can be caught and handled to prevent program crashes.

  ```javascript
  // Example of a runtime error
  var x = 10;
  var y = x / 0; // Division by zero
  ```

## Error handling techniques

- **`try...catch` statement:** In the `try...catch` statement, you can catch and handle errors inside a code block. Using this statement, code within the `try` block is executed, and in the `catch` statement, errors are caught and handled.

  ```javascript
  try {
    //code that may throw an error
  } catch (error) {
    // Handle the error
    console.error("An error occurred:", error.message);
  }
  ```

- **`throw` statement:** You can explicitly throw a user-defined error using the' throw' statement. The `throw` statement is usually used within the `try...catch` statement.

  ```javascript
  function divide(x, y) {
    if (y === 0) {
      throw new Error("Zero division is not allowed");
    }
    return x / y;
  }

  try {
    var result = divide(10, 0);
    console.log(result);
  } catch (error) {
    console.error("An error occurred:", error.message);
  }
  ```

!> You can throw any value (string, number, object) as an error.

- **Finally block:** This block can be used with the `try...catch` statement. It contains code that will always get executed regardless of whether or not an error occurred. This block is sometimes optional and can be used for clean-up tasks such as closing files.

  ```javascript
  try {
    //code that may throw an error
  } catch (error) {
    //code to handle the error
  } finally {
    //code that always executes
  }
  ```

> :construction: In JavaScript, the built-in `error` object represents an error and comes with properties such as `name` and `message`, providing more information about the error. :construction:

### Further study

Here are some resources to learn more about error handling in JavaScript:

- [Error handling in JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Control_flow_and_error_handling#Error_handling)
- [Error handling best practices](https://www.toptal.com/javascript/javascript-error-handling-guide)
- [Error handling patterns in JavaScript](https://www.sitepoint.com/error-handling-patterns-in-node-js/)

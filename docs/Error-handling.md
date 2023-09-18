# Error handling

> Error handling - navigating stormy code waters.

Error handling in JavaScript is the process of dealing with unexpected situations and errors that can occur during the execution of your code. Proper error handling ensures that your programs can gracefully handle issues, provide useful feedback, and prevent crashes.

There are various types of errors in JavaScript which include the following:

- `SyntaxError`: This is a built-in error type that occurs when there are issues in the syntax in your code such as missing parentheses or a typo. These errors prevent the code from running at all and are caught by the JavaScript engine before execution.

  ```JavaScript
  // Example of a syntax error
  console.log("Hello, World" // Missing closing parenthesis
  ```

- `TypeError`: Another built-in JavaScript error which occurs when a value is of the wrong type or an operation is performed on an inappropriate value.

  ```JavaScript
  var x = "5";  // x is a string
  var y = 10;   // y is a number

  var result = x + y;  // Try to add a string and a number

  console.log(result); // 510
  ```

- Runtime error: This type of error occurs during the execution of the code when something unexpected happens, like dividing by zero or accessing an undefined variable. These errors can be caught and handled to prevent program crashes.

  ```JavaScript
  // Example of a runtime error
  var x = 10;
  var y = x / 0; // Division by zero
  ```

## Error handling techniques

- `try...catch` statement: The `try...catch` statement allows you to catch and handle errors that occur within a block of code. The code within the `try` block is executed, and if an error occurs, it's caught and handled in the `catch` block.

  ```JavaScript
    try {
        // Code that may throw an error
    } catch (error) {
        // Handle the error
        console.error("An error occurred:", error.message);
    }
  ```

- `throw` statement: Using the `throw` statement, you can explicitly throw a user-defined error. The `throw` statement is usually used within the `try...catch` statement.

  ```JavaScript
  function divide(x, y) {
      if (y === 0) {
          throw new Error("Division by zero is not allowed");
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

- Finally block: This is another block that can be used with the `try...catch` statement. It contains code that will always get executed regardless of whether or not an error occured. This block is sometimes optional and can be used for clean up tasks such as closing files.

  ```JavaScript
    try {
        // Code that may throw an error
    } catch (error) {
        // Code to handle the error
    } finally {
        // Code that always executes
    }
  ```

> :construction: In JavaScript, the built-in `error` object represents an error and it comes with properties such as `name` and `message` which provides more information about the error. :construction:

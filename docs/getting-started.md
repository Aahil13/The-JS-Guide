# Getting Started

> JavaScript - where code meets creativity.

You can start using JavaScript on the browser by including a JavaScript file with the HTML document of your project. There are two ways of adding JavaScript to your HTML. They are as follows:

- **Internal:** This is when you have the JavaScript code in the same page as the HTML code. Internal JavaScript is written within the `<script>` tag in the HTML file's `<head>` or `<body>` section.

  ```HTML
    <!DOCTYPE html>
    <html>
    <head>
        <title>Internal JavaScript</title>
        <script>
            // Internal JavaScript code in the <head>
            function greet() {
                alert("Hello from internal script!");
            }
        </script>
    </head>
    <body>
        <h1>Internal JavaScript Example</h1>

        <button onclick="greet()">Click Me</button>
    </body>
    </html>
  ```

- **External:** This is having seperate HTML and JavaScript files and linking them together using the `<script></script>` tag. The JavaScript file is stored with a `.js` extension.

  **index.js:**

  ```HTML
      <!DOCTYPE html>
      <html>
      <head>
          <title>External JavaScript</title>
          <script src="script.js"></script>
      </head>
      <body>
          <h1>External JavaScript Example</h1>

          <button id="externalButton">Click Me</button>
      </body>
      </html>
  ```

  **script.js:**

  ```javascript
  // External JavaScript code in script.js
  document
    .getElementById("externalButton")
    .addEventListener("click", function () {
      alert("Hello from external script!");
    });
  ```

!> Remember to adjust file paths as needed when using external JavaScript files. This separation of concerns (HTML in the HTML file, JavaScript in separate `.js` files) is considered best practice for maintainability and readability.

## Basic Structure of a JavaScript Program

A JavaScript program is a set of instructions that tells the browser to perform specific tasks. It's important to understand the basic structure of a JavaScript program. Here's a breakdown of the basic structure:

```javascript
// Basic Structure of a JavaScript Program

// 1. Comments: You can add comments to explain your code. The browser ignores them.
// This is a single-line comment.

/*
   This is a multi-line comment.
   It can span multiple lines.
*/

// 2. Statements: Instructions that the browser will execute line by line.
let greeting = "Hello, World!"; // Declaring a variable and assigning a value.

// 3. Expressions: Produce a value.
let sum = 10 + 5; // An expression calculates the sum of two numbers.

// 4. Functions: Blocks of reusable code.
function sayHello() {
  console.log("Hello there!");
}

// 5. Calling a Function: Execute the code inside the function.
sayHello();

// 6. Data Types: JavaScript has various data types like strings, numbers, booleans, etc.
let name = "Alice"; // A string variable.
const passed = True; // A boolean variable.
let age = 25; // A number variable.

// 7. Control Flow: Decision-making using conditional statements.
if (age >= 18) {
  console.log("You are an adult.");
} else {
  console.log("You are a minor.");
}

// 8. Loops: Repeatedly execute code.
for (let i = 1; i <= 5; i++) {
  console.log("Iteration " + i);
}
```

## Common Tools and Development Environments

You'll need a code editor and a web browser to write JavaScript code. The following are popular options for these tools:

1. **Code editors:**

   - [Visual Studio Code](https://code.visualstudio.com/Download)
   - [Sublime Text](https://www.sublimetext.com/)
   - [Atom](https://atom.io/)

2. **Web browsers:**
   - [Google Chrome](https://atom.io/)
   - [Mozilla Firefox](https://www.mozilla.org/en-US/firefox/new/)
   - [Microsoft Edge](https://www.microsoft.com/en-us/edge)

!> Modern browsers have built-in developer tools that provide consoles for debugging and exploring JavaScript code.

With your code editor and browser in hand, you're ready to dive into the exciting world of JavaScript programming. The next step is to explore the syntax of JavaScript.

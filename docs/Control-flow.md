# Control flow

> Control flow - navigating the code rapids.

Control flow refers to the order in which code statements are executed in your code. It determines how the program flows from one statement to another based on certain conditions and control flow statements. It allows you to make decisions, create loops for repetitive tasks, and control the logical flow of your program.

JavaScript provides a few statements that help you control the flow of program execution, including:

1. Conditional statements: These statements allow you to execute different chunks of code based on specified conditions. The following are examples of conditional statements:

   - `if`:Statements here are executed only if the condition is **true**
   - `else`: Statements are only executed if the condition specified in a `if` statement is **false**
   - `else if`: This allows you to add multiple conditions and is only executed if these statements are **true**.

     **Syntax**:

   ```javascript
   let age = 18;

   if (age < 18) {
     console.log("You are a minor.");
   } else if (age >= 18 && age < 65) {
     console.log("You are an adult.");
   } else {
     console.log("You are a senior citizen.");
   }
   ```

2. Loops: As the name implies, a loop can help you execute a code block repeatedly if the condition remains **true**. In JavaScript, there are three (3) types of loops as follows:

   - `for` loop: The `for` loop repeats a code block according to a specified number.

     **Syntax:**

   ```javascript
   for (let i = 0; i < 5; i++) {
     console.log("Iteration " + i);
   }
   ```

   - `while` loop: This repeatedly executes a code block if the condition remains **true**.

     **Syntax:**

   ```javascript
   let count = 0;
   while (count < 5) {
     console.log("Count is " + count);
     count++;
   }
   ```

   - `do...while` loop: With the `do...while` loop, you can guarantee that your code block will be executed at **least once** and only repeat its execution if the condition remains **true**.

     **Syntax:**

   ```javascript
   let x = 1;
   do {
     console.log("x is " + x);
     x++;
   } while (x <= 3);
   ```

3. Break and continue statements: The `break` statement terminates or **breaks** the current loop, while the `continue` statement will skip the current iteration of the loop and **continues** to the next one.

   **Syntax:**

   ```javascript
   for (let i = 0; i < 5; i++) {
     if (i === 3) {
       continue; // Skip iteration when i is 3
     }
     console.log("Iteration " + i);
     if (i === 4) {
       break; // Exit loop when i is 4
     }
   }
   ```

4. Switch statements: This allows you to execute different statements or lines of code on different conditions.

   **Syntax:**

   ```javascript
   var day = "Monday";

   switch (day) {
     case "Monday":
       console.log("It's the start of the workweek.");
       break;
     case "Friday":
       console.log("It's almost the weekend!");
       break;
     default:
       console.log("It's a regular day.");
   }
   ```

Control flow statements are essential for making your JavaScript programs dynamic and responsive to different conditions and data. They allow you to create logic that can handle various scenarios and make your code more powerful and flexible.

### Further study

1. [MDN Web Docs - Control flow and error handling](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Control_flow_and_error_handling).
2. [JavaScript if...else statement](https://www.w3schools.com/js/js_if_else.asp).
3. [JavaScript switch Statement](https://www.w3schools.com/js/js_switch.asp).
4. [JavaScript for Loop](https://www.w3schools.com/js/js_loop_for.asp).
5. [JavaScript while Loop](https://www.w3schools.com/js/js_loop_while.asp).

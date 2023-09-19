# Variables

> Variables - your script's dynamic building blocks.

In programming, a variable is a container for storing data types. With a variable, you can have any value (integer, boolean, string) stored with any name of your choice, which you can change at any time in the future, such that whenever you need to alter the variable, all you have to do is change the initial value and not the variable name.

You can visualize a variable as an empty box storing any data type you choose. You can call this box anything you want, such that any time the data type is needed, all you have to do is call the box's name.

## Variable declarations

In JavaScript, creating a variable is called a variable declaration, and there are three (3) ways to declare variables: using the `var`, `let`, and `const` keywords.

- `var`: Variables declared using the `var` keyword can be redeclared and reassigned. They can also be function or block scoped, depending on where they are declared.
- `let`: Variables declared with `let` can only be accessible within the block they were declared; hence, they are block scoped. They can be reassigned but not redeclared within that same block.
- `const`: Variables declared with `const` are also block scoped but cannot be reassigned once they are assigned a value. However, the properties or elements can still be modified for objects and arrays.

Here's an example of using these keywords:

```javascript
// Using var
var a = 10;
if (true) {
  var a = 20; // This reassigns the outer 'a'
}
console.log(a); // Outputs 20

// Using let
let b = 10;
if (true) {
  let b = 20; // This creates a new 'b' in the block scope
}
console.log(b); // Outputs 10 (the outer 'b' is not affected)

// Using const
const c = 10;
if (true) {
  const c = 20; // This creates a new 'c' in the block scope
}
console.log(c); // Outputs 10 (the outer 'c' is not affected)
```

!> Avoid using `var` in modern JavaScript, as its behaviour can lead to unexpected issues due to its function-scoping and hoisting behaviour. Instead, use `let` and `const` for block-scoping and predictable behaviour.

## Variable scoping

Scoping refers to the accessibility of a variable in different parts of code. There are two types of scoping, which are function and block scoping;

- **Function scope:** Variables declared with `var` have function scope, meaning they are accessible within the function they are declared in, including any nested functions.
- **Block scope:** A variable declared with either `let` or `const` has a block scope, meaning they are only accessible within the block it is declared in, such as within loops or conditional statements.

!> When naming variables, ensure to adhere to the [variable naming rules](https://www.geeksforgeeks.org/what-are-the-variable-naming-conventions-in-javascript/).

### Further study

Here are some links for further study on the concept of variables in JavaScript:

1. [MDN Web Docs - Variables](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_types#Variables)
2. [W3Schools - JavaScript Variables](https://www.w3schools.com/js/js_variables.php)
3. [JavaScript Variables: var, let, and const](https://www.freecodecamp.org/news/javascript-variables-var-let-and-const-what-why-and-how-to-use-them/)
4. [Understanding JavaScript Variables](https://www.digitalocean.com/community/tutorials/understanding-variables-in-javascript)
5. [JavaScript Variable Scope and Hoisting Explained](https://www.freecodecamp.org/news/javascript-variable-scope-and-hoisting-explained/)

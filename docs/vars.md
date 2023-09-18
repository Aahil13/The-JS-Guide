# Variables

> Variables - your script's dynamic building blocks.

In programming, a variable is a container for storing data types. With a variable, you can have any value(integer, boolean, string), stored with any name of your choice which you can change any time in the future, such that, whenever you need to alter the variable, all you have to do is change the initial value and not the variable name.

You can simply visualize a variable as an empty box which can store any data type of your choice. You can call this box anything you want such that, any time the data type is needed, all you have to do, is call the name of the box.

## Variable declarations

In JavaScript, the process of creating a variable is called variable declaration and there are three (3) ways you can declare variables, which are using the `var`, `let` and `const` keyword.

- `var`: Variables declared using the `var` keyword can be redeclared and reassigned. They can also be function or block scoped depending on where they are declared.
- `let`: Variables declared with `let` can only be accessible within the block they were declared, hence they are block scoped. They can be reassigned but not redeclared within that same block.
- `const`: Variables declared with `const` are also block scoped, but they cannot be reassigned once they are assigned a value. However, for objects and arrays, the properties or elements can still be modified.

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

!> Avoid using `var` in modern JavaScript, as its behavior can lead to unexpected issues due to its function-scoping and hoisting behavior.

## Variable scoping

Scoping refers to the accessibilty of a variable in different parts of code. There are two types of scoping which are function and block scoping;

- Function scope: Variables declared with `var` have function scope, meaning they are accessible within the function they are declared in, including any nested functions.
- Block scope: Variables declared with `let` and `const` have block scope, meaning they are only accessible within the block they are declared in, such as within loops or conditional statements.

!> When naming variables, ensure to adhere to the [variable naming rules](https://www.geeksforgeeks.org/what-are-the-variable-naming-conventions-in-javascript/).

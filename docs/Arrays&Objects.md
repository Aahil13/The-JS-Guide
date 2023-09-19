# Arrays & Objects

> Arrays & Objects - structuring data, unleashing power.

Arrays and Objects are two fundamental underlying concepts of JavaScript. They play a crucial role in organizing and manipulating data within your programs.

## Arrays

An array is an indexed collection of data or values. Each value in an array is called an element, and elements can be of any data type, including other arrays or objects.

In JavaScript, an array is created using square brackets `[]` and separating its elements with commas.

**Syntax:**

```javascript
let fruits = ["apple", "banana", "orange"];
```

To access the elements in an array:

```javascript
let firstFruit = fruits[0]; // "apple"
let secondFruit = fruits[1]; // "banana"
let thirdFruit = fruits[2]; // "orange"
```

!> You can obtain the elements in an array by accessing their index, starting from 0.

You can modify array elements by assigning new values to specific indexes. To modify the elements in an array:

```javascript
fruits[1] = "grape";
console.log(fruits); // Output: ['apple', 'grape', 'orange']
```

### Array methods

Arrays in JavaScript come with built-in methods which you can use to manipulate its elements. Some commonly used methods include:

- `push()`:  By using `push()` you can add elements to the end of an array.
- `pop()`: Using the `pop()` method, remove the last element of an array.
- `shift()`: Removes the first element.
- `unshift()`: `unshift()` adds elements to the beginning of an array.
- `slice()`: This returns a new array containing a portion of its original.
- `splice()`: `slice()`changes the contents of an array by removing, replacing, or adding elements.
- `concat()`: You can use `concat()` to combine multiple arrays together.
- `join()`:  Utilizing the `join()` method, you can join an array's elements to a string.
- `indexOf()`: You can return the first index at which a given element can be found in an array.
- `includes()`: Checks if an array contains a specific element and returns a boolean value.

## Objects

Objects are collections of key-value pairs that are arranged in an unordered manner. The keys (also called properties) are strings, and the values can be of any data type, including other objects or arrays. Objects represent more complex data structures and can contain functions, arrays, and other objects as values.

You can create an object using curly braces `{}` and define its properties using key-value pairs.

```javascript
let person = {
  name: "John",
  age: 30,
  isStudent: false,
};
```

You can access objects' properties using the dot or square bracket notation.

```javascript
let personName = person.name; // "John"
let personAge = person["age"]; // 30
```

Objects also support property modification or the addition of new properties. You can add new properties or modify the key of any key-value pair in an object using the following syntax:

```javascript
person.job = "Engineer"; // Adds a new property
person.age = 31; // Modifies an existing property
```

### Object methods

A function declared in an object is called a method. These methods can carry out various tasks related to the object.

```javascript
let car = {
  brand: "Toyota",
  start: function () {
    console.log("Engine started.");
  },
};
car.start(); // "Engine started."
```

!> Objects in JavaScript also support built-in methods. An example of such a method is `Objects.keys()`.

Arrays and objects are versatile and powerful data structures that enable you to represent and manipulate data in various ways. Understanding how to work with them is essential for JavaScript development.

### Further study

Here are some links for further study on the concept of arrays and objects in JavaScript:

1. [MDN Web Docs - Arrays](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)
2. [MDN Web Docs - Objects](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)
3. [W3Schools - JavaScript Arrays](https://www.w3schools.com/js/js_arrays.asp)
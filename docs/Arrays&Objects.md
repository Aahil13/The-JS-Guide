# Arrays & Objects

> Arrays & Objects - structuring data, unleashing power.

Arrays and Objects are two fundamental underlying concepts of JavaScript. They play a crucial role in organizing and manipulating data within your programs.

## Arrays

An array is an indexed collection of data or values. Each value in an array is called an element, and elements can be of any data type, including other arrays or objects.

You can create an array in JavaScript using square brackets `[]` and separate its elements with commas.

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

!> Elements in an array are accessed by their index, starting from 0.

You can modify array elements by assigning new values to specific indexes. To modify the elements in an array:

```javascript
fruits[1] = "grape";
console.log(fruits); // Output: ['apple', 'grape', 'orange']
```

### Array methods

Arrays in JavaScript comes with built-in methods which you can use to manipulate it's elements. Some commonly used methods include:

- `push()`: Adds one or more elements to the end of an array.
- `pop():` Removes the last element from an array.
- `shift()`: Removes the first element from an array.
- `unshift()`: Adds one or more elements to the beginning of an array.
- `slice()`: Returns a new array containing a portion of the original array.
- `splice()`: Changes the contents of an array by removing, replacing, or adding elements.
- `concat()`: Combines two or more arrays.
- `join()`: Joins all elements of an array into a string.
- `indexOf()`: Returns the first index at which a given element can be found in an array.
- `includes()`: Checks if an array contains a specific element and returns a boolean value.

## Objects

An object is an unordered collection of key-value pairs. The keys (also called properties) are strings, and the values can be of any data type, including other objects or arrays. Objects are used to represent more complex data structures and can contain functions, arrays, and other objects as values.

You can create an object using curly braces `{}` and define its properties using key-value pairs.

```javascript
let person = {
  name: "John",
  age: 30,
  isStudent: false,
};
```

You can access properties in an object using the dot or square bracket notation.

```javascript
let personName = person.name; // "John"
let personAge = person["age"]; // 30
```

Objects also support property modification or addition of new properties. You can add new properties or modify the key of any key-value pair in an object using the following syntax:

```javascript
person.job = "Engineer"; // Adds a new property
person.age = 31; // Modifies an existing property
```

### Object methods

A function declared in an object is called a method. These methods can carry out various task related to the object.

```javascript
let car = {
  brand: "Toyota",
  start: function () {
    console.log("Engine started.");
  },
};
car.start(); // "Engine started."
```

!> Objects in JavaScript also supports built-in methods. An example of such methods is `Objects.keys()`.

Arrays and objects are versatile and powerful data structures that enable you to represent and manipulate data in various ways. Understanding how to work with them is essential for JavaScript development.

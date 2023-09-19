# Events

> Events - jazz up your page with interactive rhythms.

Events are interactions or occurrences that happen in the browser, such as a user clicking a button, moving the mouse, or a webpage finishing loading. JavaScript allows you to listen to and respond to these events with specific actions.

## Event Types

1. **Mouse Events:**

   - `click`: Triggered when the mouse button is clicked.
   - `mousemove`: Fired when the mouse pointer moves over an element.
   - `Mousedown` and `mouseup`: Occurs when the mouse button is pressed and released over an element.

2. **Keyboard Events:**

   - `key-down`: Fired when a key on the keyboard is pressed down.
   - `keyup`: Triggered when a key is released.

3. **Form Events:**

   - `submit`: Fired when a form is submitted.
   - `input`: Occurs when the value of an input element changes.

4. **Window Events:**
   - `load`: Fired when the web page and its resources (like images and stylesheets) finish loading.
   - `resize`: Occurs when the browser window is resized.
   - `scroll`: Triggered when the user scrolls the webpage.

## Event Listeners

To respond to events, you can attach event listeners to HTML elements. An event listener is a function that "listens" for a specific event on an element and performs an action when that event occurs.

```javascript
var button = document.getElementById("myButton");
button.addEventListener("click", function () {
  // Code to run when the button is clicked
});
```

## Event Handling

1. **Event Object:** An event object is created when an event occurs. This object contains information about the event, such as the type of event and the element it occurred on.

   ```javascript
   button.addEventListener("click", function (event) {
     // Access event properties
     console.log(event.type); // "click"
   });
   ```

2. **Preventing Default Behavior:** Some events, like form submissions and link clicks, have default behaviors. You can prevent these default behaviors using the event object's `preventDefault()` method.

   ```javascript
   link.addEventListener("click", function (event) {
     event.preventDefault(); // Prevent the link from navigating
   });
   ```

## Event Delegation

Event delegation is a technique where you attach a single event listener to a common ancestor of multiple elements instead of attaching listeners to each element. This is useful for efficiently handling events for dynamically added or removed elements from the page.

## Event Propagation

Events in JavaScript follow a process called event propagation or event bubbling. An event on an element triggers the event handlers attached to that element and then propagates to its parent elements. You can control event propagation using methods like `stopPropagation()` or `preventDefault()`.

Events are an essential part of interactive web development. They allow you to respond to user actions and create dynamic, responsive web applications. Understanding event types, listeners, and handling is fundamental for JavaScript programming.

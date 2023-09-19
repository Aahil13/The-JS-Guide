# Events

> Events - jazz up your page with interactive rhythms.

In a browser, events occur when something happens, such as a user clicking a button, moving the mouse, or loading a webpage. JavaScript allows you to listen to and respond to these events with specific actions.

## Event types

1. **Mouse events:**

   - `click`: Triggered when the mouse button is clicked.
   - `mousemove`: Fired when the mouse pointer moves over an element.
   - `Mousedown` and `mouseup`: Occurs when the mouse button is pressed and released over an element.

2. **Keyboard events:**

   - `key-down`: Fired when a key on the keyboard is pressed down.
   - `keyup`: Triggered when a key is released.

3. **Form events:**

   - `submit`: Fired when a form is submitted.
   - `input`: Occurs when the value of an input element changes.

4. **Window events:**
   - `load`: Fired when the web page and its resources (like images and stylesheets) finish loading.
   - `resize`: Occurs when the browser window is resized.
   - `scroll`: Triggered when the user scrolls the webpage.

## Event listeners

To respond to events, you can attach event listeners to HTML elements. Events listeners are functions that perform actions when a specific event occurs on an element.

```javascript
var button = document.getElementById("myButton");
button.addEventListener("click", function () {
  // Code to run when the button is clicked
});
```

## Event handling

1. **Event object:** An event object is created when an event occurs. An event object contains information about the event, such as its type and its element.

   ```javascript
   button.addEventListener("click", function (event) {
     // Access event properties
     console.log(event.type); // "click"
   });
   ```

2. **Preventing default behavior:** Some events, like form submissions and link clicks, have default behaviors. You can prevent these default behaviors using the event object's `preventDefault()` method.

   ```javascript
   link.addEventListener("click", function (event) {
     event.preventDefault(); // Prevent the link from navigating
   });
   ```

## Event delegation

The event delegation technique involves attaching a single event listener to the common ancestor of multiple elements, rather than attaching listeners to each element individually. This is useful for efficiently handling events for dynamically added or removed elements from the page.

## Event propagation

Events in JavaScript follow a process called event propagation or event bubbling. An event on an element triggers the event handlers attached to that element and then propagates to its parent elements. You can control event propagation using methods like `stopPropagation()` or `preventDefault()`.

Events are an essential part of interactive web development. They allow you to respond to user actions and create dynamic, responsive web applications. Understanding event types, listeners, and handling is fundamental for JavaScript programming.

## Further study

Here are some links for further study on the concept of events in JavaScript:

- [Event reference](https://developer.mozilla.org/en-US/docs/Web/Events)
- [Event delegation](https://javascript.info/event-delegation)
- [Event propagation](https://javascript.info/bubbling-and-capturing)

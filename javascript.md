# Introduction to JavaScript

### 1. What is the console in JavaScript?
The console in JavaScript is a tool provided by web browsers that allows developers to log information, debug code, and interact with the JavaScript environment. It's commonly used for testing and troubleshooting scripts.

### 2. What is JavaScript?
JavaScript is a programming language commonly used for creating interactive effects within web browsers. It allows developers to manipulate webpage content dynamically.

### 3. What are variables in JavaScript and how are they declared?
Variables in JavaScript are containers for storing data values. They can hold various types of data such as numbers, strings, or objects.

Declaration examples:
```js
var x = 5; // using var
let name = "John"; // using let
const PI = 3.14; // using const (constant)
```

---

# JavaScript

### 1. What does it mean to "call a function from HTML" in JavaScript?
It refers to invoking a JavaScript function directly from within an HTML element, typically through event handlers like `onclick` or `onchange`.

### 2. How can you create an object in JavaScript?
You can create an object using object literal syntax:
```js
let myObject = {
  key1: value1,
  key2: value2
};
```

### 3. Can an array in JavaScript hold different types of data? How do you access elements in an array?
Yes, an array can hold different types of data.

Accessing elements:
```js
var myArray = [1, 2, 3];
console.log(myArray[0]); // Outputs: 1
```

### 4. How do you add elements to an array?
You can add elements using:
- `push()` method
- Direct index assignment

### 5. What is an object in JavaScript?
An object is a collection of key-value pairs, where keys are strings (or symbols) and values can be any type including other objects, arrays, or functions.

### 6. What is the `length` property of an array?
It returns the number of elements in the array.

### 7. How do you iterate over elements in an array?
You can use:
- `for` loop
- `forEach()` method
- `for...of` loop
- `map()` method

### 8. What is the purpose of `document.getElementById()`?
It retrieves an HTML element by its unique ID.

### 9. How do you call a function from HTML in JavaScript?
Example:
```html
<button onclick="myFunction()">Click me</button>
```

### 10. What is the Document Object in JavaScript? How do you access it?
The Document Object represents the entire HTML document.

You access it using the `document` object in JavaScript:
```js
document.getElementById("myId");
```
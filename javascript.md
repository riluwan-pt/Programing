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


### 11. What are some common methods and properties of the Document Object in JavaScript?

Some common methods and properties of the Document Object include:
- `getElementById()`: Retrieves an element by its ID.
- `getElementsByTagName()`: Retrieves elements by their tag name.
- `getElementsByClassName()`: Retrieves elements by their class name.
- `createElement()`: Creates a new HTML element.
- `innerHTML`: Sets or returns the HTML content of an element.

### 12. How do you add or modify properties of an object in JavaScript?

You can add or modify properties of an object by simply assigning a new value to a key, like this:

```javascript
let myObject = { name: "John", age: 30 };
myObject.name = "Jane"; // Modifies the value of the 'name' property
myObject.city = "New York"; // Adds a new 'city' property
```

### 13. How do you define functions/methods within an object in JavaScript?

You can define functions/methods within an object by simply assigning a function to a property of the object. These functions are then called methods of the object.

### 14. How can we access and invoke functions/methods within JavaScript objects?

Functions or methods within JavaScript objects can be accessed and invoked using dot notation. For example:

```javascript
objectName.methodName();
```

### 15. What is an array in JavaScript?

An array in JavaScript is a data structure that allows you to store multiple values in a single variable. It's a collection of elements, each identified by an index or a key.

```javascript
var myArray = [];
```

### 16. What are properties and methods of an object?

Properties are the key-value pairs that define the characteristics or attributes of an object. Methods, on the other hand, are functions that are associated with an object and can perform actions or calculations using the object's properties.

### 17. How can you access properties of an object in JavaScript?

You can access properties of an object using dot notation or bracket notation. For example:

```javascript
let myObject = { name: "John", age: 30 };
console.log(myObject.name); // Outputs: John
console.log(myObject["age"]); // Outputs: 30
```

### 18. What purpose do switch statements serve in JavaScript?

Switch statements provide a way to perform different actions based on different conditions in JavaScript, offering an alternative to long if-else chains.

```javascript
let day = 3;
switch (day) {
  case 1:
    console.log("Monday");
    break;
  case 2:
    console.log("Tuesday");
    break;
  case 3:
    console.log("Wednesday");
    break;
  default:
    console.log("Unknown day");
}
```

### 19. How does a do...while loop differ from a while loop?

A `do...while` loop executes the code block first and then checks the condition. In contrast, a `while` loop checks the condition first and then executes the code block.

### 20. What is the difference between parameters and arguments in a JavaScript function?

Parameters are the placeholders defined in the function declaration, while arguments are the actual values passed to the function when it is called. Parameters receive values from arguments during function execution.

### 21. What are data types in JavaScript?

Data types in JavaScript refer to the classifications of data that determine the values that can be assigned to variables. The main data types are number, string, boolean, and date.

### 22. What is the number data type in JavaScript?

The number data type in JavaScript represents numeric values, including integers and floating-point numbers.

### 23. What is the string data type in JavaScript?

The string data type in JavaScript represents text and is enclosed in single quotes (`''`) or double quotes (`""`).

### 24. What is the boolean data type in JavaScript?

The boolean data type in JavaScript represents a logical value, either `true` or `false`.

### 25. What is the date data type in JavaScript?

The date data type in JavaScript represents dates and times. It allows for the manipulation and formatting of dates and times in various ways.

## 26. What is a function in JavaScript?

A block of reusable code that performs a task.

## 27. How do you define a function in JavaScript?

Using the `function` keyword:

```javascript
function greet(name) {
  return "Hello " + name;
}
```

## 28. What is the purpose of parameters in a function?

They allow functions to accept input values for flexibility and reuse.

## 29. How do you call or invoke a function in JavaScript?

Use the function name followed by parentheses:

```javascript
greet("Alice");
```

## 30. What is a return statement in JavaScript functions?

Specifies the output of a function and ends execution.

## 31. How do you declare a function that doesn't require any parameters?

```javascript
function sayHello() {
  console.log("Hello!");
}
```

## 32. Can a JavaScript function accept multiple parameters?

Yes. Parameters are separated by commas:

```javascript
function add(a, b) {
  return a + b;
}
```

## 33. Explain the role of `document.getElementsByClassName()` in JavaScript.

It returns all elements with the specified class name.

```javascript
document.getElementsByClassName("btn");
```

## 34. What are conditions in JavaScript?

Conditions allow control of program flow based on logic.

## 35. What is an if statement in JavaScript?

Executes a block if a condition is true:

```javascript
if (x > 10) {
  console.log("x is greater than 10");
}
```

## 36. What is an if-else statement in JavaScript?

Executes one block if true, another if false:

```javascript
if (x % 2 === 0) {
  console.log("Even");
} else {
  console.log("Odd");
}
```

## 37. What is code refactoring?

Improving code structure without changing functionality.


## 38. Why is refactoring important in JavaScript development?

To keep code readable, maintainable, and scalable.


## 39. How do you debug issues in Browser JavaScript?

Use browser dev tools, breakpoints, and `console.log()`.


## 40. What is a global variable in JavaScript?

Defined outside any function, accessible everywhere.


## 41. What is a local variable in JavaScript?

Defined inside a function, accessible only within it.


## 42. What is a for loop in JavaScript?

Used to repeat a block of code a set number of times.

```javascript
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```

## 43. How do you declare and use a basic for loop?

Use `for (initialization; condition; increment)` syntax.


## 44. What is the purpose of the initialization in a for loop?

It sets the starting point of the loop.


## 45. What role does the condition expression play in a for loop?

It determines whether the loop should continue.


## 46. How does the increment/decrement expression work?

It updates the counter variable after each iteration.


## 47. How does `for...of` differ from `for...in`?

- `for...of`: iterates over values of iterable objects.  
- `for...in`: iterates over keys of an object.


## 48. What are while loops in JavaScript?

Repeats code as long as the condition is true.

```javascript
while (x < 10) {
  x++;
}
```

## 49. What are do...while loops in JavaScript?

Runs the code at least once, then checks the condition.

```javascript
do {
  x++;
} while (x < 10);
```

## 50. When should you use a while loop vs. a do...while loop?

Use `while` if the condition may be false from the start.  
Use `do...while` if you want to ensure at least one execution.

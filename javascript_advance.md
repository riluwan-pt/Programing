# JavaScript Advance

## 1. What is the significance of objects in JavaScript?
Objects in JavaScript enable developers to model real-world entities more effectively by grouping related data and behavior together, promoting code reusability and maintainability.

---

## 2. How do you define properties and methods within a JavaScript class?
Properties and methods within a JavaScript class are defined inside the class body using conventional syntax. Properties represent data associated with objects, while methods represent actions or behaviors that objects can perform.

**Example:**
```javascript
class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  greet() {
    console.log(`Hello, my name is ${this.name}`);
  }
}
const john = new Person("John", 30);
john.greet(); // Output: Hello, my name is John
```

---

## 3. What is object destructuring in JavaScript?
Object destructuring is a feature in JavaScript that allows you to extract multiple properties from an object and assign them to variables in a concise and structured way.

**Example:**
```javascript
const person = { name: "Alice", age: 25 };
const { name, age } = person;
console.log(name); // Output: Alice
console.log(age);  // Output: 25
```

---

## 4. What is array destructuring in JavaScript?
Array destructuring in JavaScript is a feature that allows you to extract multiple values from an array and assign them to variables in a single statement.

**Example:**
```javascript
const fruits = ["Apple", "Banana", "Cherry"];
const [first, second] = fruits;
console.log(first);  // Output: Apple
console.log(second); // Output: Banana
```

---

## 5. How do you perform array destructuring in JavaScript?
To perform array destructuring, you enclose the variables you want to assign the array elements to within square brackets on the left side of an assignment statement, and then assign the array on the right side.

**Example:**
```javascript
const numbers = [1, 2, 3];
const [a, b, c] = numbers;
console.log(a); // Output: 1
console.log(b); // Output: 2
console.log(c); // Output: 3
```

---

## 6. How do you create an object from a class in JavaScript?
To create an object from a class in JavaScript, you use the `new` keyword followed by the class name and any necessary arguments to initialize the object.

**Example:**
```javascript
class Car {
  constructor(make, model) {
    this.make = make;
    this.model = model;
  }
}
const myCar = new Car("Toyota", "Corolla");
console.log(myCar.make); // Output: Toyota
```

---

## 7. What is the difference between a class and an object in JavaScript?
A class in JavaScript is a blueprint for creating objects, defining their structure and behavior. An object, on the other hand, is an instance of a class, representing a specific entity with its own set of data and behavior.

---

## 8. What happens if the property you're trying to destructure doesn't exist in the object?
If the property doesn't exist, the value of the variable will be `undefined`.

**Example:**
```javascript
const obj = { a: 1 };
const { b } = obj;
console.log(b); // Output: undefined
```

---

## 9. Explain the concept of inheritance in JavaScript?
Inheritance in JavaScript allows a class (subclass) to inherit properties and methods from another class (superclass), enabling code reuse and promoting a hierarchical structure among classes.

**Example:**
```javascript
class Animal {
  speak() {
    console.log("Animal makes a sound");
  }
}
class Dog extends Animal {
  speak() {
    console.log("Dog barks");
  }
}
const myDog = new Dog();
myDog.speak(); // Output: Dog barks
```

---

## 10. What are constructors in JavaScript classes?
Constructors in JavaScript classes are special methods used for initializing newly created objects. They are automatically called when an object is instantiated from a class.

**Example:**
```javascript
class Book {
  constructor(title, author) {
    this.title = title;
    this.author = author;
  }
}
const myBook = new Book("1984", "George Orwell");
console.log(myBook.title); // Output: 1984
```

---

## 11. Is it possible to skip certain elements while destructuring an array?
Yes, you can skip elements by leaving an empty space for them inside the square brackets on the left side of the assignment.

**Example:**
```javascript
const numbers = [1, 2, 3];
const [first, , third] = numbers;
console.log(first); // Output: 1
console.log(third); // Output: 3
```

---

## 12. What are some practical use cases for array destructuring?
Array destructuring is commonly used for tasks such as extracting values from function return values, swapping variables, and iterating over arrays with `for...of` loops.

**Example:**
```javascript
let a = 1, b = 2;
[a, b] = [b, a];
console.log(a, b); // Output: 2 1
```

---

## 13. What is the spread operator in JavaScript?
The spread operator (...) allows an iterable to be expanded into individual elements.

**Example:**
```javascript
const numbers = [1, 2, 3];
const newNumbers = [...numbers, 4, 5];
console.log(newNumbers); // Output: [1, 2, 3, 4, 5]
```

---

## 14. How does the spread operator differ from the rest operator in JavaScript?
The spread operator expands elements, while the rest operator gathers elements into an array.

**Example:**
```javascript
function sum(...nums) {
  return nums.reduce((total, n) => total + n, 0);
}
console.log(sum(1, 2, 3)); // Output: 6
```

---

## 15. How is object destructuring useful in JavaScript?
It simplifies code by extracting specific properties from objects.

**Example:**
```javascript
const person = { name: "John Doe", age: 30, country: "USA" };
const { name, age } = person;
console.log(name); // Output: John Doe
console.log(age);  // Output: 30
```

---

## 16. Can you destructure nested objects using object destructuring?
Yes.

**Example:**
```javascript
const person = {
  name: "John Doe",
  age: 30,
  address: { city: "New York", country: "USA" }
};
const { name, address: { city } } = person;
console.log(name); // Output: John Doe
console.log(city); // Output: New York
```

---

## 17. What are objects in JavaScript?
Objects are instances of classes or prototypes.

**Example:**
```javascript
const car = { brand: "Toyota", model: "Corolla" };
console.log(car.brand); // Output: Toyota
```

---

## 18. What is Node.js?
Node.js is a runtime environment to run JavaScript outside of the browser.

**Example:**
```javascript
// Run with Node.js
console.log("Hello from Node.js");
```

---

## 19. What is JavaScript ES2015?
ES2015 (ES6) introduced new syntax and features.

**Example:**
```javascript
let name = "Alice";
const age = 25;
console.log(`${name} is ${age} years old.`);
```

---

## 20. What are let and const in JavaScript ES2015?
`let` and `const` are block-scoped variable declarations.

**Example:**
```javascript
let x = 10;
const y = 20;
x = 15; // Allowed
// y = 25; // Error: Assignment to constant variable
```

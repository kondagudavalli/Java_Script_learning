# Java_Script_learning
offical website to learn JavaScript
## https://developer.mozilla.org/en-US/docs/Web/JavaScript
=================================================================
# 📘 Complete JavaScript Notes

JavaScript (JS) is a **high-level, interpreted, single-threaded, dynamically typed programming language** used for web development.  
It is supported by all modern browsers and runs on the server through **Node.js**.

---

## 🔹 1. Introduction
- Created in 1995 by Brendan Eich.  
- Runs in the browser (client-side) and server (Node.js).  
- Multi-paradigm: supports **Object-Oriented, Functional, and Procedural** programming.  

---

## 🔹 2. Basics
### Comments
js
// Single line
/* Multi
   line */
Variables

var → function-scoped, hoisted.

let → block-scoped, no redeclaration.

const → block-scoped, immutable reference.

Data Types

Primitive: string, number, boolean, null, undefined, symbol, bigint

Non-primitive: object, array, function

Type Conversion
Number("123");   // 123
String(123);     // "123"
Boolean(0);      // false

🔹 3. Operators

Arithmetic: + - * / % **

Assignment: = += -= *=

Comparison: == === != !== > < >= <=

Logical: && || !

Ternary: condition ? a : b

Nullish Coalescing: ??

🔹 4. Control Flow
Conditional Statements
if (x > 10) { ... }
else if (x === 10) { ... }
else { ... }

Switch
switch(day) {
  case "Mon": ...
  default: ...
}

Loops

for

while

do...while

for...of → arrays

for...in → objects

🔹 5. Functions
Function Declaration
function greet(name) {
  return `Hello ${name}`;
}

Function Expression
const greet = function(name) { ... };

Arrow Functions
const greet = (name) => `Hello ${name}`;

IIFE
(function() { console.log("Runs immediately"); })();

Higher-Order Functions

Functions that take other functions as arguments or return functions.

const nums = [1,2,3];
const doubled = nums.map(n => n*2);

🔹 6. Objects
let person = {
  name: "Dhanu",
  age: 21,
  greet() { console.log("Hi"); }
};


Access: person.name or person['name']

Add: person.city = "Hyderabad";

Delete: delete person.age;

Object Methods

Object.keys(obj)

Object.values(obj)

Object.entries(obj)

Object.assign({}, obj)

Object.freeze(obj)

Object.seal(obj)

Object.preventExtensions(obj)

🔹 7. Arrays
let arr = [1,2,3];
arr.push(4);      // add
arr.pop();        // remove last
arr.shift();      // remove first
arr.unshift(0);   // add first

Iteration Methods

forEach()

map()

filter()

reduce()

some(), every()

find(), findIndex()

includes()

🔹 8. Strings
let str = "Hello World";
str.length;
str.toUpperCase();
str.includes("World");
str.split(" ");

🔹 9. Scope & Hoisting

Global Scope → accessible everywhere.

Function Scope → inside functions.

Block Scope (let, const).

Hoisting → Variables (var) and functions are moved to top of scope during execution.

🔹 10. Execution Context & Call Stack

Global Execution Context (GEC) → created first.

Function Execution Context (FEC) → created when function is called.

Call stack manages execution order.

🔹 11. this Keyword

In global scope → window (browser).

Inside object → refers to that object.

Arrow functions → inherit from parent scope.

🔹 12. Closures

A function that remembers variables from its outer scope even after that scope ends.

function outer() {
  let count = 0;
  return function() { return ++count; }
}
const counter = outer();
console.log(counter()); // 1

🔹 13. Prototype & Inheritance

JS uses prototype-based inheritance.

function Person(name) {
  this.name = name;
}
Person.prototype.greet = function() {
  console.log("Hello " + this.name);
};


ES6 Classes (syntactic sugar):

class Person {
  constructor(name) { this.name = name; }
  greet() { console.log("Hello " + this.name); }
}

🔹 14. DOM Manipulation

document.getElementById("id")

document.querySelector(".class")

element.innerHTML = "text";

element.style.color = "red";

document.createElement("div");

parent.appendChild(child);

🔹 15. Events
element.addEventListener("click", function(){ ... });


Bubbling & Capturing phases.

Event delegation for performance.

🔹 16. Error Handling
try {
  throw new Error("Something went wrong");
} catch(e) {
  console.log(e.message);
} finally {
  console.log("Always runs");
}

🔹 17. Asynchronous JS
Callbacks
setTimeout(() => console.log("Hello"), 1000);

Promises
let promise = new Promise((resolve, reject) => {
  resolve("Success");
});
promise.then(res => console.log(res));

Async/Await
async function fetchData() {
  let res = await fetch("url");
  let data = await res.json();
  console.log(data);
}

🔹 18. Event Loop

JS is single-threaded.

Event loop handles async tasks using:

Call stack

Callback queue (macrotasks)

Microtask queue (promises)

🔹 19. ES6+ Features

Arrow functions

Template literals

Destructuring

Spread/Rest operators

Default parameters

Classes

Modules (import/export)

Map, Set, WeakMap, WeakSet

Optional chaining ?.

Nullish coalescing ??

🔹 20. JSON
let obj = {name: "Dhanu"};
let str = JSON.stringify(obj); // to JSON string
let parsed = JSON.parse(str);  // back to object

🔹 21. Storage

localStorage → permanent until cleared.

sessionStorage → clears when tab closes.

cookies → store small data, sent with requests.

🔹 22. Modules
// math.js
export function add(a,b){ return a+b; }

// app.js
import { add } from './math.js';

🔹 23. Useful Built-in Objects

Date

Math

RegExp

Error

🔹 24. Memory Management

Garbage collection with reference counting & mark-and-sweep.

🔹 25. Where JS is Used

Frontend Development: React, Angular, Vue

Backend Development: Node.js, Express

Mobile Apps: React Native, Ionic

Desktop Apps: Electron

Game Development: Phaser, Three.js

AI/ML: TensorFlow.js

---

## This is a **full end-to-end JavaScript notes file**.  
Would you like me to also make a **cheat sheet version** (just syntax + one-liners) along with this detailed README, so you can quickly revise before interviews?


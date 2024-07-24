# JavaScript Interview Question & Answer

- Basic
- Variables & Data Types
- Operators & Conditions
- Loops
- String
- Array
- Objects
- Functions
- DOM
- Error Handling
- Events
- Asynchronous Programming
- Debugging
- BOM
- Window
- Web APIs
- OOPs
- Date & Time
- Maths
- Security & Performance
- ES6
- Advanced

<!-- 1 -->

## Basic

### What is JavaScript?

JavaScript is a lightweight, cross-platform, single-threaded, and interpreted compiled programming language. It is also known as the scripting language for webpages. It allows developers to create interactive and dynamic content on websites.

### What is the role of JavaScript engine?

A JavaScript engine is a specialized program that executes JavaScript code in web browsers and runtime environments like Node.js. Its responsible for translating, executing, and optimizing JavaScript code to client or server applications.

### What is use of JavaScript?

JavaScript is a multi uses programming language so there are a lot of uses like:

- **Web Development:** Mostly its used in web development for enhancing user interfaces with dynamic content.

- **Server-Side Development:** With Node.js, JavaScript can be used for backend programming.

- **Mobile App Development:** Using frameworks like React Native to develop cross-platform mobile applications.

- **Game Development:** Creating browser-based games using HTML5 and JavaScript.

- **Desktop Applications:** Building desktop applications with frameworks like Electron.

### What are client side & server side?

Client-side refers to everything that happens in the user's browser. It involves the front-end technologies and its responsible for the user interface and user interactions.

Server-side refers to operations that occur on the web server. It involves the back-end technologies and is responsible for database interactions, server logic, and business logic.

### Difference between Client Side & Server Side?

- **Execution Environment:** Client-side code runs on the user's browser, while server-side code runs on the server.

- **Scope and Access:** Client-side code can only interact with what's on the user's device like DOM manipulation, whereas server-side code can access databases, performing business logic and calculations, and handle sensitive operations securely.

- **Visibility:** Client-side code is visible to the user and can be inspected or manipulated, while server-side code is hidden from the user and is more secure.

<!-- 2 -->

## Variables & Data Types

### What are variables?

Variables are used to store and manipulate data. It can be declared using the `var`, `let`, or `const` keywords.

### What is difference between var, let & const?

### What are rules for naming variable in JS?

- Must begin with a letter, underscore (\_), or dollar sign ($).
- Can contain letters, digits, underscores, and dollar signs.
- Case-sensitive (e.g., `myVar` and `myvar` are different variables).
- Should not be a reserved keyword (e.g., `let`, `class`, `return`).

### What are Data Types in JavaScript?

Data types refer to hold the differnt types of values in JavaScript.

JavaScript is a dynamically typed language, meaning that variables can hold values of any type without specifying their type explicitly.

Data types categorized into two main group: Primitive and Non-Primitive types.

- **Primitive Data Types:** - Primitive data types used to define simple level of data as number, string, boolean, undefined, null, symbol, bigint etc.
- **Non-Primitive Data types** - Non-primitive data types used to define complex level of data as object, array, regexp, date & function.

### What is the difference between primitive and non-primitive data types?

### What is the difference between null & undefined in JS?

`null` and `undefined` are both used to represent absence of value, but they are used in different contexts and have different meanings.

- `undefined` represents a variable that has been declared but has not been assigned a value.

```sh
let x;
console.log(x); // Output: undefined
```

- `null` indicates that a variable is intentionally assigned "no value" or "empty".

```sh
let age = null; // Explicitly assigned null to indicate no value
console.log(age); // Output: null
```

#### Key Differences:

- `typeof undefined` is "undefined", while `typeof null` is "object".
- `null == undefined` is true, but `null === undefined` is false.
- `undefined` is usually a default value, while null is intentionally assigned

### Where get undefined value in JS?

- Variable declared but not assigned a value.

```sh
let x;
console.log(x); // Output: undefined
```

- Function parameter that's not provided.

```sh
function doSomething(x) {
 console.log(x); // Output: undefined
}
doSomething()
```

- Object property that doesn't exist

```sh
let obj = {};
console.log(obj.prop); // Output: undefined
```

- Function without a return statement

```sh
function doSomething() {
  // No return statement
}

console.log(doSomething()); // Output: undefined
```

### Where define null value in JS?

- `null` is typically used when you want to reset an object or variable to an empty or null state.

- Often used as a placeholder for optional values that may be assigned later.

### What is type conversion in JavaScript?

Type conversion is the process of converting data of one type to another. For example, converting string data to number.

There are two types of type conversion in JavaScript:

- **Implicit Conversion** - Automatic type conversion.

- **Explicit Conversion** - Manual type conversion.

### What is implicit conversion in JavaScript?

### What is explicit conversion in JavaScript?

### What is type coercion in JavaScript?

### What is the use of typeof operator?

The `typeof` operator used to determine the data type of a given variable or expression. It returns a string value indicating the type.

- `undefined`: Represents an undefined value.
- `boolean`: Indicates a boolean value (`true` or `false`).
- `number`: Refers to numeric values.
- `string`: Denotes textual values.
- `object`: Refers to non-primitive objects (e.g. {} or []).
- `function`: Indicates a function (including class constructors).
- `symbol`: Represents unique symbols.
- `bigint`: Represents large integer values (e.g.42n)

> `null` is also considered an object.

```sh
console.log(typeof 42); // "number"
console.log(typeof 'Hello'); // "string"
console.log(typeof true); // "boolean"
console.log(typeof undefined); // "undefined"
console.log(typeof { name: 'Alice' }); // "object"
console.log(typeof [1, 2, 3]); // "object"
console.log(typeof null); // "object" (this is a known quirk in JavaScript)
console.log(typeof function() {}); // "function"
console.log(typeof Symbol('symbol')); // "symbol"
console.log(typeof BigInt(1234567890123456789012345678901234567890)); // "bigint"
```

<!-- 3 -->

## Operators & Conditions

### What are operators? What are the types of operators in JavaScript?

Operators are symbols used to perform specific tasks on variables or values. They can be classified into several types:

1. **Arithmetic Operators:** Perform mathematical operations.

`+` (Addition): Adds values.

`-` (Subtraction): Subtracts values.

`-` (Subtraction): Subtracts values.

`-` (Subtraction): Subtracts values.

`-` (Subtraction): Subtracts values.

`-` (Subtraction): Subtracts values.

`-` (Subtraction): Subtracts values.

`-` (Subtraction): Subtracts values.

`-` (Subtraction): Subtracts values.

`-` (Subtraction): Subtracts values.

### What is the difference between unary, binary and ternary operator?

Operators can be classified based on the number of operands they work with:

1. **Unary Operators:** Operate on a single operand.

- `typeof` (Returns the type of a variable): `typeof` "hello" results in "string"
- `!` (Logical NOT): `!true` results in `false`
- `++` (Increment): `let a = 1; a++` results in `a` being `2`
- `--` (Decrement): `let b = 2; b--` results in `b` being `1`
- `-` (Unary negation): `-3` results in `-3`
- `+` (Unary plus): `+"3"` results in `3`

### What is short-circuit evaluation in JS?

Short-circuit evaluation refers to the evaluation of an expression from left to right using the logical operators `&&` (AND) and `||` (OR).

**Logical AND (&&)**

- The expression `a && b` evaluates `a` first.
- If `a` is `false`, the entire expression returns `false` without evaluating `b`.
- If `a` is `true`, the entire expression returns the value of `b`.

```sh
let a = 0;
let b = 1;

console.log(a && b); // Output: 0 (a is falsy, so b is not evaluated)
console.log(b && a); // Output: 0 (b is truthy, so a is evaluated and returned)
```

**Logical OR (||)**

- The expression `a || b` evaluates `a` first.
- If `a` is `true`, the entire expression returns `true` without evaluating `b`.
- If `a` is `false`, the entire expression returns the value of `b`.

```sh
let a = 0;
let b = 1;

console.log(a || b); // Output: 1 (a is falsy, so b is evaluated and returned)
console.log(b || a); // Output: 1 (b is truthy, so a is not evaluated)
```

### What is operator precedence?

Operator precedence determines the order in which operators are evaluated in expressions. Operators with higher precedence are given a higher priority than the operators with lower precedence.

When operators have equal precedence, they are generally evaluated from left to right.

```sh
let result = 2 + 3 * 4 - 1;
console.log(result);  // Output: 13
```

### What are rules for operator precedence?

Some most commonly used operators in JavaScript, ordered by precedence from highest to lowest:

- Grouping: `()`
- Multiplication: `*`, Division: `/`, Remainder: `%`
- Addition: `+`, Subtraction: `-`
- Relational: `<` `<=` `>` `>=`, in, instanceof

- Equality: `==` `!=` `===` `!==`
- Logical AND: `&&`
- Logical OR: `||`
- Conditional (Ternary) Operator: `? :`
- Assignment: `=` `+=` `-=` `*=` `/=` `%=` `**=` `<<=` `>>=` `>>>=` `&=` `^=` `|=` `&&=` `||=` `??=`

- Member Access: `.`, Computed Member Access: `[]`, new (with argument list): `new`
- Function Call: `()`
- new (without argument list): `new`
- Postfix Increment: `++`, Postfix Decrement: `--`
- Logical NOT: `!`, Bitwise NOT: `~`, Unary Plus: `+`, Unary Negation: `-`, Prefix Increment: `++`, Prefix Decrement: `--`, typeof, void, delete
- Exponentiation: `**`

- Bitwise Shift: `<<` `>>` `>>>`
- Bitwise AND: `&`
- Bitwise XOR: `^`
- Bitwise OR: `|`

- Nullish Coalescing: `??`
- Comma: `,`

### What are the types of conditions statements in JS?

Condition statements are used to perform different actions based on different conditions. There are sevral types of condition statements:

- **if Statement:** Executes a block of code if a specified condition is true.

- **if...else Statement:** Executes one block of code if a condition is true and another block of code if the condition is false.

- **else if Statement:** Allows you to test multiple conditions. If one condition is true, a corresponding block of code is executed.

- **Nested if…else statement:** Allow us to create complex conditional logic by checking multiple conditions in a hierarchical manner.

- **switch Statement:** Evaluates an expression and executes the code corresponding to the matching case. The default case executes if no matching case is found.

- **Ternary Operator:** The ternary operator also known as the conditional operator, Its allows for a more concise and clearer way to perform conditional logic. It takes three operands and can be used as an alternative to the `if...else` statement.

```sh
# if Statement
if (condition) {
    // code to be executed if the condition is true
}


# if...else Statement
if (condition) {
    // code to be executed if the condition is true
} else {
    // code to be executed if the condition is false
}


# else if Statement
if (condition1) {
    // code to be executed if condition1 is true
} else if (condition2) {
    // code to be executed if condition2 is true
} else {
    // code to be executed if neither condition1 nor condition2 is true
}


# Nested if…else statement
if (condition1) {
    // code block 1
    if (condition2) {
        // code block 2
    } else {
        // code block 3
    }
} else {
    // code block 4
}

# switch Statement
switch (expression) {
    case value1:
        // code to be executed if expression === value1
        break;
    case value2:
        // code to be executed if expression === value2
        break;
    // more cases...
    default:
        // code to be executed if no case matches
}


# Ternary Operator
condition ? expr1 : expr2
```

### When to use which type of conditions statements in real application?

`if...else`, `switch`, and ternary `(?:)` conditions are used for decision-making. Each has its own use cases and syntax.

- **if...else**: The `if...else` statement is used for executing a block of code based on a condition. It allows multiple conditions through `else if` blocks.

- **switch**: The `switch` statement is used for comparing a single expression against multiple possible cases. It's useful when you need to compare one variable against multiple values.

- **Ternary Operator**: The ternary operator (`?:`) is a shorthand for an `if...else` statement. It is best used for simple conditions.

-

```sh
if (condition1) {
    // code to execute if condition1 is true
} else if (condition2) {
    // code to execute if condition2 is true
} else {
    // code to execute if none of the conditions is true
}
```

```sh
switch (expression) {
   case value1:
      // code to execute if expression === value1
      break;
   case value2:
      // code to execute if expression === value2
      break;
      // more cases
   default:
      // code to execute if no case matches
}
```

```sh
condition ? expressionIfTrue : expressionIfFalse
```

### What is the difference between == and ===?

`==` and `===` equals are both comparison operators, but they function differently:

- The `==` operator compares values loosely. it compare values with type coercion.

- On the other hand, the `===` operator performs a strict comparison. It compares both values and their data types without any type conversion.

```sh
# Because of type coercion, different types can be considered equal.
console.log(5 == "5"); // true
console.log(0 == false); // true
console.log(null == undefined); // true


# Both the type and the value must be the same for the comparison.
console.log(5 === "5"); // false
console.log(0 === false); // false
console.log(null === undefined); // false
```

### What is the difference between Spread and Rest operator in JS?

Both the spread operator (`...`) and the rest parameter (`...`) use the same syntax, but they serve different purposes depending on the context.

- The **spread operator** is used to expand elements from an iterable such as an array, string, or object into individual elements.

  - It is commonly used to:
    - Copy arrays & objects
    - Merge (combine) arrays, strings or objects
    - Pass array elements as arguments to a function
    - Create shallow copies of arrays or objects.

```sh
# Array
const arr1 = [1, 2, 3];
const arr2 = [...arr1, 4, 5, 6]; // [1, 2, 3, 4, 5, 6]

const sum = (a, b, c) => a + b + c;
console.log(sum(...arr1)); // 6

# Object
const obj1 = { a: 1, b: 2 };
const obj2 = { ...obj1, c: 3 }; // { a: 1, b: 2, c: 3 }

# Shallow Copy
const originalArray = [1, 2, 3];
const shallowCopy = [...originalArray];

console.log(shallowCopy); // [1, 2, 3]
console.log(shallowCopy === originalArray); // false (they are different arrays)

// Modifying the copy does not affect the original
shallowCopy.push(4);
console.log(originalArray); // [1, 2, 3]
console.log(shallowCopy);   // [1, 2, 3, 4]
```

- The **rest parameter** allows a function to accept an indefinite number of arguments as an array.

  - Used in function parameters and destructuring assignments.
  - It collects remaining arguments into an array & will be the last argument.

```sh
# Function Parameters
function sum(...numbers) {
  return numbers.reduce((acc, curr) => acc + curr, 0);
}

console.log(sum(1, 2, 3, 4)); // 10

# Array Destructuring
const [first, second, ...rest] = [1, 2, 3, 4, 5];

console.log(first); // 1
console.log(second); // 2
console.log(rest); // [3, 4, 5]

# Collects remaining arguments into an array
function concatenateStrings(separator, ...strings) {
  return strings.join(separator);
}

console.log(concatenateStrings(", ", "apple", "banana", "cherry")); // "apple, banana, cherry"
```

### What is use of Rest operator in JS?

<!-- 4 -->

## Loops

### What is loop? What are the types of loops in JS?

Loops are used to perform repeated tasks based on a condition. Conditions typically return `true` or `false`. A loop will continue running until the defined condition returns `false`.

There are five types of loops:

1. `for` Loop
2. `while` Loop
3. `do...while` Loop
4. `for...in` Loop
5. `for...of` Loop

### What is for loop?

The `for` loop is used when you know the exact number of iterations or need to manipulate the loop index.

It consists of three parts: initialization, condition, and increment/decrement.

```sh
# Syntax
for (initialization; condition; increment) {
    // code to be executed
}

# Example
for (let i = 0; i < 5; i++) {
    console.log(i); // Outputs 0, 1, 2, 3, 4
}
```

### What is while loop?

The `while` loop repeats a block of code as long as the specified condition is true. It is useful when the number of iterations is not known in advance.

```sh
# Syntax
while (condition) {
    // code to be executed
}

# Example
let i = 0;
while (i < 5) {
    console.log(i); // Outputs 0, 1, 2, 3, 4
    i++;
}
```

### What is do...while loop?

The `do...while` loop is similar to the while loop, but it guarantees that the code block is executed at least once before the condition is tested.

```sh
# Syntax
do {
    // code to be executed
} while (condition);

# Example
let i = 0;
do {
    console.log(i); // Outputs 0, 1, 2, 3, 4
    i++;
} while (i < 5);
```

### What is for...in loop?

The `for...in` loop used for iterating over the properties of an object, including inherited properties.

```sh
# Syntax
for (key in object) {
    // code to be executed
}

# Example
let obj = {a: 1, b: 2, c: 3};
for (let key in obj) {
    console.log(key + ": " + obj[key]); // Outputs "a: 1", "b: 2", "c: 3"
}
```

### What is for...of loop?

The `for...of` loop used for iterating over the values of an iterable object like arrays, strings, maps, sets, and more.

```sh
# Syntax
for (value of iterable) {
    // code to be executed
}

# Example
let array = [1, 2, 3, 4, 5];
for (let value of array) {
    console.log(value); // Outputs 1, 2, 3, 4, 5
}
```

### What is the difference between while and for loop?

Both `while` and `for` loops are used for repeating a block of code as long as a specified condition is true. But they have some key differences like:

- **Use Case**: `while` best for when you don't know the number of iterations in advance but `for` loop typically used when you know the number of iterations.

- **Initialization**: `while` loop initialization and increment/decrement are usually outside the loop but `for` loop initialization, condition, and increment/decrement are part of the loop declaration.

- **Readability**: `while` loop can be more readable when dealing with complex conditions but `for` loop is more compact and easier to read when you have a simple loop with a known number of iterations.

### What is the difference between while and do-while loops?

Both `while` and `do-while` loops are used for repeating a block of code as long as a specified condition is true. But they have some key differences like:

- **Condition Checking**: `while` loop checks the condition first, then executes the code block but `do...while` loop executes the code block first, then checks the condition.

- **Guarantee of Execution**: `while` loop has no guarantee of execution if the initial condition is false but `do...while` loop guarantees that the loop's body will execute at least once.

- **Syntax**: `while` loop condition added at the beginning but `do...while` condition added at the end.

- **Use Caes**: `while` loop

```sh
# While Loop
let i = 10;
while (i < 5) {
    console.log(i); // This will not execute because the condition is false initially.
    i++;
}
```

```sh
# Do While Loop
let i = 10;
do {
    console.log(i); // This will execute once even though the condition is false.
    i++;
} while (i < 5);
```

### What is the difference between break and continue statement?

### What is the difference between for and for...of loop in JavaScript?

### What is the difference between for...of and for...in loops in JavaScript?

### What is forEach method? Compare it with for...of and for...in loop?

### When to use for...of loop and when to use forEach method in application?

<!-- 5 -->

## String

### What is a String?

### What are template literals and string interpolation in string?

### Difference between single quote(''), doible quote("") and backticks(``)?

### What are some important string operations in JS?

### What is string immutability?

### In how many ways you can concatenate strings?

<!-- 6 -->

## Array

### What are Arrays in JS? How to get, add & remove elements from arrays?

### What is the indexOf() method of an Array?

### What is the difference between find() and filter() methods of an Array?

### What is the slice() method of an Array?

### What is the difference between push() and concat() method of an Array?

### What is the difference between pop() and shift() methods of an Array?

### What is the splice() method of an Array?

### Difference between the slice() and splice() methods of an Array?

### What is the difference map() and forEach() array methods of an Array?

### How to sort and reverse an array?

### What is Array Destructuring in JS?

### What are array-like objects in JS?

### How to convert an array-like object into an array?

<!-- 7 -->

## Objects

### What are Objects in JavaScript?

### In how many ways we can create an object?

### What is the difference between an array and an object?

### How do you add or modify or delete properties of an object?

### Explain the difference between dot notation and bracket notation?

### What are some common methods to iterate over the properties of an object?

### How do you check if a property exists in an object?

### How do you clone or copy an object?

### What is the difference between deep copy and shallow copy in JS?

### What is Set Object in JS?

### What is Map Object in JS?

### What is the difference between Map and Object in JS?

<!-- 8 -->

## Functions

### What are Functions in JS? What are the types of function?

### Difference between named and anonymous functions?

### What is function expression in JS?

### What are Arrow Functions in JS? What is use of it?

### What are Callback Functions? What is it use?

### What is Higher-order function in JS?

### What is difference between arguments and parameters?

### In how many ways can you pass arguments to a function?

### How do you use default parameters in a function?

### What is the use of event handling in JS?

### What are First-Class functions in JS?

### What are Pure and Impure functions in JS?

### What is Function Currying in JS?

### What are call, apply, and bind methods in JS?

<!-- 9 -->

## DOM

### What is DOM? What is the difference between HTML and DOM?

### How do you select, modify, create and remove DOM elements?

### What are selectors in JavaScript?

### Difference getElementById, getElementByClassName and getElementByTagName?

### What is the difference between querySelector() and querySelectorAll()?

### What are the methods to modify elements properties and attributes?

### What is the difference between innerHTML and textContent?

### How to add and remove properties HTML elements in the DOM using JS?

### How to add and remove style from HTML elements in DOM using JS?

### Create new elements in DOM using JS?

### What is the difference between createElement() and createTextNode()?

<!-- 10 -->

## Error Handling

### What is Error Handling in JS?

### What is the role of finally block in JS?

### What is the purpose of the throw statement in JS?

### What is Error propagation in JS?

### What are the best practices for error handling?

### What are the different types of errors in JS?

### What is Try...Catch...Finally in JS?

<!-- 11 -->

## Events

### What are Events? How are events triggered?

### What are the types of events in JS?

### What is Event Object in JS?

### What is Event Delegation in JS?

### What is Event Bubbling in JS?

### How can you stop event propagation or event bubbling in JS?

### What is Event Capturing in JS?

### What is the purpose of the event.preventDefault() method in JS?

### What is the use of "this" keyword in the content of event handling in JS?

### How to remove an event handler from an element in JS?

### What is Debouncing?

### What is Throttling?

<!-- 11 -->

## Asynchronous Programming

### What is asynchronous programming in JavaScript? What is its use?

### What is difference between synchronous and asynchronous programming?

### What are the techniques for achieving asynchronous operations in JS?

### What is setTimeout()? How is it used to handle asynchronous operations?

### What is setInterval()? How is it used to handle asynchronous operations?

### What is the role of callback in fetching API data asynchronously?

### What is callback hell? How can it be avoided?

### What are Promises in JavaScript?

### How to implement Promises in JavaScript?

### When to use Promises in real application?

### What is the use of Promise.all() method?

### What is the use of Promise.race() method?

### What is difference between Promise.all() and Promise.race() method?

### What is Async/Await in JS?

### What is the purpose of async/await? Compare it with Promises?

### Explain the use of async and await keywords in JS?

### Can we use async keyword without await keyword and vice versa?

### How do you handle errors in async/await functions?

<!-- 12 -->

## Debugging

### How many ways to debug JavaScript code?

### What is the role of Debugger keyword?

<!-- 13 -->

## BOM & Web Storage

### What is window object?

### What are Browser APIs in JS?

### What is Web Storage and its use? How many types of web storage are there?

### What is Local Storage? How to store, retrive and remove data from it?

### What is difference between LocalStorage and SessionStorage?

### How much data can be stored in localStorage and sessionStorage?

### What are cookies? How do you create and read cookies?

### What is the difference between cookies and web storage?

### When to use cookies and when to use web storage?

<!-- 14 -->

## OOPs

### What are Classes in JS?

### What is a constructor?

### What are constructor functions?

### What is use of this keyword?

### Explain the concept of prototypal inheritance?

<!-- 15 -->

## Security & Performance

### What is eval() function in JS?

### What is XSS (Cross-Site Scripting) attack?

### What is SQL Injection attack?

### What are some best practices for security in JS?

### What are the best practices for improving performance in JS?

<!-- 16 -->

## ECMAScript 6 (ES6)

### What is ES6? What are some new features introduced by it?

### What are Modules in JS?

### What is the role of export keyword?

### What are the advantages of modules?

### What is the difference between named exports and default exports?

### What is the difference between static and dynamic imports?

### What are module bundlers?

<!-- 17 -->

## Advanced

### What is Strict Mode ("use strict") in JS?

### What is Hoisting in JS & how does it works?

### What is JSON?

### What is Scope in JavaScript?

### What is Scope Chain in JS?

### Explain the concept of Lexical Scoping?

### What is Clouser?

### What are the benefits of Closures?

### What is the concept of Encapsulation in the context of closures?

### What are the disadvantage or limitations of Closures?

### How can you release the variable references or closures from memory?

### What is the difference between a Regular Function and a Closure?

### What is "this" keyword?

### What is Event Loop in JS?

### What is role of event loop in JavaScript?

```sh
https://www.w3schools.com/js/js_statements.asp

https://javascript.info/

https://www.javascripttutorial.net/

https://www.tutorialspoint.com/javascript/index.htm

https://www.geeksforgeeks.org/javascript/

https://www.javatpoint.com/javascript-tutorial

https://www.simplilearn.com/tutorials/javascript-tutorial

https://www.codecademy.com/learn/introduction-to-javascript

```

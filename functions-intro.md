# Intro to Functions

Functions are one of the fundamental building blocks in JavaScript. A function is a JavaScript procedure—a set of statements that performs a task or calculates a value. To use a function, you must define it somewhere in the scope from which you wish to call it.

## Defining functions
Function declarations
A function definition (also called a function declaration, or function statement) consists of the function keyword, followed by:

The name of the function.
A list of parameters to the function, enclosed in parentheses and separated by commas.
The JavaScript statements that define the function, enclosed in curly brackets, {...}.
For example, the following code defines a simple function named square:

```javascript
function square(number) {
  return number * number;
}
```
The function square takes one parameter, called number. The function consists of one statement that says to return the parameter of the function (that is, number) multiplied by itself. The statement return specifies the value returned by the function:

```javascript
return number * number;
```

write once, use many times

```javascript
// Declare the function
function add(a, b) {
  return a + b;
}
// Call the function
add(1, 3);
// 4
```

```javascript
function add() {
  // this code gets executed when called.
  return a + b;
}
add();
// still use () so js knows we are calling a function
```
### The functions return value
the return keyword tells js to return the value which the expression following it evaluates to
functions don't have to have a return value. if a functions doesn't return anything, undefined is returned.
functions stop executing when they reach a return statement.
```javascript
function add(a, b) {
  // this code gets executed when called.
  console.log('add', a, b);
  // the return statement
  return a + b;
}

// Call the function
add(1, 3);
// 4
```
### Calling functions
add(1, 5);
function calls are an expression.

We can assign the result of function calls to variables, we can use it where a value is used
```javascript

function add(a, b) {
  return a + b;
}
console.log(add(2, 3));

var a = add(1, 2);
var b = add(2, 3);

console.log(a, b);

// 5
// 3 5
```

```javascript
function add(a, b) {
  return a + b;
}

var a = add(1, 2) + add(2, 3);

console.log(a);

// 8
```
#### nested function calls
```javascript
var a = add(add(2, 2) 2);

console.log(a);

// 6. the 1st add is the function call. the first argument is a function, 2nd is 2.
```
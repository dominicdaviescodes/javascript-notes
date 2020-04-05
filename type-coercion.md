# Type coercion
Type coercion is the automatic or implicit conversion of values from one data type to another (such as strings to numbers). Type conversion is similar to type coercion because they both convert values from one data type to another with one key difference — type coercion is implicit whereas type conversion can be either implicit or explicit.

```javascript
const value1 = '5';
const value2 = 9;
let sum = value1 + value2;

console.log(sum);

// 59
```
In the above example, JavaScript has coerced the 9 from a number into a string and then concatenated the two values together, resulting in a string of 59. JavaScript had a choice between a string or a number and decided to use a string.

The compiler could have coerced the 5 into a number and returned a sum of 14, but it did not. To return this result, you'd have to explicitly convert the 5 to a number using the Number() method:

```javascript
sum = Number(value1) + value2;
```

Dynamically typed (types are known at run time. JS) v static typed (c, c++, java)
```javascript
var greeting = 10;
greeting = 'hello';
```
in js we can assign a number to a variable and then assign a string to it.
```javascript
var a = '1';
var b = 2;
a + b
// 12
```
js temporarily makes one type into the other to make it all work.
we can use Number to convert string to number
```javascript
var a = '1';
var b = 2;
var sum = Number(a) + Number(b);

console.log(sum);
// 3
```
can change other types in console
```javascript
Number(true)
// pass it value true and it converts it to the number 1

Boolean(1)
// true ( converts to Boolean)

string(5)
// '5'  (converts number 5 to string '5')

```


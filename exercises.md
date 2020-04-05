# Exercises, Variables and Numbers

I want you to edit this code such that the value of result is the average of the numerical values of a, b,c and d, rounded up to the nearest whole number. Note the variables are currently strings, but I want the average of the numerical values.

Do this without editing the values that a, b, c and d are assigned.

Next I want you to assign the value of a random die roll to randomDieRoll. A die of course has six sides, so the result should be created by generating a random number between 1 and 6, inclusive.

```javascript
var a = '10';
var b = '5';
var c = '20';
var d = '30';

var result;

var randomDieRollOutcome;

```
1. Find average of var a to d, then round up to nearest whole number
2. use Number function to convert the strings
```javascript
var a = '10';
var b = '5';
var c = '20';
var d = '30';

var total = Number(a) + Number(b) + Number(c) + Number(d);

var result = Math.ceil(total / 4);
console.log(result);

// 17
```
generate a random die roll 
gotcha here is random number can be a zero and * 6 will only give us max of 5
answer is we + 1
```javascript
var randomDieRollOutcome = Math.floor(
  Math.random() * 6
) + 1;

console.log(randomDieRollOutcome);
```

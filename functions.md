## Functions

1. Define a function, as a function declaration, `maxOfTwoNumbers` that takes two numbers as arguments and returns the largest of them. If they are the same, return that number. Use the if-else construct or a ternary expression.  The Math.max method is not allowed.

Using if-else:
```javascript
function maxOfTwoNumbers(x,y) {
  if(x >= y) {
    return x;
  } else return y;
};
```

Using a ternary expression:
```javascript
function maxOfTwoNumbers(x,y) {
  return (x >= y ? x : y);
}
```

2. Define a function, as a function expression, `maxOfThree` that takes three numbers as arguments and returns the largest of them. Again, the Math.max method is not allowed.

```javascript
const maxOfThree = function(x,y,z) {
  if(x>=y && x>=z) return x;
  else if(y>=x && y>=z) return y;
  else return z;
};
```

3. Define a function, as a function declaration, `isCharAVowel` that takes a character as an argument and returns true if it is a vowel, false otherwise.

```javascript
const vowels = ['a', 'e', 'i', 'o', 'u'];

function isCharAVowel(char) {
  if(vowels.includes(char)) {
    return true;
  } else return false;
};
```

4. Define a function, as a function expression, `sumArray` that takes an array of numbers and returns the sum of those numbers.

```javascript
const numbers = [10, 5, 25, 6];

let total = 0;

const sumArray = function() {
  for(let i = 0; i<numbers.length; i++) {
    total += numbers[i];
  } return total;
};
```

5. Define a function, as a function declaration, `multiplyArray` that takes an array of numbers and returns the product of those numbers.

```javascript
const numbers = [10, 5, 25, 6];

let product = 1;

function multiplyArray() {
  for(let i = 0; i<numbers.length; i++) {
    product *= numbers[i];
  } return product;
};
```

6. Define a function, as a function expression, `numArgs` that returns the number of arguments passed to the function when called.

```javascript
const numArgs = function(...arguments) {
  return arguments.length;
};
```
# JavaScript Exercises

I wanted to collect some JavaScript exercises and my solutions for them in one place, instead of having them scattered across various repl.its and elsewhere on my computer. These exercises are taken from the assignments given to me in General Assembly's Software Engineering Immersive Remote Flex program, in which I am currently a student.

![I have no idea what I'm doing](https://i.imgur.com/FxhUPPf.png)

## Loops and Conditionals

1. Create a loop that logs the numbers from 0-99 ascending.

```javascript
for(let i=0; i<100; i++) {
  console.log(i);
};
```

2. Create a loop that logs the numbers from 99-0 descending.

```javascript
for(let i=99; i>=0; i--) {
  console.log(i);
};
```

3. Create a loop that logs the *even* numbers from 0-98 ascending.

```javascript
for(let i=0; i<=98; i++) {
  if(i % 2 === 0) {
    console.log(i);
  };
};
```

4. Create a loop that logs the *even* numbers from 98-0 descending.

```javascript
for(let i=98; i>=0; i--) {
  if(i % 2 === 0) {
    console.log(i);
  };
};
```

5. Create a loop that logs the *odd* numbers from 0-99 ascending.

```javascript
for(let i=0; i<=99; i++) {
  if(i === 0 || i % 2 !== 0) {
    console.log(i);
  };
};
```

6. Create a loop that logs the *odd* numbers from 99-0 descending.

```javascript
for(let i=99; i>=0; i--) {
  if(i % 2 !== 0 || i === 0) {
    console.log(i);
  };
};
```

7. Create a loop that logs the numbers from 49-72 ascending.

```javascript
for(let i=49; i<=72; i++) {
  console.log(i);
};
```

8. Create a loop that logs the numbers from 81-26 descending.

```javascript
for(let i=82; i>=26; i--) {
  console.log(i);
};
```

9. Create a loop that logs the numbers from 3-90 that are *multiples of 3* ascending.

```javascript
for(let i=3; i<=90; i++) {
  if(i % 3 === 0) {
    console.log(i);
  };
};
```


## Arrays

1. Define an empty array named 'foods'.

```javascript
const foods = [];
```

2. Add the strings 'pizza' and 'cheeseburger' to the foods array such that 'pizza' comes before 'cheeseburger'.

```javascript
foods.push('pizza', 'cheeseburger');
```

3. Add the string 'taco' to the foods array so that 'taco' is the first food in the array.

```javascript
foods.unshift('taco');
```

4. Access the string 'pizza' (based upon its known position) in the foods array and assign it to a variable named favFood.

```javascript
let favFood = foods[1];
```

5. Insert the string 'tofu' in the foods array between 'pizza' and 'cheeseburger'.

```javascript
foods.splice(2, 0, 'tofu');
```

6. Replace the string 'pizza' in the foods array with the strings 'sushi' and 'cupcake'.

```javascript
foods.splice(1, 1, 'sushi', 'cupcake');
```

7. Use the slice method on the foods array to create a new array containing 'sushi' and 'cupcake'. Assign the new array to a variable named 'yummy'.

```javascript
let yummy = foods.slice(1, 3);
```

8. Using the indexOf method on the foods array, assign the index of the 'tofu' string to a variable named soyIdx.

```javascript
let soyIdx = foods.indexOf('tofu');
```

9. Assign to a variable named allFoods the result of joining the strings in the foods array such that the result is the following single string: 'taco -> sushi -> cupcake -> tofu -> cheeseburger'

```javascript
let allFoods = foods.join([" -> "]);
```

10. Assign a boolean to a variable named hasSoup depending upon whether or not the foods array includes the string 'soup'.

```javascript
let hasSoup = foods.includes('soup');
```

11. Use the forEach method to iterate through the provided nums array and add each odd number to a new array named odds.

```javascript
const nums = [100, 5, 23, 15, 21, 72, 9, 45, 66, 7, 81, 90];
```

```javascript
let odds = [];

nums.forEach(function(num) {
  if(num % 2 !== 0) {
    odds.push(num);
  };
});
```

12. Use the forEach method to iterate through the same nums array and add the number to arrays named fizz, buzz, and/or fizzbuzz based on the following:
  * Add to the fizz array if the number is evenly divisible by 3
  * Add to the buzz array if the number is evenly divisible by 5
  * Add to the fizzbuzz array if the number is evenly divisible by 3 and 5

```javascript
const nums = [100, 5, 23, 15, 21, 72, 9, 45, 66, 7, 81, 90];
```

```javascript
let fizz = [];
let buzz = [];
let fizzbuzz = [];

nums.forEach(function(num) {
  if(num % 3 === 0 && num % 5 === 0) {
    fizzbuzz.push(num);
  };
  if(num % 3 === 0) {
    fizz.push(num);
  };
  if(num % 5 === 0) {
    buzz.push(num);
  };
});
```

13. Given the below numArrays array of arrays (two-dimensional array), assign the last nested array to a variable named numList. Assume you do not know how many nested arrays numArrays contains.

```javascript
const numArrays = [
	[100, 5, 23],
	[15, 21, 72, 9],
	[45, 66],
	[7, 81, 90]
];
```

```javascript
let numList = numArrays[numArrays.length - 1];
```

14. Given the below numArrays array, access the number 66 and assign to a variable named num.

```javascript
const numArrays = [
	[100, 5, 23],
	[15, 21, 72, 9],
	[45, 66],
	[7, 81, 90]
];
```

```javascript
let num = numArrays[2][1];
```

15. Given the below numArrays array, use nested forEach methods to sum up all the numbers contained within numArrays and assign to a variable named total.

```javascript
const numArrays = [
	[100, 5, 23],
	[15, 21, 72, 9],
	[45, 66],
	[7, 81, 90]
];
```

```javascript
let total = 0;

numArrays.forEach(function(numArray) {
  numArray.forEach(function(num) {
    total += num;
  });
  return total;
});
```
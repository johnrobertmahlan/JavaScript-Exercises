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
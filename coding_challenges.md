# Coding Challenges

### Challenge 1 - Sum Numbers

**Prompt:** Write a function called sumNumbers that accepts a single array of numbers and returns the sum of the numbers in the array. If the array is empty, return 0.

**Difficulty: Basic**

**Solution:** 
```javascript
let sum = 0;

function sumNumbers(arr) {
    for(let i=0; i<arr.length; i++) {
        sum += arr[i];
    };
    return sum;
};
```

### Challenge 2 - Add List

**Prompt:** Write a function called addList that accepts any quantity of numbers as arguments. Your function should add these numbers together and return the resulting sum. If called with no arguments, return 0.

**Difficulty: Basic**

**Solution:**
```javascript
let sum = 0;

function addList(...nums) {
    nums.forEach(function(num) {
        sum += num;
    });
    return sum;
};
```
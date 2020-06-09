# Recursion Problems

1. Define a function that returns the largest number in a given array.

```javascript
let largest = 0;

function findMax(arr, idx) {
    if(idx === arr.length) return largest;
    if(arr[idx] > largest) {
        largest = arr[idx];
    }
    return findMax(arr, idx + 1);
};
```

2. Define a function that returns the factorial of a given integer.

```javascript
let factorial = 1;

function findFactorial(num) {
    if(num === 1) return factorial;
    factorial *= num;
    return findFactorial(num - 1);
};
```
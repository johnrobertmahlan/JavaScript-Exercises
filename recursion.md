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
# JavaScript Exercises

I wanted to collect some JavaScript exercises and my solutions for them in one place, instead of having them scattered across various repl.its and elsewhere on my computer. These exercises are taken from the assignments given to me in General Assembly's Software Engineering Immersive Remote Flex program, in which I am currently a student.

![I have no idea what I'm doing](https://i.imgur.com/FxhUPPf.png)

## Loops and Conditionals

1. Create a loop that logs the numbers from 0-99 ascending.

Solution: 
```javascript
for(let i=0; i<100; i++) {
  console.log(i);
};
```

2. Create a loop that logs the numbers from 99-0 descending.

Solution:
```javascript
for(let i=99; i>=0; i--) {
  console.log(i);
};
```

3. Create a loop that logs the *even* numbers from 0-98 ascending.

Solution: 
```javascript
for(let i=0; i<=98; i++) {
  if(i % 2 === 0) {
    console.log(i);
  };
};
```

4. Create a loop that logs the *even* numbers from 98-0 descending.

Solution:
```javascript
for(let i=98; i>=0; i--) {
  if(i % 2 === 0) {
    console.log(i);
  };
};
```

5. Create a loop that logs the *odd* numbers from 0-99 ascending.

Solution:
```javascript
for(let i=0; i<=99; i++) {
  if(i === 0 || i % 2 !== 0) {
    console.log(i);
  };
};
```

6. Create a loop that logs the *odd* numbers from 99-0 descending.

Solution:
```javascript
for(let i=99; i>=0; i--) {
  if(i % 2 !== 0 || i === 0) {
    console.log(i);
  };
};
```

7. Create a loop that logs the numbers from 49-72 ascending.

Solution:
```javascript
for(let i=49; i<=72; i++) {
  console.log(i);
};
```

8. Create a loop that logs the numbers from 81-26 descending.

Solution:
```javascript
for(let i=82; i>=26; i--) {
  console.log(i);
};
```

9. Create a loop that logs the numbers from 3-90 that are *multiples of 3* ascending.

Solution:
```javascript
for(let i=3; i<=90; i++) {
  if(i % 3 === 0) {
    console.log(i);
  };
};
```
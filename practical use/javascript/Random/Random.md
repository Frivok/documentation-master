# Random

- [Random](#random)
- [Math.random()](#mathrandom)
- [JavaScript Random Integers](#javascript-random-integers)
- [A Proper Random Function](#a-proper-random-function)

# Math.random()

```bash
Math.random() returns a random number between 0 (inclusive),  and 1 (exclusive):

Example

Math.random();              // returns a random number

Math.random() always returns a number lower than 1.
```

# JavaScript Random Integers

```bash
Math.random() used with Math.floor() can be used to return random integers.

Example

Math.floor(Math.random() * 10);     // returns a random integer from 0 to 9

Example

Math.floor(Math.random() * 11);      // returns a random integer from 0 to 10

Example

Math.floor(Math.random() * 100);     // returns a random integer from 0 to 99

Example

Math.floor(Math.random() * 101);     // returns a random integer from 0 to 100

Example

Math.floor(Math.random() * 10) + 1;  // returns a random integer from 1 to 10

Example

Math.floor(Math.random() * 100) + 1; // returns a random integer from 1 to 100
``` 

# A Proper Random Function

```bash
As you can see from the examples above, it might be a good idea to create a proper random function to use for all random integer purposes.

This JavaScript function always returns a random number between min (included) and max (excluded):

Example

function getRndInteger(min, max) {
  return Math.floor(Math.random() * (max - min) ) + min;
}

This JavaScript function always returns a random number between min and max (both included):

Example

function getRndInteger(min, max) {
  return Math.floor(Math.random() * (max - min + 1) ) + min;
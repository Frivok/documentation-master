# Javascript-Arrays-Sort

- [Javascript-Arrays-Sort](#javascript-arrays-sort)
- [Sorting an Array](#sorting-an-array)
- [Reversing an Array](#reversing-an-array)
- [Numeric Sort](#numeric-sort)
- [The Compare Function](#the-compare-function)
- [Sorting an Array in Random Order](#sorting-an-array-in-random-order)
- [The Fisher Yates Method](#the-fisher-yates-method)
- [Find the Highest (or Lowest) Array Value](#find-the-highest-or-lowest-array-value)
- [Using Math.max() on an Array](#using-mathmax-on-an-array)
- [Using Math.min() on an Array](#using-mathmin-on-an-array)

# Sorting an Array
```bash
The sort() method sorts an array alphabetically:

Example

var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.sort();        // Sorts the elements of fruits
```

# Reversing an Array
```bash
The reverse() method reverses the elements in an array.

You can use it to sort an array in descending order:

Example

var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.sort();        // First sort the elements of fruits
fruits.reverse();     // Then reverse the order of the elements  
```

# Numeric Sort
```bash
By default, the sort() function sorts values as strings.

This works well for strings ("Apple" comes before "Banana").

However, if numbers are sorted as strings, "25" is bigger than "100", because "2" is bigger than "1".

Because of this, the sort() method will produce incorrect result when sorting numbers.

You can fix this by providing a compare function:

Example

var points = [40, 100, 1, 5, 25, 10];
points.sort(function(a, b){return a - b});

Use the same trick to sort an array descending:

Example

var points = [40, 100, 1, 5, 25, 10];
points.sort(function(a, b){return b - a});
```

# The Compare Function

```bash

The purpose of the compare function is to define an alternative sort order.

The compare function should return a negative, zero, or positive value, depending on the arguments:

function(a, b){return a - b}

When the sort() function compares two values, it sends the values to the compare function, and sorts the values according to the returned (negative, zero, positive) value.

If the result is negative a is sorted before b.

If the result is positive b is sorted before a.

If the result is 0 no changes are done with the sort order of the two values.

Example:

The compare function compares all the values in the array, two values at a time (a, b).

When comparing 40 and 100, the sort() method calls the compare function(40, 100).

The function calculates 40 - 100 (a - b), and since the result is negative (-60),  the sort function will sort 40 as a value lower than 100.
```

# Sorting an Array in Random Order

```bash
Example

var points = [40, 100, 1, 5, 25, 10];
points.sort(function(a, b){return 0.5 - Math.random()});
```

# The Fisher Yates Method

```bash
The above example, array.sort(), is not accurate, it will favor some numbers over the others.

The most popular correct method, is called the Fisher Yates shuffle, and was introduced in data science as early as 1938!

In JavaScript the method can be translated to this:

Example

var points = [40, 100, 1, 5, 25, 10];

for (i = points.length -1; i > 0; i--) {
  j = Math.floor(Math.random() * i)
  k = points[i]
  points[i] = points[j]
  points[j] = k
}
```

# Find the Highest (or Lowest) Array Value

```bash
There are no built-in functions for finding the max or min value in an array.

However, after you have sorted an array, you can use the index to obtain the highest and lowest values.

Sorting ascending:
Example
var points = [40, 100, 1, 5, 25, 10];
points.sort(function(a, b){return a - b});
// now points[0] contains the lowest value
// and points[points.length-1] contains the highest value

Sorting descending:
Example
var points = [40, 100, 1, 5, 25, 10];
points.sort(function(a, b){return b - a});
// now points[0] contains the highest value
// and points[points.length-1] contains the lowest value

Sorting a whole array is a very inefficient method if you only want to find the highest (or lowest) value.
```

# Using Math.max() on an Array

```bash
You can use Math.max.apply to find the highest number in an array:
Example
function myArrayMax(arr) {
  return Math.max.apply(null, arr);
}

Math.max.apply(null, [1, 2, 3]) is equivalent to Math.max(1, 2, 3).
```

# Using Math.min() on an Array

```bash
You can use Math.min.apply to find the lowest number in an array:
Example
function myArrayMin(arr) {
  return Math.min.apply(null, arr);
}

Math.min.apply(null, [1, 2, 3]) is equivalent to Math.min(1, 2, 3).
```
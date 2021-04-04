# Javascript-Arrays

- [Javascript-Arrays](#javascript-arrays)
- [What is an Array?](#what-is-an-array)
- [Creating an Array](#creating-an-array)
- [Access the Elements of an Array](#access-the-elements-of-an-array)
- [Changing an Array Element](#changing-an-array-element)
- [Access the Full Array](#access-the-full-array)
- [Array Elements Can Be Objects](#array-elements-can-be-objects)
- [The length Property](#the-length-property)
- [Accessing the First Array Element](#accessing-the-first-array-element)
- [Looping Array Elements](#looping-array-elements)
- [Adding Array Elements](#adding-array-elements)

# What is an Array?

```bash
An array is a special variable, which can hold more than one value at a time.

If you have a list of items (a list of car names, for example), storing the cars in single variables could look like this:

var car1 = "Saab";

var car2 = "Volvo";

var car3 = "BMW";

However, what if you want to loop through the cars and find a specific one? And what if you had not 3 cars, but 300?

The solution is an array!

An array can hold many values under a single name, and you can access the values by referring to an index number.
```
# Creating an Array

```bash
Using an array literal is the easiest way to create a JavaScript Array.

Syntax:
var array_name = [item1, item2, ...];

Example
var cars = ["Saab", "Volvo", "BMW"];

```

# Access the Elements of an Array

```bash
You access an array element by referring to the index number.

This statement accesses the value of the first element in cars:

var name = cars[0];

Example
var cars = ["Saab", "Volvo", "BMW"];

document.getElementById("demo").innerHTML = cars[0]; 

```

# Changing an Array Element

```bash
This statement changes the value of the first element in cars:

cars[0] = "Opel";

Example
var cars = ["Saab", "Volvo", "BMW"];

cars[0] = "Opel";

document.getElementById("demo").innerHTML = cars[0];
```

# Access the Full Array

```bash
With JavaScript, the full array can be accessed by referring to the array name:

Example

var cars = ["Saab", "Volvo", "BMW"];

document.getElementById("demo").innerHTML = cars;
```

# Array Elements Can Be Objects

```bash
JavaScript variables can be objects. Arrays are special kinds of objects.

Because of this, you can have variables of different types in the same Array.

You can have objects in an Array. You can have functions in an Array. You can have arrays in an Array:
myArray[0] = Date.now;
myArray[1] = myFunction;
myArray[2] = myCars;
```

# The length Property

```bash
The length property of an array returns the length of an array (the number of array elements).

Example

var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.length;   // the length of fruits is 4

The length property is always one more than the highest array index.
```

# Accessing the First Array Element

```bash
Example

fruits = ["Banana", "Orange", "Apple", "Mango"];
var first = fruits[0];
```

# Looping Array Elements

```bash
The safest way to loop through an array, is using a for loop:

Example

var fruits, text, fLen, i;
fruits = ["Banana", "Orange", "Apple", "Mango"];
fLen = fruits.length;

text = "<ul>";
for (i = 0; i < fLen; i++) 
{
  text += "<li>" + fruits[i] + "</li>";
}
text += "</ul>";
```

# Adding Array Elements

```bash
The easiest way to add a new element to an array is using the push() method:

Example

var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.push("Lemon");    // adds a new element (Lemon) to fruits

New element can also be added to an array using the length property:

Example

var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits[fruits.length] = "Lemon";    // adds a new element (Lemon) to fruits 
```

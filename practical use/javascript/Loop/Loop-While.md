# Loop-While

- [Loop-While](#loop-while)
- [The While Loop](#the-while-loop)
- [The Do/While Loop](#the-dowhile-loop)
- [Comparing For and While](#comparing-for-and-while)

# The While Loop

```bash
The while loop loops through a block of code as long as a specified condition is true.

Syntax

while (condition) {
  // code block to be executed
}

Example

In the following example, the code in the loop will run, over and over again, as long as a variable (i) is less than 10:

Example

while (i < 10) {
  text += "The number is " + i;
  i++;
}

If you forget to increase the variable used in the condition, the loop will never end. This will crash your browser.
```

# The Do/While Loop

```bash
The do/while loop is a variant of the while loop. This loop will execute the code block once, before checking if the condition is true, then it will repeat the loop as long as the condition is true.

Syntax

do {
  // code block to be executed
}
while (condition);

Example

The example below uses a do/while loop. The loop will always be executed at least once, even if the condition is false, because the code block is executed before the condition is tested:

Example

do {
  text += "The number is " + i;
  i++;
}
while (i < 10);

Do not forget to increase the variable used in the condition, otherwise the loop will never end!
```

# Comparing For and While

```bash
If you have read the previous chapter, about the for loop, you will discover that a while loop is much the same as a for loop, with statement 1 and statement 3 omitted.

The loop in this example uses a for loop to collect the car names from the cars array:

Example

var cars = ["BMW", "Volvo", "Saab", "Ford"];
var i = 0;
var text = "";

for (;cars[i];) {
  text += cars[i] + "<br>";
  i++;
}

The loop in this example uses a while loop to collect the car names from the cars array:

Example

var cars = ["BMW", "Volvo", "Saab", "Ford"];
var i = 0;
var text = "";

while (cars[i]) {
  text += cars[i] + "<br>";
  i++;
}
```
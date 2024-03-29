# Math

- [Math](#math)
- [JavaScript Math Object](#javascript-math-object)
- [Math.round()](#mathround)
- [Math.pow()](#mathpow)
- [Math.sqrt()](#mathsqrt)
- [Math.abs()](#mathabs)
- [Math.ceil()](#mathceil)
- [Math.floor()](#mathfloor)
- [Math.sin()](#mathsin)
- [Math.cos()](#mathcos)
- [Math.min() and Math.max()](#mathmin-and-mathmax)
- [Math.random()](#mathrandom)
- [Math Properties (Constants)](#math-properties-constants)
- [Math Constructor](#math-constructor)
- [Math Object Methods](#math-object-methods)

# JavaScript Math Object

```bash
The JavaScript Math object allows you to perform mathematical tasks on numbers.

Example

Math.PI; // returns 3.141592653589793
```

# Math.round()

```bash
Math.round(x) returns the value of x rounded to its nearest integer:

Example

Math.round(4.7);    // returns 5
Math.round(4.4);    // returns 4
```

# Math.pow()

```bash
Math.pow(x, y) returns the value of x to the power of y:
Example
Math.pow(8, 2);      // returns 64
```

# Math.sqrt()

```bash
Math.sqrt(x) returns the square root of x:

Example

Math.sqrt(64);      // returns 8
```

# Math.abs()

```bash
Math.abs(x) returns the absolute (positive) value of x:

Example

Math.abs(-4.7);     // returns 4.7 

```
# Math.ceil()

```bash
Math.ceil(x) returns the value of x rounded up to its nearest integer:

Example

Math.ceil(4.4);     // returns 5 
```

# Math.floor()

```bash
Math.floor(x) returns the value of x rounded down to its nearest integer:

Example

Math.floor(4.7);    // returns 4
```

# Math.sin()

```bash
Math.sin(x) returns the sine (a value between -1 and 1) of the angle x (given in radians).

If you want to use degrees instead of radians, you have to convert degrees to radians:

Angle in radians = Angle in degrees x PI / 180.

Example

Math.sin(90 * Math.PI / 180);     // returns 1 (the sine of 90 degrees)
```

# Math.cos()

```bash
Math.cos(x) returns the cosine (a value between -1 and 1) of the angle x (given in radians).

If you want to use degrees instead of radians, you have to convert degrees to radians:

Angle in radians = Angle in degrees x PI / 180.

Example

Math.cos(0 * Math.PI / 180);     // returns 1 (the cos of 0 degrees)
```

# Math.min() and Math.max()

```bash
Math.min() and Math.max() can be used to find the lowest or highest value in a list of arguments:

Example

Math.min(0, 150, 30, 20, -8, -200);  // returns -200

Example

Math.max(0, 150, 30, 20, -8, -200);  // returns 150
```

# Math.random()

```bash
Math.random() returns a random number between 0 (inclusive), and 1 (exclusive):

Example

Math.random();     // returns a random number
```

# Math Properties (Constants)

```bash
JavaScript provides 8 mathematical constants that can be accessed with the Math object:

Example
Math.E        // returns Euler's number
Math.PI       // returns PI
Math.SQRT2    // returns the square root of 2
Math.SQRT1_2  // returns the square root of 1/2
Math.LN2      // returns the natural logarithm of 2
Math.LN10     // returns the natural logarithm of 10
Math.LOG2E    // returns base 2 logarithm of E
Math.LOG10E   // returns base 10 logarithm of E
```

# Math Constructor

```bash
Unlike other global objects, the Math object has no constructor. Methods and properties are static.

All methods and properties (constants) can be used without creating a Math object first.
```

# Math Object Methods

```bash
Method                  Description
abs(x)                  Returns the absolute value of x
acos(x)                 Returns the arccosine of x, in radians
acosh(x)                Returns the hyperbolic arccosine of x
asin(x)                 Returns the arcsine of x, in radians
asinh(x)                Returns the hyperbolic arcsine of x
atan(x)                 Returns the arctangent of x as a numeric value between -PI/2 and PI/2 radians
atan2(y, x)             Returns the arctangent of the quotient of its arguments
atanh(x)                Returns the hyperbolic arctangent of x
cbrt(x)                 Returns the cubic root of x
ceil(x)                 Returns x, rounded upwards to the nearest integer
cos(x)                  Returns the cosine of x (x is in radians)
cosh(x)                 Returns the hyperbolic cosine of x
exp(x)                  Returns the value of Ex
floor(x)                Returns x, rounded downwards to the nearest integer
log(x)                  Returns the natural logarithm (base E) of x
max(x, y, z, ..., n)    Returns the number with the highest value
min(x, y, z, ..., n)    Returns the number with the lowest value
pow(x, y)               Returns the value of x to the power of y
random()                Returns a random number between 0 and 1
round(x)                Rounds x to the nearest integer
sin(x)                  Returns the sine of x (x is in radians)
sinh(x)                 Returns the hyperbolic sine of x
sqrt(x)                 Returns the square root of x
tan(x)                  Returns the tangent of an angle
tanh(x)                 Returns the hyperbolic tangent of a number
trunc(x)                Returns the integer part of a number (x)
```

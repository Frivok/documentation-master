# Javascript-Date

- [Javascript-Date](#javascript-date)
- [Creating Date Objects](#creating-date-objects)
- [new Date()](#new-date)
- [new Date(year, month, ...)](#new-dateyear-month-)
- [Previous Century](#previous-century)
- [new Date(dateString)](#new-datedatestring)
- [Date Methods](#date-methods)

# Creating Date Objects

```bash
Date objects are created with the new Date() constructor.

There are 4 ways to create a new date object:

new Date()
new Date(year, month, day, hours, minutes, seconds, milliseconds)
new Date(milliseconds)
new Date(date string)
```

# new Date()

```bash
new Date() creates a new date object with the current date and time:

Example

var d = new Date();


Date objects are static. The computer time is ticking, but date objects are not.
```

# new Date(year, month, ...)

```bash
new Date(year, month, ...) creates a new date object with a specified date and time.

7 numbers specify year, month, day, hour, minute, second, and millisecond (in that order):

Example

var d = new Date(2018, 11, 24, 10, 33, 30, 0);

Note: JavaScript counts months from 0 to 11.

January is 0. December is 11.

6 numbers specify year, month, day, hour, minute, second:

Example

var d = new Date(2018, 11, 24, 10, 33, 30);

5 numbers specify year, month, day, hour, and minute:

Example

var d = new Date(2018, 11, 24, 10, 33);

4 numbers specify year, month, day, and hour:

Example

var d = new Date(2018, 11, 24, 10);

3 numbers specify year, month, and day:

Example

var d = new Date(2018, 11, 24);

2 numbers specify year and month:

Example

var d = new Date(2018, 11);

You cannot omit month. If you supply only one parameter it will be treated as milliseconds.

Example

var d = new Date(2018);
```

# Previous Century

```bash
One and two digit years will be interpreted as 19xx:

Example

var d = new Date(99, 11, 24);

Example

var d = new Date(9, 11, 24);
```

# new Date(dateString)

```bash
new Date(dateString) creates a new date object from a date string:

Example

var d = new Date("October 13, 2014 11:13:00");

Date strings are described in the next chapter.
JavaScript Stores Dates as Milliseconds

JavaScript stores dates as number of milliseconds since January 01, 1970, 00:00:00 UTC (Universal Time Coordinated).

Zero time is January 01, 1970 00:00:00 UTC.

Now the time is: 1603368749563 milliseconds past January 01, 1970

new Date(milliseconds)

new Date(milliseconds) creates a new date object as zero time plus milliseconds:

Example

var d = new Date(0);

01 January 1970 plus 100 000 000 000 milliseconds is approximately 03 March 1973:

Example

var d = new Date(100000000000);

January 01 1970 minus 100 000 000 000 milliseconds is approximately October 31 1966:

Example

var d = new Date(-100000000000);

Example

var d = new Date(86400000);

One day (24 hours) is 86 400 000 milliseconds.
```

# Date Methods

```bash
When a Date object is created, a number of methods allow you to operate on it.

Date methods allow you to get and set the year, month, day, hour, minute, second, and millisecond of date objects, using either local
time or UTC (universal, or GMT) time.


# Displaying Dates

```bash
JavaScript will (by default) output dates in full text string format:

Wed Mar 25 2015 01:00:00 GMT+0100 (heure normale d’Europe centrale)

When you display a date object in HTML, it is automatically converted to a string, with the toString() method.

Example

d = new Date();
document.getElementById("demo").innerHTML = d;

Same as:

d = new Date();
document.getElementById("demo").innerHTML = d.toString();

The toUTCString() method converts a date to a UTC string (a date display standard).

Example

var d = new Date();
document.getElementById("demo").innerHTML = d.toUTCString();

The toDateString() method converts a date to a more readable format:

Example

var d = new Date();
document.getElementById("demo").innerHTML = d.toDateString();

The toISOString() method converts a date to a string, using the ISO standard format:

Example

var d = new Date();
document.getElementById("demo").innerHTML = d.toISOString();
```




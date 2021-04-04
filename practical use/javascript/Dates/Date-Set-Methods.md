# Date-Set-Methods

- [Date-Set-Methods](#date-set-methods)
- [Set Date Methods](#set-date-methods)
- [The setFullYear() Method](#the-setfullyear-method)
- [The setMonth() Method](#the-setmonth-method)
- [The setDate() Method](#the-setdate-method)
- [The setHours() Method](#the-sethours-method)
- [The setMinutes() Method](#the-setminutes-method)
- [The setSeconds() Method](#the-setseconds-method)
- [Compare Dates](#compare-dates)

# Set Date Methods

```bash
Set Date methods are used for setting a part of a date:
Method                    Description
setDate()                 Set the day as a number (1-31)
setFullYear()             Set the year (optionally month and day)
setHours()                Set the hour (0-23)
setMilliseconds()         Set the milliseconds (0-999)
setMinutes()              Set the minutes (0-59)
setMonth()                Set the month (0-11)
setSeconds()              Set the seconds (0-59)
setTime()                 Set the time (milliseconds since January 1, 1970)
```

# The setFullYear() Method

```bash
The setFullYear() method sets the year of a date object. In this example to 2020:

Example

var d = new Date();

d.setFullYear(2020);
document.getElementById("demo").innerHTML = d;


The setFullYear() method can optionally set month and day:

Example

var d = new Date();

d.setFullYear(2020, 11, 3);
document.getElementById("demo").innerHTML = d;
```

# The setMonth() Method

```bash
The setMonth() method sets the month of a date object (0-11):

Example

var d = new Date();

d.setMonth(11);

document.getElementById("demo").innerHTML = d;
```

# The setDate() Method

```bash
The setDate() method sets the day of a date object (1-31):

Example

var d = new Date();
d.setDate(15);

document.getElementById("demo").innerHTML = d;

The setDate() method can also be used to add days to a date:

Example

var d = new Date();
d.setDate(d.getDate() + 50);

document.getElementById("demo").innerHTML = d;

If adding days shifts the month or year, the changes are handled automatically by the Date object.
```

# The setHours() Method

```bash
The setHours() method sets the hours of a date object (0-23):

Example

var d = new Date();

d.setHours(22);

document.getElementById("demo").innerHTML = d;
```

# The setMinutes() Method

```bash
The setMinutes() method sets the minutes of a date object (0-59):

Example

var d = new Date();

d.setMinutes(30);

document.getElementById("demo").innerHTML = d;
```

# The setSeconds() Method

```bash
The setSeconds() method sets the seconds of a date object (0-59):

Example

var d = new Date();

d.setSeconds(30);

document.getElementById("demo").innerHTML = d;
```

# Compare Dates

```bash
Dates can easily be compared.

The following example compares today's date with January 14, 2100:

Example

var today,
someday,
text;

today = new Date();

someday = new Date();

someday.setFullYear(2100, 0, 14);

if (someday > today)

 {
  text = "Today is before January 14, 2100.";
}

else

{
  text = "Today is after January 14, 2100.";
}

document.getElementById("demo")
.innerHTML = text;

JavaScript counts months from 0 to 11. January is 0. December is 11.
```

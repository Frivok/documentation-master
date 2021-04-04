# Date-Get-Methods
- [Date-Get-Methods](#date-get-methods)
- [JavaScript Get Date Methods](#javascript-get-date-methods)
- [The getTime() Method](#the-gettime-method)
- [The getFullYear() Method](#the-getfullyear-method)
- [The getMonth() Method](#the-getmonth-method)
- [The getDate() Method](#the-getdate-method)
- [The getHours() Method](#the-gethours-method)
- [The getSeconds() Method](#the-getseconds-method)
- [The getMilliseconds() Method](#the-getmilliseconds-method)
- [The getDay() Method](#the-getday-method)
- [UTC Date Methods](#utc-date-methods)

# JavaScript Get Date Methods

```bash
These methods can be used for getting information from a date object:
Method             Description
getFullYear()      Get the year as a four digit number (yyyy)
getMonth()         Get the month as a number (0-11)
getDate()          Get the day as a number (1-31)
getHours()         Get the hour (0-23)
getMinutes()       Get the minute (0-59)
getSeconds()       Get the second (0-59)
getMilliseconds()  Get the millisecond (0-999)
getTime()          Get the time (milliseconds since January 1, 1970)
getDay()           Get the weekday as a number (0-6)
Date.now()         Get the time. ECMAScript 5.
```

# The getTime() Method

```bash
The getTime() method returns the number of milliseconds since January 1, 1970:

Example

var d = new Date();

document.getElementById("demo").innerHTML = d.getTime();
```

# The getFullYear() Method

```bash
The getFullYear() method returns the year of a date as a four digit number:

Example

var d = new Date();

document.getElementById("demo").innerHTML = d.getFullYear();
```

# The getMonth() Method

```bash
The getMonth() method returns the month of a date as a number (0-11):

Example

var d = new Date();

document.getElementById("demo").innerHTML = d.getMonth();

In JavaScript, the first month (January) is month number 0, so December returns month number 11.

You can use an array of names, and getMonth() to return the month as a name:

Example

var d = new Date();

var months = ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"];

document.getElementById("demo").innerHTML = months[d.getMonth()];
```

# The getDate() Method

```bash
The getDate() method returns the day of a date as a number (1-31):

Example

var d = new Date();

document.getElementById("demo").innerHTML = d.getDate();
```

# The getHours() Method

```bash
The getHours() method returns the hours of a date as a number (0-23):

Example

var d = new Date();

document.getElementById("demo").innerHTML = d.getHours();

The getMinutes() Method

The getMinutes() method returns the minutes of a date as a number (0-59):

Example

var d = new Date();

document.getElementById("demo").innerHTML = d.getMinutes();
```

# The getSeconds() Method

```bash
The getSeconds() method returns the seconds of a date as a number (0-59):

Example

var d = new Date();

document.getElementById("demo").innerHTML = d.getSeconds();
```
# The getMilliseconds() Method

```bash
The getMilliseconds() method returns the milliseconds of a date as a number (0-999):

Example

var d = new Date();

document.getElementById("demo").innerHTML = d.getMilliseconds();
```

# The getDay() Method

```bash
The getDay() method returns the weekday of a date as a number (0-6):

Example

var d = new Date();

document.getElementById("demo").innerHTML = d.getDay();

In JavaScript, the first day of the week (0) means "Sunday", even if some countries in the world consider the first day of the week to be "Monday"

You can use an array of names, and getDay() to return the weekday as a name:

Example

var d = new Date();

var days = ["Sunday", "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday"];

document.getElementById("demo").innerHTML = days[d.getDay()];
```

# UTC Date Methods

```bash
UTC date methods are used for working with UTC dates

(Universal Time Zone dates):

Method                    Description

getUTCDate()              Same as getDate(), but returns the UTC date
getUTCDay()               Same as getDay(), but returns the UTC day
getUTCFullYear()          Same as getFullYear(), but returns the UTC year
getUTCHours()             Same as getHours(), but returns the UTC hour
getUTCMilliseconds()      Same as getMilliseconds(), but returns the UTC milliseconds
getUTCMinutes()           Same as getMinutes(), but returns the UTC minutes
getUTCMonth()             Same as getMonth(), but returns the UTC month
getUTCSeconds()           Same as getSeconds(), but returns the UTC seconds
```

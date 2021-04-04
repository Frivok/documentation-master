# Table of Contents
- [Table of Contents](#table-of-contents)
- [Horizontal Navigation Bar](#horizontal-navigation-bar)
- [Horizontal Navigation Bar Examples](#horizontal-navigation-bar-examples)
- [Active/Current Navigation Link](#activecurrent-navigation-link)
- [Right-Align Links](#right-align-links)
- [Fixed Navigation Bar](#fixed-navigation-bar)
- [Gray Horizontal Navbar](#gray-horizontal-navbar)
- [Sticky Navbar](#sticky-navbar)
- [More Examples](#more-examples)
- [Responsive Sidenav](#responsive-sidenav)
- [Dropdown Navbar](#dropdown-navbar)

# Horizontal Navigation Bar

```css
    Home
    News
    Contact
    About

There are two ways to create a horizontal navigation bar. Using inline or floating list items.

Inline List Items

One way to build a horizontal navigation bar is to specify the <li> elements as inline, in addition to the "standard" code from the previous page:

Example

li {
  display: inline;
}

Example explained:

    display: inline; - By default, <li> elements are block elements. Here, we remove the line breaks before and after each list item, to display them on one line

Floating List Items

Another way of creating a horizontal navigation bar is to float the <li> elements, and specify a layout for the navigation links:

Example

li {
  float: left;
}

a {
  display: block;
  padding: 8px;
  background-color: #dddddd;
}

Example explained:

    float: left; - use float to get block elements to slide next to each other
    display: block; - Displaying the links as block elements makes the whole link area clickable (not just the text), and it allows us to specify padding (and height, width, margins, etc. if you want)
    padding: 8px; - Since block elements take up the full width available, they cannot float next to each other. Therefore, specify some padding to make them look good
    background-color: #dddddd; - Add a gray background-color to each a element

Tip: Add the background-color to <ul> instead of each <a> element if you want a full-width background color:

Example

ul {
  background-color: #dddddd;
}
```

# Horizontal Navigation Bar Examples

```css
Create a basic horizontal navigation bar with a dark background color and change the background color of the links when the user moves the mouse over them:

    Home
    News
    Contact
    About

Example

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
}

li {
  float: left;
}

li a {
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

/* Change the link color to #111 (black) on hover */

li a:hover {
  background-color: #111;
}
```

# Active/Current Navigation Link

```css
Add an "active" class to the current link to let the user know which page he/she is on:

    Home
    News
    Contact
    About

Example

.active {
  background-color: #4CAF50;
}
```

# Right-Align Links

```css
Right-align links by floating the list items to the right (float:right;):

    Home
    News
    Contact
    About

Example

<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li style="float:right"><a class="active" href="#about">About</a></li>
</ul>

# Border Dividers

```css
Add the border-right property to <li> to create link dividers:

    Home
    News
    Contact
    About

Example

/* Add a gray right border to all list items, except the last item (last-child) */

li {
  border-right: 1px solid #bbb;
}

li:last-child {
  border-right: none;
}
```

# Fixed Navigation Bar

```css
Make the navigation bar stay at the top or the bottom of the page, even when the user scrolls the page:

Fixed Top

ul {
  position: fixed;
  top: 0;
  width: 100%;
}
Fixed Bottom

ul {
  position: fixed;
  bottom: 0;
  width: 100%;
}

Note: Fixed position might not work properly on mobile devices.
```

# Gray Horizontal Navbar

```css
An example of a gray horizontal navigation bar with a thin gray border:

    Home
    News
    Contact
    About

Example

ul {
  border: 1px solid #e7e7e7;
  background-color: #f3f3f3;
}

li a {
  color: #666;
}
```

# Sticky Navbar

```css
Add position: sticky; to <ul> to create a sticky navbar.

A sticky element toggles between relative and fixed, depending on the scroll position. It is positioned relative until a given offset position is met in the viewport - then it "sticks" in place (like position:fixed).

Example

ul {
  position: -webkit-sticky; /* Safari */
  position: sticky;
  top: 0;
}

Note: Internet Explorer, Edge 15 and earlier versions do not support sticky positioning. Safari requires a -webkit- prefix (see example above). You must also specify at least one of top, right, bottom or left for sticky positioning to work.
```

# More Examples

```css
Responsive Topnav

How to use CSS media queries to create a responsive top navigation.

<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
body {margin: 0;}

ul.topnav {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
}

ul.topnav li {float: left;}

ul.topnav li a {
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

ul.topnav li a:hover:not(.active) {background-color: #111;}

ul.topnav li a.active {background-color: #4CAF50;}

ul.topnav li.right {float: right;}

@media screen and (max-width: 600px) {
  ul.topnav li.right, 
  ul.topnav li {float: none;}
}
</style>
</head>
<body>

<ul class="topnav">
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li class="right"><a href="#about">About</a></li>
</ul>

<div style="padding:0 16px;">
  <h2>Responsive Topnav Example</h2>
  <p>This example use media queries to stack the topnav vertically when the screen size is 600px or less.</p>
  <p>You will learn more about media queries and responsive web design later in our CSS Tutorial.</p>
  <h4>Resize the browser window to see the effect.</h4>
</div>

</body>
</html>
```

# Responsive Sidenav

```css
How to use CSS media queries to create a responsive side navigation.

<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
body {margin: 0;}

ul.sidenav {
  list-style-type: none;
  margin: 0;
  padding: 0;
  width: 25%;
  background-color: #f1f1f1;
  position: fixed;
  height: 100%;
  overflow: auto;
}

ul.sidenav li a {
  display: block;
  color: #000;
  padding: 8px 16px;
  text-decoration: none;
}
 
ul.sidenav li a.active {
  background-color: #4CAF50;
  color: white;
}

ul.sidenav li a:hover:not(.active) {
  background-color: #555;
  color: white;
}

div.content {
  margin-left: 25%;
  padding: 1px 16px;
  height: 1000px;
}

@media screen and (max-width: 900px) {
  ul.sidenav {
    width: 100%;
    height: auto;
    position: relative;
  }
  
  ul.sidenav li a {
    float: left;
    padding: 15px;
  }
  
  div.content {margin-left: 0;}
}

@media screen and (max-width: 400px) {
  ul.sidenav li a {
    text-align: center;
    float: none;
  }
}
</style>
</head>
<body>

<ul class="sidenav">
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

<div class="content">
  <h2>Responsive Sidenav Example</h2>
  <p>This example use media queries to transform the sidenav to a top navigation bar when the screen size is 900px or less.</p>
  <p>We have also added a media query for screens that are 400px or less, which will vertically stack and center the navigation links.</p>
  <p>You will learn more about media queries and responsive web design later in our CSS Tutorial.</p>
  <h3>Resize the browser window to see the effect.</h3>
</div>

</body>
</html>
```

# Dropdown Navbar

```css
How to add a dropdown menu inside a navigation bar.

<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
}

li {
  float: left;
}

li a, .dropbtn {
  display: inline-block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover, .dropdown:hover .dropbtn {
  background-color: red;
}

li.dropdown {
  display: inline-block;
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f9f9f9;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  z-index: 1;
}

.dropdown-content a {
  color: black;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
  text-align: left;
}

.dropdown-content a:hover {background-color: #f1f1f1;}

.dropdown:hover .dropdown-content {
  display: block;
}
</style>
</head>
<body>

<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li class="dropdown">
    <a href="javascript:void(0)" class="dropbtn">Dropdown</a>
    <div class="dropdown-content">
      <a href="#">Link 1</a>
      <a href="#">Link 2</a>
      <a href="#">Link 3</a>
    </div>
  </li>
</ul>

<h3>Dropdown Menu inside a Navigation Bar</h3>
<p>Hover over the "Dropdown" link to see the dropdown menu.</p>

</body>
</html>
```
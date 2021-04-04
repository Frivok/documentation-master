# Table of Contents

- [Table of Contents](#table-of-contents)
- [Vertical Navigation Bar](#vertical-navigation-bar)
- [Vertical Navigation Bar Examples](#vertical-navigation-bar-examples)
- [Center Links & Add Borders](#center-links--add-borders)
- [Full-height Fixed Vertical Navbar](#full-height-fixed-vertical-navbar)

# Vertical Navigation Bar

```css
    Home
    News
    Contact
    About

To build a vertical navigation bar, you can style the <a> elements inside the list, in addition to the code from the previous page:

Example

li a {
  display: block;
  width: 60px;
}

Example explained:

    display: block; - Displaying the links as block elements makes the whole link area clickable (not just the text), and it allows us to specify the width (and padding, margin, height, etc. if you want)
    width: 60px; - Block elements take up the full width available by default. We want to specify a 60 pixels width

You can also set the width of <ul>, and remove the width of <a>, as they will take up the full width available when displayed as block elements. This will produce the same result as our previous example:

Example

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  width: 60px;
}

li a {
  display: block;
}
```

# Vertical Navigation Bar Examples

```css
Create a basic vertical navigation bar with a gray background color and change the background color of the links when the user moves the mouse over them:

    Home
    News
    Contact
    About

Example

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  width: 200px;
  background-color: #f1f1f1;
}

li a {
  display: block;
  color: #000;
  padding: 8px 16px;
  text-decoration: none;
}

/* Change the link color on hover */
li a:hover {
  background-color: #555;
  color: white;
}

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
  color: white;
}
```

# Center Links & Add Borders

```css
Add text-align:center to <li> or <a> to center the links.

Add the border property to <ul> add a border around the navbar. If you also want borders inside the navbar, add a border-bottom to all <li> elements, except for the last one:

    Home
    News
    Contact
    About

Example

ul {
  border: 1px solid #555;
}

li {
  text-align: center;
  border-bottom: 1px solid #555;
}

li:last-child {
  border-bottom: none;
}
```

# Full-height Fixed Vertical Navbar

```css
Create a full-height, "sticky" side navigation:

Example

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  width: 25%;
  background-color: #f1f1f1;
  height: 100%; /* Full height */
  position: fixed; /* Make it stick, even on scroll */
  overflow: auto; /* Enable scrolling if the sidenav has too much content */
}
Note: This example might not work properly on mobile devices.
```
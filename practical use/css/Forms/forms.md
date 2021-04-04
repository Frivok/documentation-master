# Table of Contents
- [Table of Contents](#table-of-contents)
- [Styling Input Fields](#styling-input-fields)
- [Padded Inputs](#padded-inputs)
- [Bordered Inputs](#bordered-inputs)
- [Colored Inputs](#colored-inputs)
- [Focused Inputs](#focused-inputs)
- [Input with icon/image](#input-with-iconimage)
- [Animated Search Input](#animated-search-input)
- [Styling Textareas](#styling-textareas)
- [Styling Select Menus](#styling-select-menus)
- [Styling Input Buttons](#styling-input-buttons)
- [Responsive Form](#responsive-form)

# Styling Input Fields

```css
Use the width property to determine the width of the input field:
First Name

Example

input {
  width: 100%;
}

The example above applies to all <input> elements. If you only want to style a specific input type, you can use attribute selectors:

    input[type=text] - will only select text fields
    input[type=password] - will only select password fields
    input[type=number] - will only select number fields
    etc..
```

# Padded Inputs

```css
Use the padding property to add space inside the text field.

Tip: When you have many inputs after each other, you might also want to add some margin, to add more space outside of them:
First Name Last Name

Example

input[type=text] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
}

Note that we have set the box-sizing property to border-box. This makes sure that the padding and eventually borders are included in the total width and height of the elements.
```

# Bordered Inputs

```css
Use the border property to change the border size and color, and use the border-radius property to add rounded corners:

First Name

Example

input[type=text] {
  border: 2px solid red;
  border-radius: 4px;
}

If you only want a bottom border, use the border-bottom property:

First Name

Example

input[type=text] {
  border: none;
  border-bottom: 2px solid red;
}
```

# Colored Inputs

```css
Use the background-color property to add a background color to the input, and the color property to change the text color:

Example

input[type=text] {
  background-color: #3CBC8D;
  color: white;
}
```

# Focused Inputs

```css
By default, some browsers will add a blue outline around the input when it gets focus (clicked on). You can remove this behavior by adding outline: none; to the input.

Use the :focus selector to do something with the input field when it gets focus:

Example

input[type=text]:focus {
  background-color: lightblue;
}

Example

input[type=text]:focus {
  border: 3px solid #555;
}
```

# Input with icon/image

```css
If you want an icon inside the input, use the background-image property and position it with the background-position property. Also notice that we add a large left padding to reserve the space of the icon:

Example

input[type=text] {
  background-color: white;
  background-image: url('searchicon.png');
  background-position: 10px 10px;
  background-repeat: no-repeat;
  padding-left: 40px;
}
```

# Animated Search Input

```css
In this example we use the CSS transition property to animate the width of the search input when it gets focus. You will learn more about the transition property later, in our CSS Transitions chapter.

Example

input[type=text] {
  transition: width 0.4s ease-in-out;
}

input[type=text]:focus {
  width: 100%;
}
```

# Styling Textareas

```css
Tip: Use the resize property to prevent textareas from being resized (disable the "grabber" in the bottom right corner):
Some text...

Example

textarea {
  width: 100%;
  height: 150px;
  padding: 12px 20px;
  box-sizing: border-box;
  border: 2px solid #ccc;
  border-radius: 4px;
  background-color: #f8f8f8;
  resize: none;
}
```

# Styling Select Menus

```css
Example

select {
  width: 100%;
  padding: 16px 20px;
  border: none;
  border-radius: 4px;
  background-color: #f1f1f1;
}
```

# Styling Input Buttons

```css
Example

input[type=button], input[type=submit], input[type=reset] {
  background-color: #4CAF50;
  border: none;
  color: white;
  padding: 16px 32px;
  text-decoration: none;
  margin: 4px 2px;
  cursor: pointer;
}

/* Tip: use width: 100% for full-width buttons */
```

# Responsive Form

```css
Resize the browser window to see the effect. When the screen is less than 600px wide, make the two columns stack on top of each other instead of next to each other.

Advanced: The following example use media queries to create a responsive form. You will learn more about this in a later chapter.

<html>
<head>
<style>
* {
  box-sizing: border-box;
}

input[type=text], select, textarea {
  width: 100%;
  padding: 12px;
  border: 1px solid #ccc;
  border-radius: 4px;
  resize: vertical;
}

label {
  padding: 12px 12px 12px 0;
  display: inline-block;
}

input[type=submit] {
  background-color: #4CAF50;
  color: white;
  padding: 12px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  float: right;
}

input[type=submit]:hover {
  background-color: #45a049;
}

.container {
  border-radius: 5px;
  background-color: #f2f2f2;
  padding: 20px;
}

.col-25 {
  float: left;
  width: 25%;
  margin-top: 6px;
}

.col-75 {
  float: left;
  width: 75%;
  margin-top: 6px;
}

/* Clear floats after the columns */
.row:after {
  content: "";
  display: table;
  clear: both;
}

/* Responsive layout - when the screen is less than 600px wide, make the two columns stack on top of each other instead of next to each other */
@media screen and (max-width: 600px) {
  .col-25, .col-75, input[type=submit] {
    width: 100%;
    margin-top: 0;
  }
}
</style>
</head>
<body>

<h2>Responsive Form</h2>
<p>Resize the browser window to see the effect. When the screen is less than 600px wide, make the two columns stack on top of each other instead of next to each other.</p>

<div class="container">
  <form action="/action_page.php">
  <div class="row">
    <div class="col-25">
      <label for="fname">First Name</label>
    </div>
    <div class="col-75">
      <input type="text" id="fname" name="firstname" placeholder="Your name..">
    </div>
  </div>
  <div class="row">
    <div class="col-25">
      <label for="lname">Last Name</label>
    </div>
    <div class="col-75">
      <input type="text" id="lname" name="lastname" placeholder="Your last name..">
    </div>
  </div>
  <div class="row">
    <div class="col-25">
      <label for="country">Country</label>
    </div>
    <div class="col-75">
      <select id="country" name="country">
        <option value="australia">Australia</option>
        <option value="canada">Canada</option>
        <option value="usa">USA</option>
      </select>
    </div>
  </div>
  <div class="row">
    <div class="col-25">
      <label for="subject">Subject</label>
    </div>
    <div class="col-75">
      <textarea id="subject" name="subject" placeholder="Write something.." style="height:200px"></textarea>
    </div>
  </div>
  <div class="row">
    <input type="submit" value="Submit">
  </div>
  </form>
</div>

</body>
</html>
```

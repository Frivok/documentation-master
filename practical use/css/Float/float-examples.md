# Table of Contents
- [Table of Contents](#table-of-contents)
- [With the float property, it is easy to float boxes of content side by side:](#with-the-float-property-it-is-easy-to-float-boxes-of-content-side-by-side)
- [Images Side By Side](#images-side-by-side)
- [Equal Height Boxes](#equal-height-boxes)
- [Navigation Menu](#navigation-menu)
- [Web Layout Example](#web-layout-example)
- [All CSS Float Properties](#all-css-float-properties)

# With the float property, it is easy to float boxes of content side by side:

```css
Example

* {
  box-sizing: border-box;
}

.box {
  float: left;
  width: 33.33%; /* three boxes (use 25% for four, and 50% for two, etc) */
  padding: 50px; /* if you want space between the images */
}

What is box-sizing?

You can easily create three floating boxes side by side. However, when you add something that enlarges the width of each box (e.g. padding or borders), the box will break. The box-sizing property allows us to include the padding and border in the box's total width (and height), making sure that the padding stays inside of the box and that it does not break.
```

# Images Side By Side

```css
The grid of boxes can also be used to display images side by side:

Example

.img-container {
  float: left;
  width: 33.33%; /* three containers (use 25% for four, and 50% for two, etc) */
  padding: 5px; /* if you want space between the images */
}
```

# Equal Height Boxes

```css
In the previous example, you learned how to float boxes side by side with an equal width. However, it is not easy to create floating boxes with equal heights. A quick fix however, is to set a fixed height, like in the example below:

Example

.box {
  height: 500px;
}

However, this is not very flexible. It is ok if you can guarantee that the boxes will always have the same amount of content in them. But many times, the content is not the same. If you try the example above on a mobile phone, you will see that the second box's content will be displayed outside of the box. This is where CSS3 Flexbox comes in handy - as it can automatically stretch boxes to be as long as the longest box:

Example

Using Flexbox to create flexible boxes:

<html>
<head>
<style>
.flex-container {
  display: flex;
  flex-wrap: nowrap;
  background-color: DodgerBlue;
}

.flex-container .box {
  background-color: #f1f1f1;
  width: 50%;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>
<h1>Flexible Boxes</h1>

<div class="flex-container">
  <div class="box">Box 1 - This is some text to make sure that the content gets really tall. This is some text to make sure that the content gets really tall.</div>
  <div class="box">Box 2 - My height will follow Box 1.</div>
</div>

<p>Try to resize the browser window to see the flexible layout.</p>
<p><strong>Note:</strong> Flexbox is not supported in Internet Explorer 10 or earlier versions.</p>

</body>
</html>
```

# Navigation Menu

```css
Use float with a list of hyperlinks to create a horizontal menu:

Example

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

li a {
  display: inline-block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover {
  background-color: #111;
}

.active {
  background-color: red;
}
</style>
</head>
<body>

<ul>
  <li><a href="#home" class="active">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>
```

# Web Layout Example

```css
It is also common to do entire web layouts using the float property:

Example

.header, .footer {
  background-color: grey;
  color: white;
  padding: 15px;
}

.column {
  float: left;
  padding: 15px;
}

.clearfix::after {
  content: "";
  clear: both;
  display: table;
}

.menu {
  width: 25%;
}

.content {
  width: 75%;
}
```

# All CSS Float Properties

```css
Property 	Description

box-sizing 	Defines how the width and height of an element are calculated: should they include padding and borders, or not
clear 	Specifies what elements can float beside the cleared element and on which side
float 	Specifies how an element should float
overflow 	Specifies what happens if content overflows an element's box
overflow-x 	Specifies what to do with the left/right edges of the content if it overflows the element's content area
overflow-y 	Specifies what to do with the top/bottom edges of the content if it overflows the element's content area
```
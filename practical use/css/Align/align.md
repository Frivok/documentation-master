# Table of Contents
- [Table of Contents](#table-of-contents)
- [Center Align Elements](#center-align-elements)
- [Center Align Text](#center-align-text)
- [Center an Image](#center-an-image)
- [Left and Right Align - Using position](#left-and-right-align---using-position)
- [Left and Right Align - Using float](#left-and-right-align---using-float)
- [The clearfix Hack](#the-clearfix-hack)
- [Center Vertically - Using padding](#center-vertically---using-padding)
- [Center Vertically - Using line-height](#center-vertically---using-line-height)
- [Center Vertically - Using position & transform](#center-vertically---using-position--transform)
- [Center Vertically - Using Flexbox](#center-vertically---using-flexbox)

# Center Align Elements

```css
To horizontally center a block element (like <div>), use margin: auto;

Setting the width of the element will prevent it from stretching out to the edges of its container.

The element will then take up the specified width, and the remaining space will be split equally between the two margins:

This div element is centered.

Example

.center {
  margin: auto;
  width: 50%;
  border: 3px solid green;
  padding: 10px;
}
Note: Center aligning has no effect if the width property is not set (or set to 100%).
```

# Center Align Text

```css
To just center the text inside an element, use text-align: center;

This text is centered.

Example

.center {
  text-align: center;
  border: 3px solid green;
}
```

# Center an Image

```css
To center an image, set left and right margin to auto and make it into a block element:

Example

img {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 40%;
}
```

# Left and Right Align - Using position

```css
One method for aligning elements is to use position: absolute;:

Example

.right {
  position: absolute;
  right: 0px;
  width: 300px;
  border: 3px solid #73AD21;
  padding: 10px;
}

Note: Absolute positioned elements are removed from the normal flow, and can overlap elements.
```

# Left and Right Align - Using float

```css
Another method for aligning elements is to use the float property:

Example

.right {
  float: right;
  width: 300px;
  border: 3px solid #73AD21;
  padding: 10px;
}

Note: If an element is taller than the element containing it, and it is floated, it will overflow outside of its container. You can use the "clearfix" hack to fix this (see example below).
```

# The clearfix Hack

```css
We can add overflow: auto; to the containing element to fix this problem:

Example

.clearfix {
  overflow: auto;
}
```

# Center Vertically - Using padding

```css
There are many ways to center an element vertically in CSS. A simple solution is to use top and bottom padding:

I am vertically centered.

Example

.center {
  padding: 70px 0;
  border: 3px solid green;
}

To center both vertically and horizontally, use padding and text-align: center:

I am vertically and horizontally centered.

Example

.center {
  padding: 70px 0;
  border: 3px solid green;
  text-align: center;
}
```

# Center Vertically - Using line-height

```css
Another trick is to use the line-height property with a value that is equal to the height property:

I am vertically and horizontally centered.

Example

.center {
  line-height: 200px;
  height: 200px;
  border: 3px solid green;
  text-align: center;
}

/* If the text has multiple lines, add the following: */
.center p {
  line-height: 1.5;
  display: inline-block;
  vertical-align: middle;
}
```

# Center Vertically - Using position & transform

```css
If padding and line-height are not options, another solution is to use positioning and the transform property:

I am vertically and horizontally centered.

Example

.center {
  height: 200px;
  position: relative;
  border: 3px solid green;
}

.center p {
  margin: 0;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
```

# Center Vertically - Using Flexbox

```css
You can also use flexbox to center things. Just note that flexbox is not supported in IE10 and earlier versions:

I am vertically and horizontally centered.

Example

.center {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 200px;
  border: 3px solid green;
}
```

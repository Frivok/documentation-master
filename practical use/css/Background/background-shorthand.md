# Table of Contents
- [Table of Contents](#table-of-contents)
- [CSS background - Shorthand property](#css-background---shorthand-property)
- [All CSS Background Properties](#all-css-background-properties)

# CSS background - Shorthand property

```bash
To shorten the code, it is also possible to specify all the background properties in one single property. This is called a shorthand property.

Instead of writing:

body {
  background-color: #ffffff;
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
}

You can use the shorthand property background:

Example

Use the shorthand property to set the background properties in one declaration:

body {
  background: #ffffff url("img_tree.png") no-repeat right top;
}

 When using the shorthand property the order of the property values is:

    background-color
    background-image
    background-repeat
    background-attachment
    background-position

It does not matter if one of the property values is missing, as long as the other ones are in this order. Note that we do not use the background-attachment property in the examples above, as it does not have a value.
```

# All CSS Background Properties

```bash
Property 	                  Description
background 	                  Sets all the background properties in one declaration
background-attachment 	      Sets whether a background image is fixed or scrolls with the rest of the page
background-clip 	          Specifies the painting area of the background
background-color 	          Sets the background color of an element
background-image 	          Sets the background image for an element
background-origin 	          Specifies where the background image(s) is/are positioned
background-position 	      Sets the starting position of a background image
background-repeat 	          Sets how a background image will be repeated
background-size 	          Specifies the size of the background image(s)
```

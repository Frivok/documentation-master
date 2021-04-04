# Table of Contents
- [Table of Contents](#table-of-contents)
- [Text Color](#text-color)
- [Text Color and Background Color](#text-color-and-background-color)

# Text Color

```bash
The color property is used to set the color of the text. The color is specified by:

    a color name - like "red"
    a HEX value - like "#ff0000"
    an RGB value - like "rgb(255,0,0)"

Look at CSS Color Values for a complete list of possible color values.

The default text color for a page is defined in the body selector.

Example

body {
  color: blue;
}

h1 {
  color: green;
}

Note: For W3C compliant CSS: If you define the color property, you must also define the background-color.
```

# Text Color and Background Color

```bash
In this example, we define both the background-color property and the color property:

Example

body {
  background-color: lightgrey;
  color: blue;
}

h1 {
  background-color: black;
  color: white;
} 
```
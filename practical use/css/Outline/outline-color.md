# Table of Contents
- [Table of Contents](#table-of-contents)
- [CSS Outline Color](#css-outline-color)
- [HEX Values](#hex-values)
- [RGB Values](#rgb-values)
- [HSL Values](#hsl-values)
- [Invert Color](#invert-color)

# CSS Outline Color

```bash
The outline-color property is used to set the color of the outline.

The color can be set by:

    name - specify a color name, like "red"
    HEX - specify a hex value, like "#ff0000"
    RGB - specify a RGB value, like "rgb(255,0,0)"
    HSL - specify a HSL value, like "hsl(0, 100%, 50%)"
    invert - performs a color inversion (which ensures that the outline is visible, regardless of color background)

Example

p.ex1 {
  border: 2px solid black;
  outline-style: solid;
  outline-color: red;
}

p.ex2 {
  border: 2px solid black;
  outline-style: dotted;
  outline-color: blue;
}

p.ex3 {
  border: 2px solid black;
  outline-style: outset;
  outline-color: grey;
}
```

# HEX Values

```bash
The outline color can also be specified using a hexadecimal value (HEX):

Example

p.ex1 {
  outline-style: solid;
  outline-color: #ff0000; /* red */
}
```

# RGB Values

```bash
Or by using RGB values:

Example

p.ex1 {
  outline-style: solid;
  outline-color: rgb(255, 0, 0); /* red */
}
```

# HSL Values

```bash
You can also use HSL values:

Example

p.ex1 {
  outline-style: solid;
  outline-color: hsl(0, 100%, 50%); /* red */
}
```

# Invert Color

```bash
The following example uses outline-color: invert, which performs a color inversion. This ensures that the outline is visible, regardless of color background:

A solid invert outline.

Example

p.ex1 {
  border: 1px solid yellow;
  outline-style: solid;
  outline-color: invert;
}
```
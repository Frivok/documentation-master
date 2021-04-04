# Table of Contents
- [Table of Contents](#table-of-contents)
- [CSS Border Color](#css-border-color)
- [Specific Side Colors](#specific-side-colors)
- [RGB Values](#rgb-values)
- [HSL Values](#hsl-values)

# CSS Border Color

```bash
The border-color property is used to set the color of the four borders.

The color can be set by:

    name - specify a color name, like "red"
    HEX - specify a HEX value, like "#ff0000"
    RGB - specify a RGB value, like "rgb(255,0,0)"
    HSL - specify a HSL value, like "hsl(0, 100%, 50%)"
    transparent

Note: If border-color is not set, it inherits the color of the element.

Example

Demonstration of the different border colors:

p.one {
  border-style: solid;
  border-color: red;
}

p.two {
  border-style: solid;
  border-color: green;
}

p.three {
  border-style: dotted;
  border-color: blue;
}
```

# Specific Side Colors

```bash
The border-color property can have from one to four values (for the top border, right border, bottom border, and the left border).

Example

p.one {
  border-style: solid;
  border-color: red green blue yellow; /* red top, green right, blue bottom and yellow left */
}

# HEX Values

```bash
The color of the border can also be specified using a hexadecimal value (HEX):

Example

p.one {
  border-style: solid;
  border-color: #ff0000; /* red */
}
```

# RGB Values

```bash
Or by using RGB values:

Example

p.one {
  border-style: solid;
  border-color: rgb(255, 0, 0); /* red */
}
```

# HSL Values

```bash
You can also use HSL values:

Example

p.one {
  border-style: solid;
  border-color: hsl(0, 100%, 50%); /* red */
}
```

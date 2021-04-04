# Table of Contents
- [Table of Contents](#table-of-contents)
- [CSS Border - Individual Sides](#css-border---individual-sides)

# CSS Border - Individual Sides

```bash
From the examples on the previous pages, you have seen that it is possible to specify a different border for each side.

In CSS, there are also properties for specifying each of the borders (top, right, bottom, and left):

Example

p {
  border-top-style: dotted;
  border-right-style: solid;
  border-bottom-style: dotted;
  border-left-style: solid;
}

The example above gives the same result as this:

Example

p {
  border-style: dotted solid;
}

So, here is how it works:

If the border-style property has four values:

    border-style: dotted solid double dashed;
        top border is dotted
        right border is solid
        bottom border is double
        left border is dashed

If the border-style property has three values:

    border-style: dotted solid double;
        top border is dotted
        right and left borders are solid
        bottom border is double

If the border-style property has two values:

    border-style: dotted solid;
        top and bottom borders are dotted
        right and left borders are solid

If the border-style property has one value:

    border-style: dotted;
        all four borders are dotted

Example

/* Four values */

p {
  border-style: dotted solid double dashed;
}

/* Three values */

p {
  border-style: dotted solid double;
}

/* Two values */

p {
  border-style: dotted solid;
}

/* One value */

p {
  border-style: dotted;
}

The border-style property is used in the example above. However, it also works with border-width and border-color.
```
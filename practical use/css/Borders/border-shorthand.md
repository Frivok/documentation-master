# Table of Contents
- [Table of Contents](#table-of-contents)
- [CSS Border - Shorthand Property](#css-border---shorthand-property)

# CSS Border - Shorthand Property

```bash
Like you saw in the previous page, there are many properties to consider when dealing with borders.

To shorten the code, it is also possible to specify all the individual border properties in one property.

The border property is a shorthand property for the following individual border properties:

    border-width
    border-style (required)
    border-color

Example

p {
  border: 5px solid red;
}

Result:

Some text

You can also specify all the individual border properties for just one side:

Left Border

p {
  border-left: 6px solid red;
  background-color: lightgrey;
}

Result:

Some text

Bottom Border

p {
  border-bottom: 6px solid red;
  background-color: lightgrey;
}

Result:

Some text
```
# Table of Contents
- [Table of Contents](#table-of-contents)
- [Text Alignment](#text-alignment)
- [Text Direction](#text-direction)
- [Vertical Alignment](#vertical-alignment)

# Text Alignment

```bash
The text-align property is used to set the horizontal alignment of a text.

A text can be left or right aligned, centered, or justified.

The following example shows center aligned, and left and right aligned text (left alignment is default if text direction is left-to-right, and right alignment is default if text direction is right-to-left):

Example

h1 {
  text-align: center;
}

h2 {
  text-align: left;
}

h3 {
  text-align: right;
}

When the text-align property is set to "justify", each line is stretched so that every line has equal width, and the left and right margins are straight (like in magazines and newspapers):

Example

div {
  text-align: justify;
}
```

# Text Direction

```bash
The direction and unicode-bidi properties can be used to change the text direction of

an element:

Example

p {
  direction: rtl;
  unicode-bidi: bidi-override;
}
```

# Vertical Alignment

```bash
The vertical-align property sets the vertical alignment of an element.

This example demonstrates how to set the vertical alignment of an image in a text:

Example

img.top {
  vertical-align: top;
}

img.middle {
  vertical-align: middle;
}

img.bottom {
  vertical-align: bottom;
}
```
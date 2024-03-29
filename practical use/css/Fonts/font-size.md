# Table of Contents
- [Table of Contents](#table-of-contents)
- [Font Size](#font-size)
- [Set Font Size With Pixels](#set-font-size-with-pixels)
- [Set Font Size With Em](#set-font-size-with-em)
- [Use a Combination of Percent and Em](#use-a-combination-of-percent-and-em)
- [Responsive Font Size](#responsive-font-size)

# Font Size

```bash
The font-size property sets the size of the text.

Being able to manage the text size is important in web design. However, you should not use font size adjustments to make paragraphs look like headings, or headings look like paragraphs.

Always use the proper HTML tags, like <h1> - <h6> for headings and <p> for paragraphs.

The font-size value can be an absolute, or relative size.

Absolute size:

    Sets the text to a specified size
    Does not allow a user to change the text size in all browsers (bad for accessibility reasons)
    Absolute size is useful when the physical size of the output is known

Relative size:

    Sets the size relative to surrounding elements
    Allows a user to change the text size in browsers

Note: If you do not specify a font size, the default size for normal text, like paragraphs, is 16px (16px=1em).
```

# Set Font Size With Pixels

```bash
Setting the text size with pixels gives you full control over the text size:

Example

h1 {
  font-size: 40px;
}

h2 {
  font-size: 30px;
}

p {
  font-size: 14px;
}

Tip: If you use pixels, you can still use the zoom tool to resize the entire page.
```

# Set Font Size With Em

```bash
To allow users to resize the text (in the browser menu), many developers use em instead of pixels.

The em size unit is recommended by the W3C.

1em is equal to the current font size. The default text size in browsers is 16px. So, the default size of 1em is 16px.

The size can be calculated from pixels to em using this formula: pixels/16=em

Example

h1 {
  font-size: 2.5em; /* 40px/16=2.5em */
}

h2 {
  font-size: 1.875em; /* 30px/16=1.875em */
}

p {
  font-size: 0.875em; /* 14px/16=0.875em */
}

In the example above, the text size in em is the same as the previous example in pixels. However, with the em size, it is possible to adjust the text size in all browsers.

Unfortunately, there is still a problem with older versions of Internet Explorer. The text becomes larger than it should when made larger, and smaller than it should when made smaller.
```

# Use a Combination of Percent and Em

```bash
The solution that works in all browsers, is to set a default font-size in percent for the <body> element:

Example

body {
  font-size: 100%;
}

h1 {
  font-size: 2.5em;
}

h2 {
  font-size: 1.875em;
}

p {
  font-size: 0.875em;
}

Our code now works great! It shows the same text size in all browsers, and allows all browsers to zoom or resize the text!
```

# Responsive Font Size

```bash
The text size can be set with a vw unit, which means the "viewport width".

That way the text size will follow the size of the browser window:
Hello World

Resize the browser window to see how the font size scales.

Example
<h1 style="font-size:10vw">Hello World</h1>

Viewport is the browser window size. 1vw = 1% of viewport width. If the viewport is 50cm wide, 1vw is 0.5cm.
```

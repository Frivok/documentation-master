# Table of Contents
- [Table of Contents](#table-of-contents)
- [CSS background-repeat](#css-background-repeat)
- [CSS background-repeat: no-repeat](#css-background-repeat-no-repeat)
- [CSS background-position](#css-background-position)

# CSS background-repeat

```bash
By default, the background-image property repeats an image both horizontally and vertically.

Some images should be repeated only horizontally or vertically, or they will look strange, like this:

Example

body {
  background-image: url("gradient_bg.png");
}

If the image above is repeated only horizontally (background-repeat: repeat-x;), the background will look better:

Example

body {
  background-image: url("gradient_bg.png");
  background-repeat: repeat-x;
}

Tip: To repeat an image vertically, set background-repeat: repeat-y;
```

# CSS background-repeat: no-repeat

```bash
Showing the background image only once is also specified by the background-repeat property:

Example

Show the background image only once:
body {
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
}

In the example above, the background image is placed in the same place as the text. We want to change the position of the image, so that it does not disturb the text too much.
```

# CSS background-position

```bash
The background-position property is used to specify the position of the background image.

Example

Position the background image in the top-right corner:

body {
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
}
```
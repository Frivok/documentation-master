# Table of Contents
- [Table of Contents](#table-of-contents)
- [CSS background-attachment](#css-background-attachment)

# CSS background-attachment

```bash
The background-attachment property specifies whether the background image should scroll or be fixed (will not scroll with the rest of the page):

Example

Specify that the background image should be fixed:

body {
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
  background-attachment: fixed;
}

Example

Specify that the background image should scroll with the rest of the page:

body {
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
  background-attachment: scroll;
}
```
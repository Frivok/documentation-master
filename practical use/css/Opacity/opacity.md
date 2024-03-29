# Table of Contents
- [Table of Contents](#table-of-contents)
- [Transparent Image](#transparent-image)
- [Transparent Hover Effect](#transparent-hover-effect)
- [Transparent Box](#transparent-box)
- [Transparency using RGBA](#transparency-using-rgba)
- [Text in Transparent Box](#text-in-transparent-box)

# Transparent Image

```css
The opacity property can take a value from 0.0 - 1.0. The lower value, the more transparent:

Example

img {
  opacity: 0.5;
}
```

# Transparent Hover Effect

```css
The opacity property is often used together with the :hover selector to change the opacity on mouse-over:

Example

img {
  opacity: 0.5;
}

img:hover {
  opacity: 1.0;
}

Example explained

The first CSS block is similar to the code in Example 1. In addition, we have added what should happen when a user hovers over one of the images. In this case we want the image to NOT be transparent when the user hovers over it. The CSS for this is opacity:1;.

When the mouse pointer moves away from the image, the image will be transparent again.

An example of reversed hover effect:

Example

img:hover {
  opacity: 0.5;
}
```

# Transparent Box

```css
When using the opacity property to add transparency to the background of an element, all of its child elements inherit the same transparency. This can make the text inside a fully transparent element hard to read:

opacity 1

opacity 0.6

opacity 0.3

opacity 0.1

Example

div {
  opacity: 0.3;
}
```

# Transparency using RGBA

```css
If you do not want to apply opacity to child elements, like in our example above, use RGBA color values. The following example sets the opacity for the background color and not the text:

100% opacity

60% opacity

30% opacity

10% opacity

You learned from our CSS Colors Chapter, that you can use RGB as a color value. In addition to RGB, you can use an RGB color value with an alpha channel (RGBA) - which specifies the opacity for a color.

An RGBA color value is specified with: rgba(red, green, blue, alpha). The alpha parameter is a number between 0.0 (fully transparent) and 1.0 (fully opaque).

Tip: You will learn more about RGBA Colors in our CSS Colors Chapter.

Example

div {
  background: rgba(76, 175, 80, 0.3) /* Green background with 30% opacity */
}
```

# Text in Transparent Box

```css
This is some text that is placed in the transparent box.

Example

<html>
<head>
<style>
div.background {
  background: url(klematis.jpg) repeat;
  border: 2px solid black;
}

div.transbox {
  margin: 30px;
  background-color: #ffffff;
  border: 1px solid black;
  opacity: 0.6;
}

div.transbox p {
  margin: 5%;
  font-weight: bold;
  color: #000000;
}
</style>
</head>
<body>

<div class="background">
  <div class="transbox">
    <p>This is some text that is placed in the transparent box.</p>
  </div>
</div>

</body>
</html>

Example explained

First, we create a <div> element (class="background") with a background image, and a border.

Then we create another <div> (class="transbox") inside the first <div>.

The <div class="transbox"> have a background color, and a border - the div is transparent.

Inside the transparent <div>, we add some text inside a <p> element.
```
# Table of Contents
- [Table of Contents](#table-of-contents)
- [CSS Layout - float and clear](#css-layout---float-and-clear)
- [The float Property](#the-float-property)
- [Example - float: right;](#example---float-right)
- [Example - float: left;](#example---float-left)
- [Example - No float](#example---no-float)

# CSS Layout - float and clear

```css
The CSS float property specifies how an element should float.

The CSS clear property specifies what elements can float beside the cleared element and on which side.
```

# The float Property

```css
The float property is used for positioning and formatting content e.g. let an image float left to the text in a container.

The float property can have one of the following values:

    left - The element floats to the left of its container
    right - The element floats to the right of its container
    none - The element does not float (will be displayed just where it occurs in the text). This is default
    inherit - The element inherits the float value of its parent

In its simplest use, the float property can be used to wrap text around images.
```

# Example - float: right;

```css
The following example specifies that an image should float to the right in a text:
PineappleLorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Mauris ante ligula, facilisis sed ornare eu, lobortis in odio. Praesent convallis urna a lacus interdum ut hendrerit risus congue. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac...

Example

img {
  float: right;
}
```

# Example - float: left;

```css
The following example specifies that an image should float to the left in a text:

PineappleLorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Mauris ante ligula, facilisis sed ornare eu, lobortis in odio. Praesent convallis urna a lacus interdum ut hendrerit risus congue. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac...

Example

img {
  float: left;
}
```

# Example - No float

```css
In the following example the image will be displayed just where it occurs in the text (float: none;):

Pineapple Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Mauris ante ligula, facilisis sed ornare eu, lobortis in odio. Praesent convallis urna a lacus interdum ut hendrerit risus congue. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac...
Example
img {
  float: none;
}
```
# Table of Contents
- [Table of Contents](#table-of-contents)
- [CSS Overflow](#css-overflow)
- [overflow: visible](#overflow-visible)
- [overflow: hidden](#overflow-hidden)
- [overflow: scroll](#overflow-scroll)
- [overflow: auto](#overflow-auto)
- [overflow-x and overflow-y](#overflow-x-and-overflow-y)
- [All CSS Overflow Properties](#all-css-overflow-properties)

# CSS Overflow

```css
The overflow property specifies whether to clip the content or to add scrollbars when the content of an element is too big to fit in the specified area.

The overflow property has the following values:

    visible - Default. The overflow is not clipped. The content renders outside the element's box
    hidden - The overflow is clipped, and the rest of the content will be invisible
    scroll - The overflow is clipped, and a scrollbar is added to see the rest of the content
    auto - Similar to scroll, but it adds scrollbars only when necessary

Note: The overflow property only works for block elements with a specified height.

Note: In OS X Lion (on Mac), scrollbars are hidden by default and only shown when being used (even though "overflow:scroll" is set).
```

# overflow: visible

```css
By default, the overflow is visible, meaning that it is not clipped and it renders outside the element's box:
You can use the overflow property when you want to have better control of the layout. The overflow property specifies what happens if content overflows an element's box.

Example

div {
  width: 200px;
  height: 50px;
  background-color: #eee;
  overflow: visible;
}
```

# overflow: hidden

```css
With the hidden value, the overflow is clipped, and the rest of the content is hidden:

You can use the overflow property when you want to have better control of the layout. The overflow property specifies what happens if content overflows an element's box.

Example

div {
  overflow: hidden;
}
```
# overflow: scroll

```css
Setting the value to scroll, the overflow is clipped and a scrollbar is added to scroll inside the box. Note that this will add a scrollbar both horizontally and vertically (even if you do not need it):
You can use the overflow property when you want to have better control of the layout. The overflow property specifies what happens if content overflows an element's box.

Example

div {
  overflow: scroll;
}
```

# overflow: auto

```css
The auto value is similar to scroll, but it adds scrollbars only when necessary:
You can use the overflow property when you want to have better control of the layout. The overflow property specifies what happens if content overflows an element's box.

Example

div {
  overflow: auto;
}
```

# overflow-x and overflow-y

```css
The overflow-x and overflow-y properties specifies whether to change the overflow of content just horizontally or vertically (or both):

overflow-x specifies what to do with the left/right edges of the content.
overflow-y specifies what to do with the top/bottom edges of the content.
You can use the overflow property when you want to have better control of the layout. The overflow property specifies what happens if content overflows an element's box.

Example

div {
  overflow-x: hidden; /* Hide horizontal scrollbar */
  overflow-y: scroll; /* Add vertical scrollbar */
}
```

# All CSS Overflow Properties

```css
Property 	Description

overflow 	Specifies what happens if content overflows an element's box
overflow-x 	Specifies what to do with the left/right edges of the content if it overflows the element's content area
overflow-y 	Specifies what to do with the top/bottom edges of the content if it overflows the element's content area
```
# Table of Contents
- [Table of Contents](#table-of-contents)
- [The position Property](#the-position-property)
- [position: static;](#position-static)
- [position: relative;](#position-relative)
- [position: fixed;](#position-fixed)
- [position: absolute;](#position-absolute)
- [position: sticky;](#position-sticky)
- [Overlapping Elements](#overlapping-elements)
- [All CSS Positioning Properties](#all-css-positioning-properties)

# The position Property

```css
The position property specifies the type of positioning method used for an element.

There are five different position values:

    static
    relative
    fixed
    absolute
    sticky

Elements are then positioned using the top, bottom, left, and right properties. However, these properties will not work unless the position property is set first. They also work differently depending on the position value.
```

# position: static;

```css
HTML elements are positioned static by default.

Static positioned elements are not affected by the top, bottom, left, and right properties.

An element with position: static; is not positioned in any special way; it is always positioned according to the normal flow of the page:

This <div> element has position: static;

Here is the CSS that is used:

Example

div.static {
  position: static;
  border: 3px solid #73AD21;
}
```

# position: relative;

```css
An element with position: relative; is positioned relative to its normal position.

Setting the top, right, bottom, and left properties of a relatively-positioned element will cause it to be adjusted away from its normal position. Other content will not be adjusted to fit into any gap left by the element.

This <div> element has position: relative;

Here is the CSS that is used:

Example

div.relative {
  position: relative;
  left: 30px;
  border: 3px solid #73AD21;
}
```

# position: fixed;

```css
An element with position: fixed; is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled. The top, right, bottom, and left properties are used to position the element.

A fixed element does not leave a gap in the page where it would normally have been located.

Notice the fixed element in the lower-right corner of the page. Here is the CSS that is used:

Example

div.fixed {
  position: fixed;
  bottom: 0;
  right: 0;
  width: 300px;
  border: 3px solid #73AD21;
}
```

# position: absolute;

```css
An element with position: absolute; is positioned relative to the nearest positioned ancestor (instead of positioned relative to the viewport, like fixed).

However; if an absolute positioned element has no positioned ancestors, it uses the document body, and moves along with page scrolling.

Note: A "positioned" element is one whose position is anything except static.

Here is a simple example:

This <div> element has position: relative;
This <div> element has position: absolute;

Here is the CSS that is used:

Example

div.relative {
  position: relative;
  width: 400px;
  height: 200px;
  border: 3px solid #73AD21;
}

div.absolute {
  position: absolute;
  top: 80px;
  right: 0;
  width: 200px;
  height: 100px;
  border: 3px solid #73AD21;
}
```

# position: sticky;

```css
An element with position: sticky; is positioned based on the user's scroll position.

A sticky element toggles between relative and fixed, depending on the scroll position. It is positioned relative until a given offset position is met in the viewport - then it "sticks" in place (like position:fixed).

Note: Internet Explorer does not support sticky positioning. Safari requires a -webkit- prefix (see example below). You must also specify at least one of top, right, bottom or left for sticky positioning to work.

In this example, the sticky element sticks to the top of the page (top: 0), when you reach its scroll position.

Example

div.sticky {
  position: -webkit-sticky; /* Safari */
  position: sticky;
  top: 0;
  background-color: green;
  border: 2px solid #4CAF50;
}
```

# Overlapping Elements

```css
When elements are positioned, they can overlap other elements.

The z-index property specifies the stack order of an element (which element should be placed in front of, or behind, the others).

An element can have a positive or negative stack order:

This is a heading

Because the image has a z-index of -1, it will be placed behind the text.

Example

img {
  position: absolute;
  left: 0px;
  top: 0px;
  z-index: -1;
}

An element with greater stack order is always in front of an element with a lower stack order.

Note: If two positioned elements overlap without a z-index specified, the element positioned last in the HTML code will be shown on top.
```

# All CSS Positioning Properties

```css
Property 	Description

bottom 	Sets the bottom margin edge for a positioned box
clip 	Clips an absolutely positioned element
left 	Sets the left margin edge for a positioned box
position 	Specifies the type of positioning for an element
right 	Sets the right margin edge for a positioned box
top 	Sets the top margin edge for a positioned box
z-index 	Sets the stack order of an element
```



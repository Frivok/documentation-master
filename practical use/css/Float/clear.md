# Table of Contents
- [Table of Contents](#table-of-contents)
- [The clear Property](#the-clear-property)
- [The clearfix Hack](#the-clearfix-hack)

# The clear Property

```css
The clear property specifies what elements can float beside the cleared element and on which side.

The clear property can have one of the following values:

    none - Allows floating elements on both sides. This is default
    left - No floating elements allowed on the left side
    right- No floating elements allowed on the right side
    both - No floating elements allowed on either the left or the right side
    inherit - The element inherits the clear value of its parent

The most common way to use the clear property is after you have used a float property on an element.

When clearing floats, you should match the clear to the float: If an element is floated to the left, then you should clear to the left. Your floated element will continue to float, but the cleared element will appear below it on the web page.

The following example clears the float to the left. Means that no floating elements are allowed on the left side (of the div):

Example

div {
  clear: left;
}
```

# The clearfix Hack

```css
If an element is taller than the element containing it, and it is floated, it will "overflow" outside of its container:

Without Clearfix
With Clearfix

Then we can add overflow: auto; to the containing element to fix this problem:

Example

.clearfix {
  overflow: auto;
}

The overflow: auto clearfix works well as long as you are able to keep control of your margins and padding (else you might see scrollbars). The new, modern clearfix hack however, is safer to use, and the following code is used for most webpages:

Example

.clearfix::after {
  content: "";
  clear: both;
  display: table;
}
```
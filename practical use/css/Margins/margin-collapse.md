# Table of Contents
- [Table of Contents](#table-of-contents)
- [Margin Collapse](#margin-collapse)
- [All CSS Margin Properties](#all-css-margin-properties)

# Margin Collapse

```bash
Top and bottom margins of elements are sometimes collapsed into a single margin that is equal to the largest of the two margins.

This does not happen on left and right margins! Only top and bottom margins!

Look at the following example:

Example

Demonstration of margin collapse:
h1 {
  margin: 0 0 50px 0;
}

h2 {
  margin: 20px 0 0 0;
}

In the example above, the <h1> element has a bottom margin of 50px and the <h2> element has a top margin set to 20px.

Common sense would seem to suggest that the vertical margin between the <h1> and the <h2> would be a total of 70px (50px + 20px). But due to margin collapse, the actual margin ends up being 50px.
```

# All CSS Margin Properties

```bash
Property 	Description

margin 	A shorthand property for setting the margin properties in one declaration
margin-bottom 	Sets the bottom margin of an element
margin-left 	Sets the left margin of an element
margin-right 	Sets the right margin of an element
margin-top 	Sets the top margin of an element
```
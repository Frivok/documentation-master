# Table of Contents
- [Table of Contents](#table-of-contents)
- [Responsive Table](#responsive-table)
- [CSS Table Properties](#css-table-properties)

# Responsive Table

```css
A responsive table will display a horizontal scroll bar if the screen is too small to display the full content:
First Name 	Last Name 	Points 	Points 	Points 	Points 	Points 	Points 	Points 	Points 	Points 	Points 	Points 	Points
Jill 	Smith 	50 	50 	50 	50 	50 	50 	50 	50 	50 	50 	50 	50
Eve 	Jackson 	94 	94 	94 	94 	94 	94 	94 	94 	94 	94 	94 	94
Adam 	Johnson 	67 	67 	67 	67 	67 	67 	67 	67 	67 	67 	67 	67

Add a container element (like <div>) with overflow-x:auto around the <table> element to make it responsive:

Example

<div style="overflow-x:auto;">

<table>
... table content ...
</table>

</div>

Note: In OS X Lion (on Mac), scrollbars are hidden by default and only shown when being used (even though "overflow:scroll" is set).
```

# CSS Table Properties

```css
Property 	Description

border 	Sets all the border properties in one declaration
border-collapse 	Specifies whether or not table borders should be collapsed
border-spacing 	Specifies the distance between the borders of adjacent cells
caption-side 	Specifies the placement of a table caption
empty-cells 	Specifies whether or not to display borders and background on empty cells in a table
table-layout 	Sets the layout algorithm to be used for a table
```
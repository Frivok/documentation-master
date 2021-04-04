# Table of Contents
- [Table of Contents](#table-of-contents)
- [Table Padding](#table-padding)
- [Horizontal Dividers](#horizontal-dividers)
- [Hoverable Table](#hoverable-table)
- [Striped Tables](#striped-tables)
- [Table Color](#table-color)

# Table Padding

```css
To control the space between the border and the content in a table, use the padding property on <td> and <th> elements:

Example

th, td {
  padding: 15px;
  text-align: left;
}
```

# Horizontal Dividers

```css
First Name 	Last Name 	Savings
Peter 	Griffin 	$100
Lois 	Griffin 	$150
Joe 	Swanson 	$300

Add the border-bottom property to <th> and <td> for horizontal dividers:

Example

th, td {
  border-bottom: 1px solid #ddd;
}
```

# Hoverable Table

```css
Use the :hover selector on <tr> to highlight table rows on mouse over:

First Name 	Last Name 	Savings
Peter 	Griffin 	$100
Lois 	Griffin 	$150
Joe 	Swanson 	$300

Example

tr:hover {background-color: #f5f5f5;}
```

# Striped Tables

```css
First Name 	Last Name 	Savings
Peter 	Griffin 	$100
Lois 	Griffin 	$150
Joe 	Swanson 	$300

For zebra-striped tables, use the nth-child() selector and add a background-color to all even (or odd) table rows:

Example

tr:nth-child(even) {background-color: #f2f2f2;}
```

# Table Color

```css
The example below specifies the background color and text color of <th> elements:

First Name 	Last Name 	Savings
Peter 	Griffin 	$100
Lois 	Griffin 	$150
Joe 	Swanson 	$300

Example

th {
  background-color: #4CAF50;
  color: white;
}
```
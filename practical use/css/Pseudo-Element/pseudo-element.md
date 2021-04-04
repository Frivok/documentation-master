# Table of Contents
- [Table of Contents](#table-of-contents)
- [What are Pseudo-Elements?](#what-are-pseudo-elements)
- [Syntax](#syntax)
- [The ::first-line Pseudo-element](#the-first-line-pseudo-element)
- [The ::first-letter Pseudo-element](#the-first-letter-pseudo-element)
- [Pseudo-elements and CSS Classes](#pseudo-elements-and-css-classes)
- [Multiple Pseudo-elements](#multiple-pseudo-elements)
- [CSS - The ::before Pseudo-element](#css---the-before-pseudo-element)
- [CSS - The ::after Pseudo-element](#css---the-after-pseudo-element)
- [CSS - The ::selection Pseudo-element](#css---the-selection-pseudo-element)
- [All CSS Pseudo Elements](#all-css-pseudo-elements)
- [All CSS Pseudo Classes](#all-css-pseudo-classes)

# What are Pseudo-Elements?

```css
A CSS pseudo-element is used to style specified parts of an element.

For example, it can be used to:

    Style the first letter, or line, of an element
    Insert content before, or after, the content of an element
```

# Syntax

```css
The syntax of pseudo-elements:
selector::pseudo-element {
  property: value;
}
```

# The ::first-line Pseudo-element

```css
The ::first-line pseudo-element is used to add a special style to the first line of a text.

The following example formats the first line of the text in all <p> elements:

Example 

p::first-line {
  color: #ff0000;
  font-variant: small-caps;
}

Note: The ::first-line pseudo-element can only be applied to block-level elements.

The following properties apply to the ::first-line pseudo-element:

    font properties
    color properties
    background properties
    word-spacing
    letter-spacing
    text-decoration
    vertical-align
    text-transform
    line-height
    clear

Notice the double colon notation - ::first-line versus :first-line

The double colon replaced the single-colon notation for pseudo-elements in CSS3. This was an attempt from W3C to distinguish between pseudo-classes and pseudo-elements.

The single-colon syntax was used for both pseudo-classes and pseudo-elements in CSS2 and CSS1.

For backward compatibility, the single-colon syntax is acceptable for CSS2 and CSS1 pseudo-elements.
```

# The ::first-letter Pseudo-element

```css
The ::first-letter pseudo-element is used to add a special style to the first letter of a text.

The following example formats the first letter of the text in all <p> elements: 

Example

p::first-letter {
  color: #ff0000;
  font-size: xx-large;
}

Note: The ::first-letter pseudo-element can only be applied to block-level elements.

The following properties apply to the ::first-letter pseudo- element: 

    font properties
    color properties 
    background properties
    margin properties
    padding properties
    border properties
    text-decoration
    vertical-align (only if "float" is "none")
    text-transform
    line-height
    float
    clear
```

# Pseudo-elements and CSS Classes

```css
Pseudo-elements can be combined with CSS classes: 

Example

p.intro::first-letter {
  color: #ff0000;
  font-size: 200%;
}

The example above will display the first letter of paragraphs with class="intro", in red and in a larger size.
```

# Multiple Pseudo-elements

```css
Several pseudo-elements can also be combined.

In the following example, the first letter of a paragraph will be red, in an xx-large font size. The rest of the first line will be blue, and in small-caps. The rest of the paragraph will be the default font size and color:

Example

p::first-letter {
  color: #ff0000;
  font-size: xx-large;
}

p::first-line {
  color: #0000ff;
  font-variant: small-caps;
}
```

# CSS - The ::before Pseudo-element

```css
The ::before pseudo-element can be used to insert some content before the content of an element.

The following example inserts an image before the content of each <h1> element:

Example

h1::before {
  content: url(smiley.gif);
}
```

# CSS - The ::after Pseudo-element

```css
The ::after pseudo-element can be used to insert some content after the content of an element.

The following example inserts an image after the content of each <h1> element:

Example

h1::after {
  content: url(smiley.gif);
}
```

# CSS - The ::selection Pseudo-element

```css
The ::selection pseudo-element matches the portion of an element that is selected by a user.

The following CSS properties can be applied to ::selection: color, background, cursor, and outline.

The following example makes the selected text red on a yellow background:

Example

::selection {
  color: red;
  background: yellow;
}
```

# All CSS Pseudo Elements

```css
Selector 	Example 	Example description

::after 	p::after 	Insert something after the content of each <p> element
::before 	p::before 	Insert something before the content of each <p> element
::first-letter 	p::first-letter 	Selects the first letter of each <p> element
::first-line 	p::first-line 	Selects the first line of each <p> element
::selection 	p::selection 	Selects the portion of an element that is selected by a user
```

# All CSS Pseudo Classes

```css
Selector 	Example 	Example description

:active 	a:active 	Selects the active link
:checked 	input:checked 	Selects every checked <input> element
:disabled 	input:disabled 	Selects every disabled <input> element
:empty 	p:empty 	Selects every <p> element that has no children
:enabled 	input:enabled 	Selects every enabled <input> element
:first-child 	p:first-child 	Selects every <p> elements that is the first child of its parent
:first-of-type 	p:first-of-type 	Selects every <p> element that is the first <p> element of its parent
:focus 	input:focus 	Selects the <input> element that has focus
:hover 	a:hover 	Selects links on mouse over
:in-range 	input:in-range 	Selects <input> elements with a value within a specified range
:invalid 	input:invalid 	Selects all <input> elements with an invalid value
:lang(language) 	p:lang(it) 	Selects every <p> element with a lang attribute value starting with "it"
:last-child 	p:last-child 	Selects every <p> elements that is the last child of its parent
:last-of-type 	p:last-of-type 	Selects every <p> element that is the last <p> element of its parent
:link 	a:link 	Selects all unvisited links
:not(selector) 	:not(p) 	Selects every element that is not a <p> element
:nth-child(n) 	p:nth-child(2) 	Selects every <p> element that is the second child of its parent
:nth-last-child(n) 	p:nth-last-child(2) 	Selects every <p> element that is the second child of its parent, counting from the last child
:nth-last-of-type(n) 	p:nth-last-of-type(2) 	Selects every <p> element that is the second <p> element of its parent, counting from the last child
:nth-of-type(n) 	p:nth-of-type(2) 	Selects every <p> element that is the second <p> element of its parent
:only-of-type 	p:only-of-type 	Selects every <p> element that is the only <p> element of its parent
:only-child 	p:only-child 	Selects every <p> element that is the only child of its parent
:optional 	input:optional 	Selects <input> elements with no "required" attribute
:out-of-range 	input:out-of-range 	Selects <input> elements with a value outside a specified range
:read-only 	input:read-only 	Selects <input> elements with a "readonly" attribute specified
:read-write 	input:read-write 	Selects <input> elements with no "readonly" attribute
:required 	input:required 	Selects <input> elements with a "required" attribute specified
:root 	root 	Selects the document's root element
:target 	#news:target 	Selects the current active #news element (clicked on a URL containing that anchor name)
:valid 	input:valid 	Selects all <input> elements with a valid value
:visited 	a:visited 	Selects all visited links
```
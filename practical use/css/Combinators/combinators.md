# Table of Contents
- [Table of Contents](#table-of-contents)
- [CSS Combinators](#css-combinators)
- [Descendant Selector](#descendant-selector)
- [Child Selector](#child-selector)
- [Adjacent Sibling Selector](#adjacent-sibling-selector)
- [General Sibling Selector](#general-sibling-selector)
- [All CSS Combinator Selectors](#all-css-combinator-selectors)

# CSS Combinators

```css
A combinator is something that explains the relationship between the selectors.

A CSS selector can contain more than one simple selector. Between the simple selectors, we can include a combinator.

There are four different combinators in CSS:

    descendant selector (space)
    child selector (>)
    adjacent sibling selector (+)
    general sibling selector (~)
```

# Descendant Selector

```css
The descendant selector matches all elements that are descendants of a specified element.

The following example selects all <p> elements inside <div> elements:

Example

div p {
  background-color: yellow;
}
```

# Child Selector

```css
The child selector selects all elements that are the children of a specified element.

The following example selects all <p> elements that are children of a <div> element:

Example

div > p {
  background-color: yellow;
}
```

# Adjacent Sibling Selector

```css
The adjacent sibling selector selects all elements that are the adjacent siblings of a specified element.

Sibling elements must have the same parent element, and "adjacent" means "immediately following".

The following example selects all <p> elements that are placed immediately after <div> elements:

Example

div + p {
  background-color: yellow;
}
```

# General Sibling Selector

```css
The general sibling selector selects all elements that are siblings of a specified element.

The following example selects all <p> elements that are siblings of <div> elements:

Example

div ~ p {
  background-color: yellow;
}
```

# All CSS Combinator Selectors

```css
Selector 	Example 	Example description

element element 	div p 	Selects all <p> elements inside <div> elements
element>element 	div > p 	Selects all <p> elements where the parent is a <div> element
element+element 	div + p 	Selects all <p> elements that are placed immediately after <div> elements
element1~element2 	p ~ ul 	Selects every <ul> element that are preceded by a <p> element
```

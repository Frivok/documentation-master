# Table of Contents
- [Table of Contents](#table-of-contents)
- [CSS [attribute] Selector](#css-attribute-selector)
- [CSS [attribute="value"] Selector](#css-attributevalue-selector)
- [CSS [attribute~="value"] Selector](#css-attributevalue-selector-1)
- [CSS [attribute|="value"] Selector](#css-attributevalue-selector-2)
- [CSS [attribute^="value"] Selector](#css-attributevalue-selector-3)
- [CSS [attribute$="value"] Selector](#css-attributevalue-selector-4)
- [CSS [attribute*="value"] Selector](#css-attributevalue-selector-5)
- [Styling Forms](#styling-forms)
- [All CSS Attribute Selectors](#all-css-attribute-selectors)

# CSS [attribute] Selector

```css
The [attribute] selector is used to select elements with a specified attribute.

The following example selects all <a> elements with a target attribute:

Example

a[target] {
  background-color: yellow;
}
```

# CSS [attribute="value"] Selector

```css
The [attribute="value"] selector is used to select elements with a specified attribute and value.

The following example selects all <a> elements with a target="_blank" attribute:

Example

a[target="_blank"] {
  background-color: yellow;
}
```

# CSS [attribute~="value"] Selector

```css
The [attribute~="value"] selector is used to select elements with an attribute value containing a specified word.

The following example selects all elements with a title attribute that contains a space-separated list of words, one of which is "flower":

Example

[title~="flower"] {
  border: 5px solid yellow;
}

The example above will match elements with title="flower", title="summer flower", and title="flower new", but not title="my-flower" or title="flowers".
```

# CSS [attribute|="value"] Selector

```css
The [attribute|="value"] selector is used to select elements with the specified attribute starting with the specified value.

The following example selects all elements with a class attribute value that begins with "top":

Note: The value has to be a whole word, either alone, like class="top", or followed by a hyphen( - ), like class="top-text"!

Example

[class|="top"] {
  background: yellow;
}
```

# CSS [attribute^="value"] Selector

```css
The [attribute^="value"] selector is used to select elements whose attribute value begins with a specified value.

The following example selects all elements with a class attribute value that begins with "top":

Note: The value does not have to be a whole word! 

Example

[class^="top"] {
  background: yellow;
}
```

# CSS [attribute$="value"] Selector

```css
The [attribute$="value"] selector is used to select elements whose attribute value ends with a specified value.

The following example selects all elements with a class attribute value that ends with "test":

Note: The value does not have to be a whole word!  

Example

[class$="test"] {
  background: yellow;
}
```

# CSS [attribute*="value"] Selector

```css
The [attribute*="value"] selector is used to select elements whose attribute value contains a specified value.

The following example selects all elements with a class attribute value that contains "te":

Note: The value does not have to be a whole word!  

Example

[class*="te"] {
  background: yellow;
}
```

# Styling Forms

```css
The attribute selectors can be useful for styling forms without class or ID:

Example

input[type="text"] {
  width: 150px;
  display: block;
  margin-bottom: 10px;
  background-color: yellow;
}

input[type="button"] {
  width: 120px;
  margin-left: 35px;
  display: block;
}
```

# All CSS Attribute Selectors

```css
Selector 	Example 	Example description

[attribute] 	[target] 	Selects all elements with a target attribute
[attribute=value] 	[target=_blank] 	Selects all elements with target="_blank"
[attribute~=value] 	[title~=flower] 	Selects all elements with a title attribute containing the word "flower"
[attribute|=value] 	[lang|=en] 	Selects all elements with a lang attribute value starting with "en"
[attribute^=value] 	a[href^="https"] 	Selects every <a> element whose href attribute value begins with "https"
[attribute$=value] 	a[href$=".pdf"] 	Selects every <a> element whose href attribute value ends with ".pdf"
[attribute*=value] 	a[href*="w3schools"] 	Selects every <a> element whose href attribute value contains the substring "w3schools"
```
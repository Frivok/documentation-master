# Table of Contents
- [Table of Contents](#table-of-contents)
- [CSS Font Families](#css-font-families)
- [Font Family](#font-family)

# CSS Font Families

```bash
In CSS, there are two types of font family names:

    generic family - a group of font families with a similar look (like "Serif" or "Monospace")
    font family - a specific font family (like "Times New Roman" or "Arial")

Generic family 	Font family 	Description
Serif 	Times New Roman
Georgia 	Serif fonts have small lines at the ends on some characters
Sans-serif 	Arial
Verdana 	"Sans" means without - these fonts do not have the lines at the ends of characters
Monospace 	Courier New
Lucida Console 	All monospace characters have the same width

Note: On computer screens, sans-serif fonts are considered easier to read than serif fonts.
```

# Font Family

```bash
The font family of a text is set with the font-family property.

The font-family property should hold several font names as a "fallback" system. If the browser does not support the first font, it tries the next font, and so on.

Start with the font you want, and end with a generic family, to let the browser pick a similar font in the generic family, if no other fonts are available.

Note: If the name of a font family is more than one word, it must be in quotation marks, like: "Times New Roman".

More than one font family is specified in a comma-separated list:

Example

Specify the font for three paragraphs:

.serif {
  font-family: "Times New Roman", Times, serif;
}

.sansserif {
  font-family: Arial, Helvetica, sans-serif;
}

.monospace {
  font-family: "Lucida Console", Courier, monospace;
}
Example

Specify the "Impact" font for a paragraph:

p.impact {
  font-family: Impact, Charcoal, sans-serif;
}
```

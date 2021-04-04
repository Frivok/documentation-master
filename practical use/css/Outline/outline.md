# Table of Contents
- [Table of Contents](#table-of-contents)
- [CSS Outline](#css-outline)
- [CSS Outline Style](#css-outline-style)

# CSS Outline

```bash
An outline is a line that is drawn around elements, OUTSIDE the borders, to make the element "stand out".

CSS has the following outline properties:

    outline-style
    outline-color
    outline-width
    outline-offset
    outline

Note: Outline differs from borders! Unlike border, the outline is drawn outside the element's border, and may overlap other content. Also, the outline is NOT a part of the element's dimensions; the element's total width and height is not affected by the width of the outline.
```

# CSS Outline Style

```bash
The outline-style property specifies the style of the outline, and can have one of the following values:

    dotted - Defines a dotted outline
    dashed - Defines a dashed outline
    solid - Defines a solid outline
    double - Defines a double outline
    groove - Defines a 3D grooved outline
    ridge - Defines a 3D ridged outline
    inset - Defines a 3D inset outline
    outset - Defines a 3D outset outline
    none - Defines no outline
    hidden - Defines a hidden outline

The following example shows the different outline-style values:

Example

Demonstration of the different outline styles:

p.dotted {outline-style: dotted;}
p.dashed {outline-style: dashed;}
p.solid {outline-style: solid;}
p.double {outline-style: double;}
p.groove {outline-style: groove;}
p.ridge {outline-style: ridge;}
p.inset {outline-style: inset;}
p.outset {outline-style: outset;}
```
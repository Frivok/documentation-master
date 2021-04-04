# Css

- [Css](#css)
  - [Commands](#commands)
    - [.classname (used to select a class)](#classname-used-to-select-a-class)
    - [background (used to set all background style like color image size)](#background-used-to-set-all-background-style-like-color-image-size)
    - [background-attachement (used to set whetever a background image position is fixed or scrolls)](#background-attachement-used-to-set-whetever-a-background-image-position-is-fixed-or-scrolls)
    - [background-image (used to set one or more background images on an element)](#background-image-used-to-set-one-or-more-background-images-on-an-element)
    - [color(used to setup a color value of a text)](#colorused-to-setup-a-color-value-of-a-text)
    - [font(used to set all different properties of an element's font)](#fontused-to-set-all-different-properties-of-an-elements-font)
    - [text-align (align the text to the left right or center of the screen)](#text-align-align-the-text-to-the-left-right-or-center-of-the-screen)
    - [align a picture (align a picture to thecenter of the screen)](#align-a-picture-align-a-picture-to-thecenter-of-the-screen)
    - [text-decoration (used to specify the color of the text-decoration underline,overline)](#text-decoration-used-to-specify-the-color-of-the-text-decoration-underlineoverline)
    - [float (used to place a picture on the right or left side of a text )](#float-used-to-place-a-picture-on-the-right-or-left-side-of-a-text-)
    - [padding (used to generate space around a text or picture )](#padding-used-to-generate-space-around-a-text-or-picture-)
    - [position (used to position an element in a document(use absolute to move a picture))](#position-used-to-position-an-element-in-a-documentuse-absolute-to-move-a-picture)
    - [max-width (used to describe how much space can a line or picture take (really useful for mobile website))](#max-width-used-to-describe-how-much-space-can-a-line-or-picture-take-really-useful-for-mobile-website)
    - [@media (used to put anything inside a rule(really useful for mobile))](#media-used-to-put-anything-inside-a-rulereally-useful-for-mobile)
    - [hover (used to style a link when you mouse over it))](#hover-used-to-style-a-link-when-you-mouse-over-it)

## Commands

[Css](http://www.css-faciles.com/proprietes-css-liste-alphabetique.php)

### .classname (used to select a class)

```bash
.class{
color:red;
}
```

### background (used to set all background style like color image size)

```bash
background:
```

### background-attachement (used to set whetever a background image position is fixed or scrolls)

```bash
background-attachment: scroll;
background-attachment: fixed;
background-attachment: local;
```

### background-image (used to set one or more background images on an element)

```bash
background-image url("filepath/image.png")
                 url("filepath/secondimage.png")
```

### color(used to setup a color value of a text)

```bash
color: rebeccapurple;
color: rgb(214,122,127);
color: #00f00;
```

### font(used to set all different properties of an element's font)

```bash
font: 1.2em "Fira Sans", sans-serif;
font: italic 1.2em "Fira Sans", serif;
font-size: 18px;
```

### text-align (align the text to the left right or center of the screen)

```bash
text-align: left;
text-align: right;
text-align: center;
```

### align a picture (align a picture to thecenter of the screen)

```bash
display: block;
margin: 0 auto;
```

### text-decoration (used to specify the color of the text-decoration underline,overline)

```bash
text-decoration: underline;
text-decoration-color: red;
```

### float (used to place a picture on the right or left side of a text )

```bash
float: none;
float: left;
float: right;
```

### padding (used to generate space around a text or picture )

```bash
padding-top: 50px;
padding-right: 30px;
padding-bottom: 50px;
padding-left: 80px;
```

### position (used to position an element in a document(use absolute to move a picture))

```bash
position: static;
position: relative;
position: absolute;
```

### max-width (used to describe how much space can a line or picture take (really useful for mobile website))

```bash
max-width: 50%;
```

### @media (used to put anything inside a rule(really useful for mobile))

```bash
@media (max-width: 600px) {
  .sidebar {
    display: none;
  }
}
```

### hover (used to style a link when you mouse over it))

```bash
a:hover{
  background-color;green;
}
p:hover{
  background-color: green;
}
etc
```

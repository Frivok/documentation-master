# Html

- [Html](#html)
  - [Commands](#commands)
    - [link (link to other pages of your project)](#link-link-to-other-pages-of-your-project)
    - [Href (adress of a link)](#href-adress-of-a-link)
    - [Href Target (open the link in a new window)](#href-target-open-the-link-in-a-new-window)
    - [Br (break line, go to the next line)](#br-break-line-go-to-the-next-line)
    - [Div (create a section in a document (really useful if you assign a class to it))](#div-create-a-section-in-a-document-really-useful-if-you-assign-a-class-to-it)
    - [Source (used to specify resources like videos audio or picture)](#source-used-to-specify-resources-like-videos-audio-or-picture)
    - [Span (create an element to color a part of a text)](#span-create-an-element-to-color-a-part-of-a-text)
    - [Strong (Define important text)](#strong-define-important-text)
    - [Class (create a class that can be modified using javascript or css)](#class-create-a-class-that-can-be-modified-using-javascript-or-css)
    - [Button (create a clickable button)](#button-create-a-clickable-button)
    - [Small (define smaller text)](#small-define-smaller-text)
    - [Link (used to link to a document or an external ressource)](#link-used-to-link-to-a-document-or-an-external-ressource)
    - [Ol (used to to represent a list used with li)](#ol-used-to-to-represent-a-list-used-with-li)
    - [Li (the list represented by Ol)](#li-the-list-represented-by-ol)
    - [Img (create a picture)](#img-create-a-picture)
    - [H1-H6 (define the size of the writting)](#h1-h6-define-the-size-of-the-writting)
    - [Form (is used to describe a section of a document where the user send stuff to the server)](#form-is-used-to-describe-a-section-of-a-document-where-the-user-send-stuff-to-the-server)
    - [Label (is used to give a name or description to a button or an object)](#label-is-used-to-give-a-name-or-description-to-a-button-or-an-object)
    - [Input (is used to create a place to give the user a way to input stuff (will change a lot depanding on the type attribute))](#input-is-used-to-create-a-place-to-give-the-user-a-way-to-input-stuff-will-change-a-lot-depanding-on-the-type-attribute)
    - [Common HTML events ()](#common-html-events-)
    - [TextArea (make a huge text area)](#textarea-make-a-huge-text-area)

## Commands

[Html](http://www.transaction.net/web/tutor/cmdtable.html)

### link (link to other pages of your project)

```bash
<link rel="stylesheet" href="style.css" />
```

### Href (adress of a link)

```bash
<a href="https://www.google.com">google</a>
```

### Href Target (open the link in a new window)

```bash
<a href="https://www.google.com" target="_blank">google</a>
```

### Br (break line, go to the next line)

```bash
<br />
```

### Div (create a section in a document (really useful if you assign a class to it))

```bash
<div></div>
```

### Source (used to specify resources like videos audio or picture)

```bash
<audio controls>
  <source src="horseshooe.mp3" type="audio/mp3">
  Your browser does not support the audio element
  </audio>
```

### Span (create an element to color a part of a text)

```bash
<p> My mother has <span style="color:blue">blue</span> eyes.</p>
```

### Strong (Define important text)

```bash
<strong>This text is important!!</strong >
```

### Class (create a class that can be modified using javascript or css)

```bash
<strong class="important">This text is important!!</strong >
```

### Button (create a clickable button)

```bash
<button type="button">Click Me!</button>
```

### Small (define smaller text)

```bash
<small>This is a small text</small>
```

### Link (used to link to a document or an external ressource)

```bash
<link href="style.css" rel="stylesheet">
```

### Ol (used to to represent a list used with li)

```bash
<ol>
<li>First element</li>
<li>Second element</li>
<li>Third element</li>
</ol>
```

### Li (the list represented by Ol)

```bash
<ol>
<li>First element</li>
<li>Second element</li>
<li>Third element</li>
</ol>
```

### Img (create a picture)

```bash
<img src="link of the source" alt="name in case the picture doesn't show up" width="width of the picture" height ="height of the picture">
```

### H1-H6 (define the size of the writting)

```bash
<h1> <h2> <h3> <h4> <h5> <h6>
```

### Form (is used to describe a section of a document where the user send stuff to the server)

```bash
<form method="post" action="mailto:behague45@gmail.com">
```

### Label (is used to give a name or description to a button or an object)

```bash
<label for="Firstname">First Name</label>
<input type="text" name="Firstname" placeholder="Enter your first name.." />
```

### Input (is used to create a place to give the user a way to input stuff (will change a lot depanding on the type attribute))

```bash
<label for="name">Name (4 to 8 characters):</label>
<input type="text" id="name" name="name" required
minlength="4" maxlength="8" size="10">

All the different kind of input
<button> an empty button
<checkbox> a case to tick that select or remove a value
<color> used to define colors
<date> used to set a date (days months years)
<datetime-local> used to set a date manually
<email id="email"> used to put an email
<file> used to select a file
<image id="image" src="picture path"> used to create graphic buttons so the send button will look like an image instead of a text
<month min="2020-08" value="2020-10"> used to input date (month and year)
<number min="10" max="100"> a control that allows you to input a number
<password minlength="8"> allow a user to put a password
<range> used to make an audio slider
<reset> used to make a reset button
<search> used to make a user search something on the site
<submit> used to submit what the user wrote
<tel> used to input a phone number
<text> used to put text on a single line
<time min="9:00" max="18:00"> used to input a time (minutes hours)
<url> used to make an user enter an url
```

### Common HTML events ()

```bash
Event             Description
onchange          An HTML element has been changed
onclick           The user clicks an HTML element
onmouseover       The user moves the mouse over an HTML element
onmouseout        The user moves the mouse away from an HTML element
onkeydown         The user pushes a keyboard key
onload            The browser has finished loading the page
```


### TextArea (make a huge text area)

```bash
<textarea id="story" name="story" rows="5" cols="33">
```

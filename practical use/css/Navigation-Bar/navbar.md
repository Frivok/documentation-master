# Table of Contents
- [Table of Contents](#table-of-contents)
- [Navigation Bars](#navigation-bars)
- [Navigation Bar = List of Links](#navigation-bar--list-of-links)

# Navigation Bars

```css
Having easy-to-use navigation is important for any web site.

With CSS you can transform boring HTML menus into good-looking navigation bars.
```

# Navigation Bar = List of Links

```css
A navigation bar needs standard HTML as a base.

In our examples we will build the navigation bar from a standard HTML list.

A navigation bar is basically a list of links, so using the <ul> and <li> elements makes perfect sense:

Example

<ul>
  <li><a href="default.asp">Home</a></li>
  <li><a href="news.asp">News</a></li>
  <li><a href="contact.asp">Contact</a></li>
  <li><a href="about.asp">About</a></li>
</ul>

Now let's remove the bullets and the margins and padding from the list:

Example

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

Example explained:

    list-style-type: none; - Removes the bullets. A navigation bar does not need list markers
    Set margin: 0; and padding: 0; to remove browser default settings

The code in the example above is the standard code used in both vertical, and horizontal navigation bars, which you will learn more about in the next chapters.
```
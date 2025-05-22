---
Date: 2025-05-01 00:00
Type: Page
Template: Page Template
Title: Intersect
Location: /intersect
---

# Intersect

**Table of content**

{toc}

---

## CSS

In CSS files:

- `#08F` and `#0088FF` are the same.

The difference between `#08F` and `#0088FF` is that #08f is a shorthand representation of the color #0088ff. The shorthand format uses a single digit for each color component (red, green, blue), and the full six-digit format expands each single digit to two digits, repeating the digit

`#08F` expands to `#0088FF` by duplicating the digits: `0` becomes `00`, `8` becomes `88`, and `F` becomes `FF`. This expands the shorthand notation to the standard six-digit hexadecimal color code.

---

## The CSS `element` Selector

The element selector selects HTML elements based on the element name.

Here, all HTML `<p>` elements on the page will be center-aligned.

In CSS:

```css
p {
  text-align: center;
}
```
In HTML: 

```html
<p>Every paragraph will be affected by the style.</p>
<p id="paragraph">Me too!</p>
<p>And me!</p>
```

---

## CSS `.class` Selector

Select and style all elements with `class="intro"`:

```css
.intro {
  background-color: yellow;
}
```

In HTML:

```html
<h1>Demo of the .class selector</h1>

<div class="intro">
  <p>My name is Donald.</p>
  <p>I live in Duckburg.</p>
</div>

<p>My best friend is Mickey.</p>

<p class="intro">My best friend is Mickey.</p>
```

---

## The CSS `id` Selector

The id selector uses the id attribute of an HTML element to select a specific element.

The id of an element is unique within a page, so the id selector is used to select one unique element!

To select an element with a specific id, write a hash `#` character, followed by the id of the element.

In CSS:

```css
#paragraph1 {
  text-align: center;
}
```

In HTML:

```html
<p id="paragraph1">Hello World!</p>
<p>This paragraph is not affected by the style.</p>
```

---

## The CSS class Selector

**Note: A class name cannot start with a number!**

The class selector selects HTML elements with a specific class attribute.

To select elements with a specific class, write a period `.` character, followed by the class name.

In CSS:

```css
.center {
  text-align: center;
}
```

In HTML:

```html
<h1 class="center">Center-aligned heading</h1>
<p class="center">Center-aligned paragraph.</p>
```

---

## The CSS Universal Selector

The universal selector `*` selects all HTML elements on the page.

In CSS:

```css
* {
  text-align: center;
}
```

In HTML:

```html
<h1>Hello world!</h1>

<p>Every element on the page will be affected by the style.</p>
<p id="paragraph">Me too!</p>
<p>And me!</p>
```

---

## The CSS Grouping Selector

The grouping selector selects all the HTML elements with the same style definitions.

Look at the following CSS code (the `h1`, `h2`, and `p` elements have the same style definitions):

```css
h1 {
  text-align: center;
}

h2 {
  text-align: center;
}

p {
  text-align: center;
}
```

It will be better to group the selectors, to minimize the code.

To group selectors, separate each selector with a comma.


In CSS:

```css
h1, h2, p {
  text-align: center;
}
```

In HTML:

```html
<h1>Hello World!</h1>
<h2>Smaller heading!</h2>
<p>This is a paragraph.</p>
```

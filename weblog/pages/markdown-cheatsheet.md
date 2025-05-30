---
Date: 2025-05-25 00:00
Type: Page
Title: Markdown Cheatsheet
Location: /markdown-cheatsheet
Tags: Slashes, Markdown, Cheatsheet, Markdown Cheatsheet
Index: Exclude
---

# Markdown Cheatsheet

---

**Table of Contents**

{toc}

---

# Headers

```
# Header 1
## Header 2
### Header 3
#### Header 4
##### Header 5
###### Header 6
```

# Header 1
## Header 2
### Header 3
#### Header 4
##### Header 5
###### Header 6

---

# Emphasis

```
*italic*, **bold**, `inline code`, ~~strikethrough~~
```


*italic*, **bold**, `inline code`, ~~strikethrough~~

---

# Blockquote

```
> This is a blockquote
```

> This is a blockquote

---

# Lists and Tasks

---

## Unordered List

```
- Item 1
- Item 2
    - Item 3a
    - Item 3b
```

- Item 1
- Item 2
    - Item 3a
    - Item 3b

---

## Ordered List

```
1. Item 1
2. Item 2
     3. Item 3
     4. Item 4
```

1. Item 1
2. Item 2
     3. Item 3a
     4. Item 4

---

## Tasks

```
- [ ] Checkbox off
- [x] Checkbox on
```

- [ ] Checkbox off
- [x] Checkbox on

---

# Links

```
[link](https://luxury-format.weblog.lol)

<https://luxury-format.weblog.lol>
```

[link](https://luxury-format.weblog.lol)

<https://luxury-format.weblog.lol>

---

# Horizontal line

```
---
```

---

---

# Code

---

## Code Blocks

````markdown
```javascript
console.log("This is a block code");
```
````

```javascript
console.log("This is a block code");
```

---

```
    4 space indent makes a code block
```

    4 space indent makes a code block

---

## Escaped code

Escaped code blocks can be done with more back ticks on the outside or a different symbol.

`````markdown
````markdown
```bash
echo hi
```
````
`````

````markdown
```bash
echo hi
```
````

---

## Inline code

```
`Inline code` has back-ticks around it.
```

`Inline code` has back-ticks around it.

---

# Tables

```
| Left Column | Center Column | Right Column |
| :--- | :---: | ---: |
| Row 1 | Centered | $1600 |
| Row 2 | Cell | $12 |
```

| Left Column | Center Column | Right Column |
| :--- | :---: | ---: |
| Row 1 | Centered | $1600 |
| Row 2 | Cell | $12 |

---

# Images

```
![LUXURY FORMAT Logo](https://profiles.cache.lol/luxury-format/picture.png)
```

![LUXURY FORMAT Logo](https://profiles.cache.lol/luxury-format/picture.png)

---

## Image with link

```
[![LUXURY FORMAT Logo](https://profiles.cache.lol/luxury-format/picture.png)](https://luxury-format.weblog.lol)
```

[![LUXURY FORMAT Logo](https://profiles.cache.lol/luxury-format/picture.png)](https://luxury-format.weblog.lol)

---

# Backslash escapes

| Characters | Escape | Description |
|:--|:--|:--|
| \ | \\\ | Backslash |
| \` | \\` | Backtick |
| * | \\* | Asterisk |
| _ | \\_ | Underscore |
| {} | 	\\{\\} | Curly braces |
| [] | \\[\\] | Square brackets |
| () | \\(\\) | Parentheses |
| # | \\# | Hash mark |
| + | \\+ | Plus sign |
| - | \\- | Minus sign (hyphen) |
| . | \\. | Dot |
| ! | \\! | Exclamation mark |

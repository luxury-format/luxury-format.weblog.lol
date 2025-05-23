---
Date: 2025-05-01 00:00
Type: Page
Title: Markdown Cheatsheet
Location: /markdown-cheatsheet
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
*italic*
**bold**  
`inline code`
~~strikethrough~~
```


*italic*
**bold**
`inline code`
~~strikethrough~~

---

# Blockquote

```
> This is a blockquote
```

> This is a blockquote

---

## Lists and Tasks

## Unordered List

```
- Item 1
- Item 2
    - item 3a
    - item 3b
```

- Item 1
- Item 2
    - item 3a
    - item 3b

---

## Ordered List

```
1. Item 1
2. Item 2  
     a. Item 3a  
     b. Item 3b
```

1. Item 1
2. Item 2  
     a. Item 3a  
     b. Item 3b

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
[link](http://google.com)

[link][google]  
[google]: http://google.com

<http://google.com>
```

[link](http://google.com)

[link][google]  
[google]: http://google.com

<http://google.com>

---

# Horizontal line

```
---
```

---

---

# Code

````markdown
```javascript
console.log("This is a block code");
```
````

```javascript
console.log("This is a block code");
```

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
|:--|:--|:--|
| Row 1 | Centered | $1600 |
| Row 2 | Cell | $12 |
```

| Left Column | Center Column | Right Column |
|:--|:--|:--|
| Row 1 | Centered | $1600 |
| Row 2 | Cell | $12 |

---

# Images

```
![GitHub Logo](/images/logo.png)

![Alt Text](url)
```

![GitHub Logo](/images/logo.png)

![Alt Text](url)

---

## Image with link

```
[![GitHub Logo](/images/logo.png)](https://github.com/)

[![Alt Text](image_url)](link_url)
```

[![GitHub Logo](/images/logo.png)](https://github.com/)

[![Alt Text](image_url)](link_url)

---

## Reference style images

```markdown
![alt text][logo]

[logo]: /images/logo.png "Logo Title"
```

![alt text][logo]

[logo]: /images/logo.png "Logo Title"

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

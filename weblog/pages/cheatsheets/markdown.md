---
Date: 2025-05-01 00:00
Type: Page
Title: Markdown Cheatsheet
Location: /cheatsheets/markdown-cheatsheet
Index: Exclude
---

# Markdown Cheatsheet

---

## Headers

```markdown
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

## Blockquotes

```markdown
> This is  
> a blockquote
>
> > Nested  
> > Blockquote
```

> This is  
> a blockquote
>
> > Nested  
> > Blockquote

## Unordered List

```markdown
- Item 1
- Item 2
    - item 3a
    - item 3b

or

- [ ] Checkbox off
- [x] Checkbox on
```

- Item 1
- Item 2
    - item 3a
    - item 3b

or

- [ ] Checkbox off
- [x] Checkbox on

## Ordered List

```markdown
1. Item 1
2. Item 2  
     a. Item 3a  
     b. Item 3b
```

1. Item 1
2. Item 2  
     a. Item 3a  
     b. Item 3b

## Links

```markdown
[link](http://google.com)

[link][google]  
[google]: http://google.com

<http://google.com>
```

[link](http://google.com)

[link][google]  
[google]: http://google.com

<http://google.com>

## Emphasis

```markdown
*italic*
**bold**  
`inline code`
~~struck out~~
```

*italic*
**bold**
`inline code`
~~struck out~~

## Horizontal line

```markdown
---
```

---

## Code

````markdown
```javascript
console.log("This is a block code");
```
````

```javascript
console.log("This is a block code");
```

```markdown
    4 space indent makes a code block
```

    4 space indent makes a code block

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

```markdown
`Inline code` has back-ticks around it.
```

`Inline code` has back-ticks around it.

## Tables

```markdown
| Left Column | Center Column | Right Column |
|:--|:--|:--|
| Row 1 | Centered | $1600 |
| Row 2 | Cell | $12 |
```

| Left Column | Center Column | Right Column |
|:--|:--|:--|
| Row 1 | Centered | $1600 |
| Row 2 | Cell | $12 |

## Images

```markdown
![GitHub Logo](/images/logo.png)

![Alt Text](url)
```

![GitHub Logo](/images/logo.png)

![Alt Text](url)

### Image with link

```markdown
[![GitHub Logo](/images/logo.png)](https://github.com/)

[![Alt Text](image_url)](link_url)
```

[![GitHub Logo](/images/logo.png)](https://github.com/)

[![Alt Text](image_url)](link_url)

### Reference style

```markdown
![alt text][logo]

[logo]: /images/logo.png "Logo Title"
```

![alt text][logo]

[logo]: /images/logo.png "Logo Title"

## Backslash escapes

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

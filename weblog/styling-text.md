---
Date: 2025-04-28 19:40
Title: Styling text
Tags: Markdown, Style, Test, GitHub
---

# Styling text

You can indicate emphasis with **bold**, *italic*, ~~strikethrough~~, <sub>subscript</sub>, <sup>superscript</sup>, <mark>mark</mark>,  text in comment fields and `.md` files.

---

# This is a h1 tag

## This is a h2 tag

#### This is a h4 tag

---

_This text will be italic_

**This text will be bold**

_You **can** combine them_

---

- Item 1
- Item 2
    - Item 2a
    - Item 2b

---

1. Item 1
1. Item 2
1. Item 3
    1. Item 3a
    1. Item 3b

---

![GitHub Logo](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png)

Format: `![Alt Text](url)`

---

http://github.com - automatic!
[GitHub](http://github.com)

---

As Kanye West said:

> We're living the future so
> the present is our past.

---

I think you should use an
`<addr>` element here instead.

---

Syntax highlighting

Here’s an example of how you can use syntax highlighting with [GitHub Flavored Markdown](https://help.github.com/articles/basic-writing-and-formatting-syntax/):

```js:fancyAlert.js
function fancyAlert(arg) {
  if (arg) {
    $.facebox({ div: '#foo' })
  }
}
```

And here's how it looks - nicely colored with styled code titles!

---

Footnotes

Here is a simple footnote[^1]. With some additional text after it.

[^1]: My reference.

---

Task Lists

- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item

---

Tables

You can create tables by assembling a list of words and dividing them with hyphens - (for the first row), and then separating each column with a pipe `|`:

| First Header                | Second Header                |
| --------------------------- | ---------------------------- |
| Content from cell 1         | Content from cell 2          |
| Content in the first column | Content in the second column |

---

Strikethrough

Any word wrapped with two tildes (like `~~this~~`) will appear crossed out.

---

`#007FFF`

---

<svg fill="none" height="128" viewBox="0 0 208 128" width="208" xmlns="http://www.w3.org/2000/svg"><g fill="#000"><path clip-rule="evenodd" d="m15 10c-2.7614 0-5 2.2386-5 5v98c0 2.761 2.2386 5 5 5h178c2.761 0 5-2.239 5-5v-98c0-2.7614-2.239-5-5-5zm-15 5c0-8.28427 6.71573-15 15-15h178c8.284 0 15 6.71573 15 15v98c0 8.284-6.716 15-15 15h-178c-8.28427 0-15-6.716-15-15z" fill-rule="evenodd"/><path d="m30 98v-68h20l20 25 20-25h20v68h-20v-39l-20 25-20-25v39zm125 0-30-33h20v-35h20v35h20z"/></g></svg>

---

<!-- This content will not appear in the rendered Markdown -->

---

> [!NOTE]
> Useful information that users should know, even when skimming content.

---

> [!TIP]
> Helpful advice for doing things better or more easily.

---

> [!IMPORTANT]
> Key information users need to know to achieve their goal.

---

> [!WARNING]
> Urgent info that needs immediate user attention to avoid problems.

---

> [!CAUTION]
> Advises about risks or negative outcomes of certain actions.

---

Heading
=======

Sub-heading
-----------

# Alternative heading

## Alternative sub-heading

---

Paragraphs are separated 
by a blank line.

Two spaces at the end of a line  
produce a line break.

Text attributes _italic_, **bold**, `monospace`.

---

Horizontal rule:

---

Bullet lists nested within numbered list:

  1. fruits
     * apple
     * banana
  2. vegetables
     - carrot
     - broccoli

---

A [link](http://example.com).

---

`![Image](Icon-pictures.png "icon")`

---

> Markdown uses email-style
characters for blockquoting.
>
> Multiple paragraphs need to be prepended individually.

---

Most inline <abbr title="Hypertext Markup Language">HTML</abbr> tags are supported.

---

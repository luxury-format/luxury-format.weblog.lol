---
Date: 2025-05-25 00:00
Type: Page
Title: Test
Location: /test
Tags: Test, Manual
Index: Exclude
---

# Test

###### Weblog Shortcodes

---

Note: Remove `\` after `{` to use **shortcodes!**

# `{toc}`

`{toc}`

Generate Table of Contents - Each Headings in list view, better to use at the top of your **Post** or **Page**.

IDK if this tag works in **Templates**, but it's works in **Posts** and on **Pages**.

{toc}

---

## `{\weblog-title}` - `{\separator}` - `{\author}` - `{\weblog-description}`

In my **Configuration** it's looks next:

```
Weblog title: LUXURY FORMAT
Separator:  ❯ 
Author: Me, Myself and I
Weblog description: Good as Gold!
```

Then using this **shortcodes** I get output like this:

{weblog-title}
{separator}
{author}
{weblog-description}

Note! For **Separator** I use next symbol: `❯` insted of `·`, but you can use any symbol that you want, here is some examples: `-` or `–` or `—` or `|` or `•` or `»` anything, even words!

Make sure you put 2 whitespaces before **Separator:** and one whitespace after your separator, to get output like this: 

{weblog-title}{separator}{weblog-descriprion}

If you don't use whitespaces, then your output will look like this:

{weblog-title}❯{weblog-description}

---

## {\post-title}

Can use it in your **Templates** or **Posts** and **Pages** to get current **post** or **page** title, so currently I use this tag on my page with title: **Test**, so in output below in must be word: **Test**

Here is output: 

{post-title}

---

#### {\weblog-short-title}

This is my custom tag.

In configuration I have added next:

```
Weblog short title: LF.
```

In output I get next: 

{weblog-short-title}

---

### {\recent-posts}

List of your recent posts, in my configuration, I set next: 

```
Recent posts count: 5
```

You can use it in your **Templates**, **Posts** or on **Pages**.

So here is my last 5 post:

{recent-posts}

---

### {\post-list}

List of all your post, better to use on **Archive** page, but you can use it anywhere.

Here is list of all my **Posts**:

{post-list}

---

## {\page-list}

This tag generate automaticaly list of all **Pages** on your **Weblog**.

Note: Except **Tags** page, and your **/** page.

Here is list of all pages in my **Weblog**:

{page-list}

---

## {\multiple-posts}

Seems doesn't work anywhere... 

{multiple-posts}

---

## {\tags}

Note: If you want to use it on your page, you must add in frontmatter next:

`Tags: ` <- and here are your tags, comma separated.

So, creating this page, I have add to frontmatter next:

```
Tags: Test, Manual
```

So in output below I must get this 2 tags: **Test** and **Manual**

{tags}

---

## {\base-path}

{base-path}

You will get in output just plain `/`, you can use this tag for example in your **Posts** and on **Pages** using *Markdown* like this:

```
[(weblog-title)]((base-path))
```

And you will get output like this:

[{weblog-title}]({base-path})

Or using next *HTML* for example in: **Templates**, **Posts**, on **Pages**

```
<a href="(base-path)">(weblog-title)</a>
```

And output will be like this:

<a href="{base-path}">{weblog-title}</a>

---

## {\navigation}

Better to use only in **Templates**, but here is on page:

{navigation}

---

## {\year} - {\month} - {\day}

You can use it anywhere.

{year} - {month} - {day}

---

## {\date} - {\relative-date} - {\unix-date} - {\iso8601-date}

Note: Do not forget to use date in your frontmatter and set **Timezone** and **Date format** in your configuration, my configuration under **Time stuff** looks next:

```
;; Time stuff
;; ----------

Timezone: America/Chicago
Date format: F j, Y
```

Here is output for **{\date}** - **{\relative-date}** - **{\unix-date}** - **{\iso8601-date}** **shortcodes** output:

{date} - {relative-date} - {unix-date} - {iso8601-date}

---

## {\post-title-urlencoded}

{post-title-urlencoded}

---

## {\tag-listing}

List of all your **Tags** on your **Weblog**, like this:

{tag-listing}

---

## {\permalink} - {\slug} - {\location}

{permalink} - {slug} - {location}

---

## {\rss-location} - {\atom-location} - {\json-location}

{rss-location}

{atom-location}

{json-location}

---

## {\rss-url} - {\atom-url}  - {\json-url}

{rss-url}  

{atom-url}  

{json-url}

---

## {\rss} - {\atom} - {\json}

These **shortcodes** use only in your **Templates** head only. And you will get output like this:

`{rss}`

`{atom}`

`{json}`

---

## {\feeds}

This **shortcode** use only in your **Templates** head only. And you will get output like this:

```
{feeds}
```

---

## {\post-number} - {\post-count}

IDK what difference between them...

{post-number} - {post-count}

---

## {\body}

Works everywhere, but better to use in your **Templates** only!

---

## {\titleless-body}

Works everywhere, but better to use in your **Templates** only!

---

## {\previous-page}

Works only in: **Landing Page Template**.

{previous-page}

---

## {\next-page}

Works only in: **Landing Page Template**.

{next-page}

---

## {\search}

**{\search} shortcode** currently doesn't work, instead use next **HTML** code anywhere in your **Templates**, in **Posts** or on **Pages**:

```
<form action="/" method="get" class="search">
<label for="search">Search</label>
<input type="text" name="search">
<button type="submit">Search</button>
</form>
```

Output: 

<form action="/" method="get" class="search">
<label for="search">Search</label>
<input type="text" name="search">
<button type="submit">Search</button>
</form>

Or without next line, if you don't want **Search** word above your search form:

```
<label for="search">Search</label>
```

Like this:

```
<form action="/" method="get" class="search">
<input type="text" name="search">
<button type="submit">Search</button>
</form>
```

Output without **Search** word above your search form:

<form action="/" method="get" class="search">
<input type="text" name="search">
<button type="submit">Search</button>
</form>

{search}

---

## {\profile}

Will "redirect" to your **Profile** page: YOUR-ADDRESS.omg.lol

---

## {\now}

Will "redirect" to your **Now** page: YOUR-ADDRESS.omg.lol/now

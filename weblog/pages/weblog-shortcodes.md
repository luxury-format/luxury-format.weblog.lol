---
Date: 2025-05-25 00:00
Type: Page
Title: Weblog shortcodes
Location: /weblog-shortcodes
Tags: Weblog, Shortcodes
Index: Exclude
---

# Weblog shortcodes

---

> Note: Remove `\` after `{` to use **shortcodes!**

# `{\toc}`

`{\toc}`

Generate Table of Contents - Each Headings in list view, better to use at the top of your **Post** or **Page**.

IDK if this tag works in **Templates**, but it's works in **Posts** and on **Pages**.

Here is example for this page:

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

Then using this **shortcodes** like this:

```
{\weblog-title}{\separator}{\author}{\separator}{\weblog-description}
```

I get next output:

{weblog-title}{separator}{author}{separator}{weblog-description}

Note! For **Separator** I use next symbol: `❯` insted of `·`, but you can use any symbol that you want, here is some examples: `-` or `|` or `•` or `»` anything, even words!

Make sure you put 2 whitespaces before **Separator:** and 1 whitespace after your separator, to get output like this: 

{weblog-title}{separator}{weblog-description}

If you don't use 2 whitespaces before, and 1 whitespace after your **Separator** then your output will look like this:

{weblog-title}❯{weblog-description}

Like you can see above, there is no whitespace between `LUXURY` and `❯`, and no whitespace between `❯` and `Good`, It's can happens when you don't use 2 whitespaces before and 1 whitespace after your **Separator**!

{weblog-title}{separator}{weblog-description}  
{weblog-title}❯{weblog-description}

---

## {\post-title}

You can use it in your **Templates** or **Posts** and **Pages** to get current **post** or **page** title, so currently I use this {\post-title} bellow on my page, this current page title is: **Weblog shortcodes**, so in output below in must be next words: **Weblog shortcodes**

Here is output: 

**{\post-title}** - {post-title}

---

#### {\weblog-short-title}

This is my custom tag. In my configuration I have added next:

```
Weblog short title: LF.
```

In output I get next: 

**{\weblog-short-title}** - {weblog-short-title}

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

Seems doesn't work... 

{multiple-posts}

---

## {\tags}

Note: If you want to use it not for your **Posts**, but for your **Pages**, you must add in frontmatter for your **Page** next:

`Tags: ` <- and here are your tags, comma separated.

So, creating this page, I have add to frontmatter next:

```
Tags: Weblog, Shortcodes
```

So in output below I must get this 2 tags: **Weblog** and **Shortcodes**

{tags}

Note! If you use: **Weblog** and **weblog** for your **Tags**, they counts as same **Tag**.

---

## {\base-path}

**{\base-path}** - {base-path}

You will get in output just plain `/`, you can use this **shortcode** for example in your **Posts** and on **Pages** using *Markdown* like this:

```
[{\weblog-title}]({\base-path})
```

And you will get output like this:

[{weblog-title}]({base-path})

Or using next *HTML* for example in: **Templates**, **Posts**, on **Pages**

```
<a href="{\base-path}">{weblog-title}</a>
```

And output will be like this:

<a href="{base-path}">{weblog-title}</a>

---

## {\navigation}

Better to use only in **Templates**, but here is it on page:

{navigation}

---

## {\year} - {\month} - {\day}

You can use it anywhere.

**{\year}** - {year}  
**{\month}** - {month}  
**{\day}** - {day}

---

## {\date} - {\relative-date} - {\unix-date} - {\iso8601-date}

Note! Do not forget to use **Date:** in your frontmatter and set **Timezone:** and **Date format:** in your configuration, here is my configuration under **Time stuff**:

```
;; Time stuff
;; ----------

Timezone: America/Chicago
Date format: F j, Y
```

Here is output for this page:

**{\date}** - {date}  
**{\relative-date}** - {relative-date}  
**{\unix-date}** - {unix-date}  
**{\iso8601-date}** - {iso8601-date}  

---

## {\post-title-urlencoded}

Here is my page **Weblog shortcodes** URL Encoded title: 

**{\post-title-urlencoded}** - {post-title-urlencoded}

It's works for your **Posts** titles also.

---

## {\tag-listing}

List of all your **Tags** on your **Weblog**, like this:

{tag-listing}

---

## {\permalink} - {\slug} - {\location}

Here is permalink, slug and location for current page **Weblog shortcodes**:

**{\permalink}** - {permalink}  
**{\slug}** - {slug}  
**{\location}** - {location}

---

## {\rss-location} - {\atom-location} - {\json-location}

Here is my RSS, Atom and JSON locations:  

**{\rss-location}** - {rss-location}  
**{\atom-location}** - {atom-location}  
**{\json-location}** - {json-location}  

---

## {\rss-url} - {\atom-url}  - {\json-url}

Here is my RSS, Atom and JSON URL's:  
**{\rss-url}** - {rss-url}  
**{\atom-url}** - {atom-url}  
**{\json-url}** - {json-url}  

---

## {\rss} - {\atom} - {\json}

These **shortcodes** use only in your **Templates** head only. And you will get output like this:

```
{rss}
```

```
{atom}
```

```
{json}
```

---

## {\feeds}

This **shortcode** use only in your **Templates** head only. And you will get output like this:

```
{feeds}
```

---

## {\post-number} - {\post-count}

IDK what difference between them... but here is: 

**{\post-number}** - {post-number}  
**{\post-count}** - {post-count}

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

Or without next line, if you don't want **Search** word next to your search form:

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

Output without **Search** word next to your search form:

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

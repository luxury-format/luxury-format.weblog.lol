---
Date: 2025-05-25 00:00
Type: Page
Title: Test
Location: /test
Index: Exclude
---

# Test

---

Note: Use {} instead of ()

# (toc)

Table of Contents

{toc}

---

## Tags that you can use: in Templates, in posts, on pages

---

### (weblog-title) - (separator) - (author) - (post-title) - (weblog-description)

{weblog-title} - {separator} - {author} - {post-title} - {weblog-description}

---

#### (weblog-short-title) (my custom tag)

In configuration I have added nex:

`Weblog short title: LF.`

{weblog-short-title}

---

### (recent-posts)

{recent-posts}

---

### (post-list)

{post-list}

---

## (page-list)

{page-list}

---

## (multiple-posts)

Seems doesn't work anywhere... 

{multiple-posts}

---

## (tags)

Note: If you want to use it on your page, you must add in frontmatter next:

`Tags: ` <- and here are your tags, comma separated.

{tags}

---

## (base-path)

{base-path}

You will get in output just plain `/`, you can use this tag for example in your **Posts** and on **Pages** using *Markdown* like this:

```
[(weblog-title)]((base-path))
```

And get output like this:

[{weblog-title}]({base-path})

Or using next *HTML* for example in: **Templates**, **Posts**, on **Pages**

```
<a href="(base-path)">(weblog-title)</a>
```

<a href="{base-path}">{weblog-title}</a>

---

## navigation

Better to use only in **Templates**.

{navigation}

---

## (year) - (month) - (day)

You can use it anywhere.

{year} - {month} - {day}

---

## (date) - (relative-date) - (unix-date) - (iso8601-date)

Note: Do not forget to use date in your frontmatter.

{date} - {relative-date} - {unix-date} - {iso8601-date}

---

## (post-title-urlencoded)

{post-title-urlencoded}

---

## (tag-listing)

{tag-listing}

---

## (permalink) - (slug) - (location)

{permalink} - {slug} - {location}

---

## (rss-location) - (atom-location) - (json-location)

{rss-location}

{atom-location}


{json-location}

---

## (rss-url) - (atom-url)  - (json-url)

{rss-url}  

{atom-url}  

{json-url}

---

Next Tags use only in your **Templates** head.

## (rss) - (atom) - (json)

`{rss}`

`{atom}`

`{json}`

---

## (feeds)

```
{feeds}
```

---

## (post-number) - (post-count) ?

IDK what difference between... looks like same numbers...

{post-number} - {post-count}

---

## (body)

Works everywhere, but better to use only in your **Templates** only!

---

## (titleless-body)

Works everywhere, but better to use only in your **Templates** only!

---

## (previous-page)

Works only in: **Landing Page Template**.

{previous-page}

---

## (next-page)

Works only in: **Landing Page Template**.

{next-page}

---

## (search)

Doesn't work, instead use next **HTML** code anywhere:

```
<form action="/" method="get" class="search">
<label for="search">Search</label>
<input type="text" name="search">
<button type="submit">Search</button>
</form>
```

{search}

---

## (profile)

Will "redirect" to: YOUR-ADDRESS.omg.lol - **Profile** page

---

## (now)

Will "redirect" to: YOURADDRES.omg.lol/now - **Now** page

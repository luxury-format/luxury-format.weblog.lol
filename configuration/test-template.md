---
Type: Template
Title: Test Template
Location: /test-template
---

<!DOCTYPE html>
<html lang="en">
<!-- TestTemplate -->
<!-- Weblog.lol/configuration/test-template.md -->
<!-- HEAD -->
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>{weblog-title}{separator}{post-title}</title>
<meta property="og:title" content="{weblog-title}{separator}{post-title}">
<meta name="description" content="{weblog-description}">
<meta property="og:description" content="{weblog-description}">
<meta property="og:type" content="article">
<meta property="og:url" content="{permalink}">
<!-- <meta property="og:url" content="{location}"> -->
<meta property="og:image" content="https://profiles.cache.lol/luxury-format/picture.png">
<!-- FEDIVERSE CREATOR -->
<meta name="fediverse:creator" content="@luxury_format@social.lol">
<!-- FEEDS -->
<link rel="alternate" type="application/atom+xml" title="{weblog-title} Atom Feed" href="https://luxury-format.weblog.lol/atom.xml">
<link rel="alternate" type="application/rss+xml" title="{weblog-title} RSS Feed" href="https://luxury-format.weblog.lol/rss.xml">
<link rel="alternate" type="application/json" title="{weblog-title} JSON Feed" href="https://luxury-format.weblog.lol/feed.json">
<!-- BLOGROLL -->
<!-- <link rel="blogroll" type="text/xml" href="/blogroll/opml.xml" title="{weblog-title} blogroll"> -->
<!-- ICONS -->
<!-- FAVICON.ICO -->
<link rel='icon' href='https://luxury-format.omg.lol/favicon.ico'>
<!-- FAVICON.ICO for older browsers/tools -->
<link rel="shortcut icon" href="https://luxury-format.omg.lol/favicon.ico">
<!-- iOS Home‑Screen icon -->
<link rel="apple-touch-icon" href="https://profiles.cache.lol/luxury-format/picture.png">
<meta name="apple-mobile-web-app-title" content="LF.">
<meta name="apple-mobile-web-app-capable" content="yes">
<!-- Safari pinned tab -->
<!-- A monochrome SVG icon that adapts to Safari’s toolbar theme
<link rel="mask-icon" href="https://profiles.cache.lol/luxury-format/picture.png" color="#0062FF"> -->
<!-- Tile color in Windows/Edge
<meta name="msapplication-TileColor" content="#0062FF">
<meta name="msapplication-TileImage" content="https://profiles.cache.lol/luxury-format/picture.png"> -->
<link rel="manifest" href="/site.webmanifest">
<!-- <meta name="msapplication-TileColor" content="#0062FF"> -->
<!-- COLOR SCHEME: LIGHT DARK -->
<meta name="color-scheme" content="light dark">
<!-- THEME COLOR -->
<meta name="theme-color" content="#F8F8F2" media="(prefers-color-scheme: light)">
<meta name="theme-color" content="#1C1C1E" media="(prefers-color-scheme: dark)">
<!-- FONTS: Atkinson Hyperlegible and Source Code Pro -->
<link rel="preconnect" href="https://fonts.bunny.net" crossorigin="anonymous" referrerpolicy="no-referrer">
<link rel="stylesheet" href="https://fonts.bunny.net/css?family=atkinson-hyperlegible:400,400i,700,700i%7Csource-code-pro:400,700&display=swap" crossorigin="anonymous" referrerpolicy="no-referrer">
<!-- Font Awesome Icons -->
<link rel="preconnect" href="https://cdnjs.cloudflare.com" crossorigin="anonymous" referrerpolicy="no-referrer">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.2/css/all.min.css" crossorigin="anonymous" referrerpolicy="no-referrer">
<!-- Highlight -->
<!-- /style.css -->
<link rel="stylesheet" href="/style.css">
</head>
<!-- BODY -->
<body>
<!-- HEADER -->
<header class="weblog-header">
<!-- First row: Logo+Title and Social Icons -->
<div class="header-top-row">
<div class="logo-title">
<a href="/">
<img src="https://profiles.cache.lol/luxury-format/picture.png" alt="{weblog-title} Logo">
<h1 class="weblog-title">
<span class="short">{weblog-short-title}</span>
<span class="long">{weblog-title}</span>
</h1>
</a>
</div>
<div class="header-icons">
<a href="https://social.lol/@luxury_format" aria-label="Mastodon"><i class="fa-brands fa-mastodon"></i><span>Mastodon</span></a>
<a href="/feeds" aria-label="RSS Feeds"><i class="fa-solid fa-rss"></i><span>Subscribe</span></a>
</div>
</div>
<!-- Second row: Navigation Menu -->
<div class="weblog-navigation">
{navigation}
</div>
</header>
<!-- MAIN NO TITLE LINK -->
<main class="no-title-link">
<p></p>weblog-title: start >{weblog-title}< finish</p>
<hr>
<p>weblog-short-title: start >{weblog-short-title}< finish</p>
<hr>
<p>weblog-description: start >{weblog-description}< finish</p>
<hr>
<p>separator: start >{separator}< finish</p>
<hr>
<p>recent-posts: start >{recent-posts}< finish</p>
<hr>
<p>post-list: start >{post-list}< finish</p>
<hr>
<p>page-list: start >{page-list}< finish</p>
<hr>
<p>multiple-posts: start >{multiple-posts}< finish</p>
<hr>
<p>tags: start >{tags}< finish</p>
<hr>
<p>base-path: start >{base-path}< finish</p>
<hr>
<p>navigation: start >{navigation}< finish</p>
<hr>
<p>relative-date: start >{relative-date}< finish</p>
<hr>
<p>unix-date: start >{unix-date}< finish</p>
<hr>
<p>iso8601-date: start >{iso8601-date}< finish</p>
<hr>
<p>post-title-urlencoded: start >{post-title-urlencoded}< finish</p>
<hr>
<p>tag-listing: start >{tag-listing}< finish</p>
<hr>
<p>date: start >{date}< finish</p>
<hr>
<p>slug: start >{slug}< finish</p>
<hr>
<p>location: start >{location}< finish</p>
<hr>
<p>rss-location: start >{rss-location}< finish</p>
<hr>
<p>atom-location: start >{atom-location}< finish</p>
<hr>
<p>json-location: start >{json-location}< finish</p>
<hr>
<p>rss-url: start >{rss-url}< finish</p>
<hr>
<p>atom-url: start >{atom-url}< finish</p>
<hr>
<p>json-url: start >{json-url}< finish</p>
<hr>
<p>rss: start >{rss}< finish</p>
<hr>
<p>atom: start >{atom}< finish</p>
<hr>
<p>json: start >{json}< finish</p>
<hr>
<p>feeds: start >{feeds}< finish</p>
<hr>
<p>permalink: start >{permalink}< finish</p>
<hr>
<p>year: start >{year}< finish</p>
<hr>
<p>month: start >{month}< finish</p>
<hr>
<p>day: start >{day}< finish</p>
<hr>
<p>post-number: start >{post-number}< finish</p>
<hr>
<p>post-count: start>{post-count}< finish</p>
<hr>
<p>body: start >{body}< finish</p>
<hr>
<p>titleless-body: start >{titleless-body}< finish</p>
<hr>
<p>now: start >{now}< finish</p>
<hr>
<p>profile: start >{profile}< finish</p>
<hr>
<p>previous-page: start >{previous-page}< finish</p>
<hr>
<p>next-page: start >{next-page}< finish</p>
<hr>
<pre>
<code>
weblog-title: start >{weblog-title}< finish
<hr>
weblog-short-title: start >{weblog-short-title}< finish
<hr>
weblog-description: start >{weblog-description}< finish
<hr>
separator: start >{separator}< finish
<hr>
recent-posts: start >{recent-posts}< finish
<hr>
post-list: start >{post-list}< finish
<hr>
page-list: start >{page-list}< finish
<hr>
multiple-posts: start >{multiple-posts}< finish
<hr>
tags: start >{tags}< finish
<hr>
base-path: start >{base-path}< finish
<hr>
navigation: start >{navigation}< finish
<hr>
relative-date: start >{relative-date}< finish
<hr>
unix-date: start >{unix-date}< finish
<hr>
iso8601-date: start >{iso8601-date}< finish
<hr>
post-title-urlencoded: start >{post-title-urlencoded}< finish
<hr>
tag-listing: start >{tag-listing}< finish
<hr>
date: start >{date}< finish
<hr>
slug: start >{slug}< finish
<hr>
location: start >{location}< finish
<hr>
rss-location: start >{rss-location}< finish
<hr>
atom-location: start >{atom-location}< finish
<hr>
json-location: start >{json-location}< finish
<hr>
rss-url: start >{rss-url}< finish
<hr>
atom-url: start >{atom-url}< finish
<hr>
json-url: start >{json-url}< finish
<hr>
rss: start >{rss}< finish
<hr>
atom: start >{atom}< finish
<hr>
json: start >{json}< finish
<hr>
feeds: start >{feeds}< finish
<hr>
permalink: start >{permalink}< finish
<hr>
year: start >{year}< finish
<hr>
month: start >{month}< finish
<hr>
day: start >{day}< finish
<hr>
post-number: start >{post-number}< finish
<hr>
post-count: start>{post-count}< finish
<hr>
body: start >{body}< finish
<hr>
titleless-body: start >{titleless-body}< finish
<hr>
now: start >{now}< finish
<hr>
profile: start >{profile}< finish
<hr>
previous-page: start >{previous-page}< finish
<hr>
next-page: start >{next-page}< finish
<hr>
</code>
</pre>
</main>
<!-- FOOTER -->
<footer>
<hr>
<p>&copy; {year} <a href="/">{weblog-title}</a></p>
<p class="footer-weblog-p">Made with <a href="https://home.omg.lol/referred-by/luxury-format">Weblog.lol</a></p>
</footer>
</body>
</html>

---
Type: Template
Title: Tag Listing Template
---

// Note: tag listing order can be "alphabetical", "ascending", or "descending" where alphabetical sorts by the tag name and ascending/descending sorts by the count of entries with that tag
<!DOCTYPE html>
<html lang="en">
<!-- Page Template -->
<!-- Weblog.lol/configuration/landing-page-template.md -->
<head>
<title>{weblog-title}{separator}{post-title}</title>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="preconnect" href="https://cdnjs.cloudflare.com">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.2/css/all.min.css">
<link rel="stylesheet" href="/style.css" type="text/css">
</head>
<body>

<header>
<h1 class="weblog-title"><a href="/">{weblog-title}</a></h1>
{navigation}
<hr>
</header>

<main class="no-title-link">

Tag listing order: ascending
Tag listing format: <<[
<h2>TAGS</h2>
<ul>
[tag:begin]<li><a href="$location">$tag</a> ($count)</li>[tag:end]
</ul>
]>>

</main>

<footer>
<hr>

<script src="https://status.lol/luxury-format.js?time&link&fluent&pretty"></script>

<hr>

<p>&copy; {year} <a href="/">{weblog-title}</a></p>

<p class="footer-weblog-p">Made with <a href="https://weblog.lol">Weblog.lol</a>.</p>
</footer>

</body>
</html>
